# Nagios and Icinga soft vs hard states explained

> What soft and hard states mean in Nagios and Icinga 2, how check attempts work, and how long a failure takes to become hard. With a worked example.

- Web: https://apps.schimpf.es/tinag2/nagios-soft-vs-hard-states-explained/
- App: Tinag2: Icinga & Nagios Alerts, https://apps.schimpf.es/tinag2/index.md
A service in Nagios, Naemon or Icinga 2 does not alert on the first failed check. It first goes through a soft state and only becomes hard after several failed checks in a row. This page explains the states, the attempt counter and the timing, with one worked example.

## The four service states

Every check plugin ends with an exit code. The monitoring core turns that code into a state. This follows the Nagios Plugin Development Guidelines (nagios-plugins.org) and the Icinga 2 documentation, chapter "Monitoring Basics".

| Exit code | State | Meaning |
|---|---|---|
| 0 | OK | The check passed. |
| 1 | WARNING | The value is outside the warning threshold. |
| 2 | CRITICAL | The value is outside the critical threshold, or the service is failing. |
| 3 | UNKNOWN | The plugin could not decide, for example a bad argument or a timeout. |

Hosts are simpler. A host is UP or DOWN. Thruk also reports UNREACHABLE, a host that cannot be reached because something between the monitoring server and the host is down.

## Soft and hard state types

The state type says how sure the core is about the problem.

- **Soft**: a check failed, but the number of failed checks is still below `max_check_attempts`. The core keeps checking, now at the shorter retry interval.
- **Hard**: the failed checks reached `max_check_attempts`, or the state changed from one hard problem state to another. Notifications are normally sent from this point.

A soft state that returns to OK before the last attempt never becomes hard. This filters out short blips such as one lost packet.

## The three settings that set the timing

Each host and service has these settings in its configuration:

1. `check_interval`: time between checks while the state is stable.
2. `retry_interval`: time between checks while the state is soft.
3. `max_check_attempts`: how many failed checks in a row make the state hard. The first failed check counts as attempt 1.

## How long until a failure becomes hard

Counting from the first failed check:

time to hard = (`max_check_attempts` − 1) × `retry_interval`

Counting from the moment the service really broke, the worst case adds one full check interval, because the failure can start right after a good check:

worst case = `check_interval` + (`max_check_attempts` − 1) × `retry_interval`

## Worked example

Settings: `check_interval` 5 minutes, `retry_interval` 1 minute, `max_check_attempts` 3.

1. 09:55:00. Check passes. State OK.
2. 09:55:30. The service breaks. Nothing is noticed yet.
3. 10:00:00. Check fails. State CRITICAL, soft, attempt 1/3.
4. 10:01:00. Check fails. CRITICAL, soft, attempt 2/3.
5. 10:02:00. Check fails. CRITICAL, hard, attempt 3/3. Notifications start.

The state became hard 2 minutes after the first failed check: (3 − 1) × 1 minute. It became hard 6.5 minutes after the service really broke. The worst case for these settings is 5 + 2 = 7 minutes.

```
worst case: 5 min (check interval) + 2 x 1 min (retries) = 7 min
            |#####|##|
```

If the check at 10:01:00 had passed, the service would have returned to OK without ever becoming hard, and nobody would have been notified.

## Tuning the numbers

- Raising `max_check_attempts` removes more false alarms but delays real ones.
- A shorter `retry_interval` makes the hard state come sooner without more noise on the stable-state schedule.
- For a very important service, a low `max_check_attempts` such as 2 plus a short retry interval keeps the delay small.

## One detail in Icinga 2

Icinga 2 resets its internal `check_attempt` counter to 1 when a state turns hard. If you read the raw API value on a hard problem, it can show 1/3 instead of 3/3. Tinag2 shows hard problems as max/max, like Nagios does.

## Soft and hard states in Tinag2

Tinag2 is an Android client for Icinga 2 and for Nagios/Naemon through Thruk. It reads the state type and the attempt counter from the server and uses them in three places:

- **Problem detail** shows the state type and the attempts, for example "soft 2/3" or "hard 3/3".
- **Hard only filter** on the Problems screen hides soft problems.
- **Alert rules** skip soft states by default, so you are only notified about hard problems. You can switch that off on the Alerts screen. There is also an option to wait 5 minutes before alerting, measured from the problem's last state change, which damps checks that flip back and forth.

The app asks the server for data every 15 minutes in the background, and when you pull to refresh. A hard problem therefore reaches your phone at the next sync after it becomes hard, not at the exact second.

Tinag2 only reads and acts on problems. It does not change check intervals or attempt counts; do that in your Icinga or Nagios configuration.

Tinag2 lets you filter, search and acknowledge hard problems from your phone, and sends alerts only for the problems that matter to you. Add your Icinga 2 or Thruk server in the app to try it.
