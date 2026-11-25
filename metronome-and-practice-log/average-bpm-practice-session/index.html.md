# How to Calculate Average BPM of a Practice Session

> Work out the time-weighted average tempo of a practice session when you change BPM along the way, with a worked example and common mistakes.

- Web: https://apps.schimpf.es/metronome-and-practice-log/average-bpm-practice-session/
- App: Metronome & Practice Log, https://apps.schimpf.es/metronome-and-practice-log/index.md
If you change the metronome tempo during practice, one number for the whole session is useful: the average BPM. A plain average of the tempos you used gives the wrong answer. You need a time-weighted average.

## The formula

**average BPM = (BPM1 x time1 + BPM2 x time2 + ...) / (time1 + time2 + ...)**

Each tempo counts in proportion to how long you stayed on it. Use the same unit of time for every part. Minutes or seconds both work.

This is the formula Metronome & Practice Log uses. While you play, it adds up tempo multiplied by elapsed time, then divides by total elapsed time when you pause.

## Worked example

You practice a piece for 20 minutes:

1. 10 minutes at 80 BPM.
2. 5 minutes at 100 BPM.
3. 5 minutes at 120 BPM.

Step by step:

1. Multiply each tempo by its time: 80 x 10 = 800, 100 x 5 = 500, 120 x 5 = 600.
2. Add them: 800 + 500 + 600 = 1,900.
3. Add the times: 10 + 5 + 5 = 20 minutes.
4. Divide: 1,900 / 20 = 95 BPM.

```
80 BPM  |##########  10 min
100 BPM |#####        5 min
120 BPM |#####        5 min
Average: 95 BPM
```

The plain average of 80, 100 and 120 is 100. That is too high, because you spent half the session at the slowest tempo.

## Average BPM and last BPM are different

A session has two tempo numbers worth keeping:

- Last BPM is the tempo when you stopped. In the example it is 120.
- Average BPM is the time-weighted figure. In the example it is 95.

Last BPM shows where you ended. Average BPM shows how you worked. If you warm up slowly and finish fast, the last BPM looks high while the average covers the whole session. Metronome & Practice Log stores both for every session.

## A second example with seconds

You play for 45 seconds at 60 BPM, then 15 seconds at 90 BPM.

1. 60 x 45 = 2,700.
2. 90 x 15 = 1,350.
3. Total: 4,050, divided by 60 seconds = 67.5 BPM.

## Common mistakes

- Averaging the tempos without weights. Always weigh by time.
- Counting pauses. Time with the metronome stopped does not belong in the calculation. The app starts a session when you press play and stops when you pause, so only playing time counts.
- Mixing units. Do not use minutes for one part and seconds for another.
- Expecting a late tempo change to matter. A change near the end barely moves the average, which is correct.

## Using average BPM to track progress

One session says little, so log the same piece over several weeks and watch the average climb:

| Week | Average BPM |
|---|---|
| 1 | 72 |
| 2 | 80 |
| 3 | 88 |
| 4 | 96 |

An increase of about 8 BPM per week is a clear trend. If the number stalls, hold the tempo for a few more days before you push on.

## What the app records

- A session starts when you press play and ends when you pause.
- Sessions shorter than 30 seconds are ignored, so a quick tempo test does not clutter the log.
- Each session saves its piece (or "General"), the time signature, the last tempo and the time-weighted average tempo.
- You can edit or delete any session, with undo.
- Every day with at least one minute of practice counts toward your daily streak.
- Per-piece tempo progress graphs and a 12-week view are part of the Pro purchase. The 7-day chart works without it.

All data stays on your device. The app has no internet permission and no account.

## Try it in the app

Metronome & Practice Log is an Android metronome that logs practice automatically, so you do not need to do this arithmetic by hand. Search for it on Google Play.
