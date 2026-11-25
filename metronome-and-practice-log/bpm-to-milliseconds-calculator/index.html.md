# BPM to Milliseconds Calculator and Formula

> Convert BPM to milliseconds per beat with one formula, worked examples, and a table of note lengths from whole notes to sixteenths.

- Web: https://apps.schimpf.es/metronome-and-practice-log/bpm-to-milliseconds-calculator/
- App: Metronome & Practice Log, https://apps.schimpf.es/metronome-and-practice-log/index.md
Delay times, click tracks and tempo-synced effects often ask for milliseconds, while music is written in beats per minute (BPM). The conversion is one division.

## The formula

One minute has 60,000 milliseconds. If a tempo has a certain number of beats in that minute, divide:

**milliseconds per beat = 60,000 / BPM**

To go the other way:

**BPM = 60,000 / milliseconds per beat**

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/metronome-and-practice-log/bpm-to-milliseconds-calculator/

## Worked example

You practice at 90 BPM and want the time between clicks.

1. Write the formula: 60,000 / 90.
2. Divide: 666.67.
3. The gap between beats is about 667 ms.

Check it: 90 beats of 666.67 ms each is 60,000 ms, which is one minute.

## Common tempos

| BPM | ms per beat |
|---|---|
| 40 | 1500 |
| 60 | 1000 |
| 72 | 833.3 |
| 80 | 750 |
| 100 | 600 |
| 120 | 500 |
| 144 | 416.7 |
| 180 | 333.3 |
| 240 | 250 |
| 300 | 200 |

```
 60 BPM |##########  1000 ms
120 BPM |#####       500 ms
240 BPM |###         250 ms
```

Doubling the BPM halves the gap.

## Note lengths at a given tempo

The BPM number counts one kind of beat, usually the quarter note. Other note values are fractions of it. At 100 BPM, with the quarter note as the beat (600 ms):

| Note | Share of a quarter note | Length at 100 BPM |
|---|---|---|
| Whole | 4 | 2400 ms |
| Half | 2 | 1200 ms |
| Quarter | 1 | 600 ms |
| Eighth | 1/2 | 300 ms |
| Eighth triplet | 1/3 | 200 ms |
| Sixteenth | 1/4 | 150 ms |

To get any of these, calculate the quarter note with the formula and multiply by the share. A dotted note is 1.5 times its plain length. A dotted quarter at 100 BPM is 600 x 1.5 = 900 ms.

## What counts as a beat

Be careful when the beat is not a quarter note. In 6/8, a score may mark a dotted quarter as the beat, which gives two beats per bar. If a metronome clicks every eighth note instead, the BPM you set is the number of eighth notes per minute, so it is three times the dotted-quarter tempo. A dotted quarter at 60 BPM equals eighth notes at 180 BPM.

Metronome & Practice Log uses the same rule: the BPM you set is the number of clicks per minute, and each beat of the bar gets one click. In 6/8 that means six clicks per bar. By default the app accents the first and fourth click, so you hear two dotted-quarter pulses. You can change the accent on every beat.

## Why timing precision matters

At 120 BPM a beat is 500 ms. An error of 10 ms is 2 percent of the beat, and errors from ordinary timers add up over a bar or two. Phone metronomes that use them can wander, especially with the screen off.

The app counts audio samples instead of timers. Each beat is written to the audio output with its exact length, and the fractional part of the length is carried to the next beat, so the tempo does not drift. For example, at 48,000 samples per second and 100 BPM, a beat is 28,800 samples, an exact number. At 70 BPM it is 41,142.857 samples, and the extra fraction is carried forward so the average stays exactly at 70 BPM. Tempo changes apply from the next beat.

## Rounding

- For delay plugins, round to the nearest whole millisecond. The error is under half a millisecond.
- For click tracks, keep two decimals if the tool allows it.
- Do not round the BPM. 666.67 ms corresponds to 90 BPM, while 667 ms gives 89.96 BPM.

## Try it in the app

Metronome & Practice Log is an Android metronome that works offline and logs each practice session automatically. It runs from 30 to 300 BPM, which is 2000 ms down to 200 ms per beat. It keeps steady time in the background and with the screen off, and offers screen flash and vibration on the beat. Search for it on Google Play.
