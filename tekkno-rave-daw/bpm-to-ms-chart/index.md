# BPM to ms Chart for Hard Techno, 140 to 220 BPM

> Milliseconds per beat, 16th note and bar for 140 to 220 BPM, with the formulas and a worked example for song length in seconds.

- Web: https://apps.schimpf.es/tekkno-rave-daw/bpm-to-ms-chart/
- App: Tekkno Rave DAW: Beat Maker, https://apps.schimpf.es/tekkno-rave-daw/index.md
Delays, loop lengths and sample cuts are easier when you know how long a beat lasts in milliseconds. This page gives a chart for the tempo range used in hard techno and hardcore (140 to 220 BPM), the formulas behind it, and a small calculator.

## The formulas

BPM means beats per minute. One minute has 60,000 milliseconds, so:

- Beat (quarter note) in ms = 60000 / BPM
- 8th note in ms = 30000 / BPM
- 16th note in ms = 15000 / BPM
- Bar of 4/4 in ms = 240000 / BPM

A bar of 4/4 holds 4 beats, which is 16 sixteenth notes. Most step sequencers, including a 16-step pattern, treat one step as one 16th note.

## BPM to ms chart

| BPM | 16th note (ms) | 8th note (ms) | Beat (ms) | Bar (ms) |
|-----|----------------|---------------|-----------|----------|
| 140 | 107.14 | 214.29 | 428.57 | 1714.29 |
| 150 | 100.00 | 200.00 | 400.00 | 1600.00 |
| 160 | 93.75 | 187.50 | 375.00 | 1500.00 |
| 170 | 88.24 | 176.47 | 352.94 | 1411.76 |
| 175 | 85.71 | 171.43 | 342.86 | 1371.43 |
| 180 | 83.33 | 166.67 | 333.33 | 1333.33 |
| 190 | 78.95 | 157.89 | 315.79 | 1263.16 |
| 200 | 75.00 | 150.00 | 300.00 | 1200.00 |
| 210 | 71.43 | 142.86 | 285.71 | 1142.86 |
| 220 | 68.18 | 136.36 | 272.73 | 1090.91 |

Values are rounded to two decimals.

## Worked example: how long is my track?

Say you write a track at 175 BPM and it is 32 bars long.

1. One bar at 175 BPM = 240000 / 175 = 1371.43 ms.
2. 32 bars = 32 x 1371.43 = 43,885.7 ms.
3. That is about 43.9 seconds.

You can check this a second way. 32 bars x 16 steps = 512 steps. One step at 175 BPM = 15000 / 175 = 85.71 ms. 512 x 85.71 = 43,885.7 ms. Same answer.

Longer tracks scale in a straight line: 64 bars at 175 BPM is about 87.8 seconds, and 128 bars is about 175.5 seconds.

## From milliseconds to audio frames

Digital audio is counted in frames. At a 44.1 kHz sample rate there are 44,100 frames per second.

Frames per 16th note = 44100 x 60 / BPM / 4

At 175 BPM that is 44100 x 60 / 175 / 4 = 3,780 frames per step. A tempo that divides evenly like this keeps steps on whole frames. At 170 BPM the result is 3,891.18 frames, so a sequencer has to track a fractional position to stay in time over a long loop.

## Which tempo for which style?

Tempo ranges are loose conventions. Genre names overlap and producers break the ranges all the time. As a rough guide:

- Hard techno often sits around 150 to 160 BPM.
- Gabber and hardcore often sit around 170 to 200 BPM.
- Speedcore goes higher still.

The chart above covers 140 to 220 BPM, the range of the app's tempo control.

## Tips for using the numbers

- To set a delay time that lands on the grid, use the 8th note or 16th note value from the chart. A dotted 8th is 1.5 x the 8th note value.
- A kick every beat at 175 BPM repeats every 342.86 ms. That is 175 kicks per minute.
- Faster tempo shortens each step. Samples that ring longer than a step will overlap with the next hit, so trim long kicks and bass tails as you raise the BPM.
- Tempo changes do not change pitch in a step sequencer. Only the spacing between triggers changes.

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/tekkno-rave-daw/bpm-to-ms-chart/

## Try it in the app

Tekkno Rave DAW is an Android groovebox for hard techno and hardcore. Its tempo control runs from 140 to 220 BPM, a pattern has 8, 16, 32 or 64 steps, and one step is one 16th note. In the song view, one bar is 16 steps, so the song length formula above is the one the app uses for playback.
