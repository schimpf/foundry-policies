# Alarm Not Going Off on Android: Causes and Fixes

> Why an Android alarm stays silent or rings late, and a checklist of settings to fix it, from exact alarms to battery limits.

- Web: https://apps.schimpf.es/alarm-clock/alarm-not-going-off-android/
- App: Alarm Clock: Wake-Up Missions, https://apps.schimpf.es/alarm-clock/index.md
An alarm that does not ring is usually blocked by a setting. This page lists the common causes on Android and how to check each one.

## Quick checklist

1. The alarm is switched on, and the right days are selected.
2. The time is correct (check AM and PM).
3. The alarm volume is up (not the media volume).
4. Notifications for the alarm app are allowed.
5. The exact alarm permission is allowed, if your Android version asks for it.
6. Battery optimization does not restrict the app.
7. Your phone maker's background limits do not stop the app.
8. You tested the alarm for one minute ahead.

## Cause 1: The alarm volume is low

Android keeps separate volumes for media, ringtone and alarms. Turning down the media volume does not change the alarm volume. Open the volume panel, expand it and check the alarm slider. Alarm Clock plays on the alarm stream, so it rings even in silent mode. It also raises the volume gradually over a time you set, from 0 to 120 seconds (the default is 30). If you set a long ramp, the first seconds are quiet by design. Set it to 0 to start at full volume.

## Cause 2: Exact alarm permission

Android 12 and 12L (API 31 and 32) can block apps from setting exact alarms until you allow it. Android 13 and later grant it automatically to apps that are alarm clocks. See *Schedule alarms*, Android Developers documentation. If you are on Android 12 or 12L, open the app's special access settings and allow alarms and reminders.

## Cause 3: Notifications are off

If notifications are blocked, the ringing screen may not appear. Open the app's notification settings and turn them on. On Android 13 and later, the app must also ask for the notification permission.

## Cause 4: Full-screen alerts

On Android 14 and later, an app needs the full-screen notification permission to show the ringing screen over the lock screen. Alarm apps qualify. Check the permission in the app's settings if the screen stays dark when the alarm rings.

## Cause 5: Battery optimization

Android saves power by limiting apps that run in the background. Exempting your alarm app from battery optimization lowers the risk that the system delays or stops it. Open the battery settings for the app and choose the unrestricted option.

## Cause 6: Phone-maker battery savers

Some makers add their own limits on top of Android. Xiaomi, Redmi, Poco, Samsung, Huawei, Honor, OnePlus, Oppo, Vivo and Realme are the usual ones. They may close apps swiped from recents or put them to sleep. The community site *Don't kill my app* (dontkillmyapp.com) tracks what each maker does. Alarm Clock's setup guide includes steps for these brands.

## Cause 7: Reboots and time changes

An alarm must be set again after a restart, after a time change and after a time zone change. Alarm Clock does this on its own. If you use another app, open it once after an update or restart and check that the next alarm is still shown.

## Test the alarm

Do not wait until tomorrow to find out. Set a test alarm one minute ahead and lock the screen. If it rings and the screen turns on, the settings work.

## How Alarm Clock helps

- A first-run setup wizard walks through the exact alarm, notification, full-screen and battery settings, and shows brand-specific steps.
- A self-test alarm rings one minute later.
- You can reopen the wizard from Settings at any time.
- The alarm is set through the system alarm clock API, which Android treats as a user-visible alarm.
- If you move or delete your own sound file, a bundled tone plays instead of silence.
- If you leave a wake-up mission, the alarm rings again after one minute, and it also rings again after a reboot while it was sounding.

Alarm Clock has no internet permission, no account and no analytics. It is open source under the GNU GPL v3 or later. Open the app, finish the setup wizard once, and run the self-test.
