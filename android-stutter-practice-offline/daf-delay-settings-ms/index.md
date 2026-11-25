# DAF Delay Settings in ms: What to Set and Why

> How much delay to set for delayed auditory feedback, why your phone adds its own delay, and a worked example with a calculator.

- Web: https://apps.schimpf.es/android-stutter-practice-offline/daf-delay-settings-ms/
- App: Stutter Practice: DAF, https://apps.schimpf.es/android-stutter-practice-offline/index.md
Delayed auditory feedback (DAF) plays your own voice back to you a fraction of a second late. The setting you choose is a delay in milliseconds (ms). The catch on a phone is that the audio path adds delay of its own, so the number you set is not always the delay you hear. This page shows the formula and two worked examples.

## What DAF is

You speak into the microphone, and the app plays your voice into your headphones after a short delay. DAF is a technique used in speech therapy for stuttering. How much it helps differs from person to person, and the right setting is best found with a speech and language therapist. This page is general information and not medical advice.

## Typical delay values

Stutter Practice lets you set the delay from 25 to 250 ms. It starts at 75 ms, and offers four quick presets:

| Preset | Delay |
|---|---|
| 1 | 50 ms |
| 2 | 75 ms (also the starting value) |
| 3 | 100 ms |
| 4 | 150 ms |

Change the value in small steps and keep what feels comfortable.

## Why the phone adds delay

Every Android phone has some delay between the microphone and the headphones. It comes from the input buffer, the processing and the output buffer. This is called device latency. If you set 100 ms in an app that ignores it, you may hear 100 ms plus the device latency.

Stutter Practice reads the device latency during a short calibration and lets you fine-tune it by tapping along with clicks. The stored value is:

- Device latency = measured base latency + fine-tune
- The fine-tune is the median lateness of your last taps, between 0 and 60 ms.

## The formula

- Delay the app adds = target delay − device latency
- It never goes below zero.
- If the target is lower than the device latency, the delay you hear is the device latency alone, and the app shows a warning.

## Worked examples

Assume calibration found a device latency of 40 ms.

1. You want 100 ms. The app adds 100 − 40 = 60 ms. You hear about 100 ms in total.
2. You want 75 ms. The app adds 75 − 40 = 35 ms.
3. You want 25 ms. 25 − 40 is negative, so the app adds 0 ms. You hear about 40 ms, which is higher than you asked for. The app warns you that your setting is below the device delay.

Now assume a device latency of 70 ms, which is common on some phones:

| Target | Added by app | Heard (about) |
|---|---|---|
| 50 ms | 0 ms | 70 ms |
| 75 ms | 5 ms | 75 ms |
| 100 ms | 30 ms | 100 ms |
| 150 ms | 80 ms | 150 ms |

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/android-stutter-practice-offline/daf-delay-settings-ms/

## Headphones matter

- Use wired or USB headphones. They add the least delay and keep it steady.
- Bluetooth adds extra delay that varies from one device to the next, so the app shows a warning when a Bluetooth output is active.
- The phone speaker is also flagged, because it adds extra delay too.
- Calibration is stored for the output you used. If you switch to different headphones, recalibrate.

## Practice with Stutter Practice

Stutter Practice is an Android app for DAF, paced speech and easy onset exercises. It works without an internet connection, has no network permission, and processes your voice live without recording it. The delay can be changed with a slider, plus and minus buttons or presets, while DAF is running. You can also combine DAF with read-aloud texts.
