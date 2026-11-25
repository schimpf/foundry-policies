# Snooze Time Calculator: How Late Will You Wake Up?

> Work out how many minutes snoozing costs you and when the last alarm rings. Includes a calculator and a worked example.

- Web: https://apps.schimpf.es/alarm-clock/snooze-time-calculator/
- App: Alarm Clock: Wake-Up Missions, https://apps.schimpf.es/alarm-clock/index.md
Every snooze tap pushes your wake-up later. This page shows the formula, a worked example and a small calculator, so you can see what your snooze habit really costs.

## The formula

The extra time you lose follows this formula:

**Total delay = snooze interval × number of snoozes**

The last alarm rings at:

**Last ring = alarm time + total delay**

A few points about how this works in practice:

- The interval is counted from the moment you tap Snooze.
- If you let the alarm ring for a while before you tap, the real delay is a little longer than the formula says.
- The formula gives the minimum delay. It is exact when you tap Snooze right away.

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/alarm-clock/snooze-time-calculator/

## Worked example

You set an alarm for 6:30 with a 5-minute snooze interval and tap Snooze 3 times.

1. Total delay = 5 min × 3 = 15 min.
2. Last ring = 6:30 + 15 min = 6:45.
3. You get up at 6:45 at the earliest.

The same alarm with a 10-minute interval and 4 snoozes:

1. Total delay = 10 min × 4 = 40 min.
2. Last ring = 6:30 + 40 min = 7:10.

Here is the delay for a few common settings:

| Interval | Snoozes | Total delay |
| --- | --- | --- |
| 5 min | 1 | 5 min |
| 5 min | 3 | 15 min |
| 9 min | 3 | 27 min |
| 10 min | 4 | 40 min |
| 15 min | 5 | 75 min |
| 30 min | 10 | 300 min (5 h) |

## Read the result as a budget

If you must be out of bed at 7:00 and you plan to snooze, work backward:

1. Pick your interval and the number of snoozes you expect.
2. Multiply them to get the total delay.
3. Subtract that delay from 7:00 to get the alarm time.

For a 5-minute interval and 3 snoozes, the delay is 15 minutes, so the alarm goes at 6:45. The last ring lands at 7:00. Add a small buffer for the time between rings, because you will not tap Snooze at the exact second the alarm starts.

## Set a limit that you can live with

Unlimited snoozing has no upper bound, so the total delay has none either. A cap makes the cost known in advance. When the cap is reached, the alarm stops offering Snooze and you have to get up.

## Snooze settings in Alarm Clock

Alarm Clock lets you set both numbers for each alarm:

- **Interval:** 1 to 30 minutes. The default is 5 minutes.
- **Maximum snoozes:** 0 to 10, or unlimited. The default is 3.
- **0 snoozes** turns snooze off for that alarm.
- A chip on the ringing screen shows your snooze count.
- Snooze is always available on the ringing screen until you reach your limit.
- Once a wake-up mission has started, snoozing is no longer possible. You finish the mission first.

With the defaults, the worst case is 5 × 3 = 15 minutes of extra sleep, which matches the first worked example above.

## Combine snooze with a mission

If snooze is the habit you want to break, set the maximum to a small number and add a mission. Alarm Clock offers four: math problems, shaking the phone, scanning a QR code or barcode, and walking a number of steps. The mission cannot be skipped. If you fail it three times, the app offers an easier math problem so you are never stuck.

Alarm Clock rings on the exact minute through the system alarm clock API, uses the alarm volume so it also rings on silent, and has no internet permission. It is open source under the GNU GPL v3 or later. Set your interval and snooze limit in the alarm editor.
