# Scale Intervals Chart for Minor, Phrygian, Harmonic Minor

> Semitone intervals for minor, major, phrygian, harmonic minor and minor pentatonic scales, plus the pitch ratio of every semitone.

- Web: https://apps.schimpf.es/tekkno-rave-daw/scale-intervals-chart/
- App: Tekkno Rave DAW: Beat Maker, https://apps.schimpf.es/tekkno-rave-daw/index.md
Dark hard techno leads and acid stabs usually sit in a minor or phrygian scale. This page lists the semitone intervals of five common scales, shows how to spell them from any root note, and gives the pitch ratio of each semitone so you can see what happens when a sample is transposed.

## Scale interval chart

Numbers are semitones above the root note. The root is 0 and the octave is 12.

| Scale | Semitones from the root | Notes |
|-------|-------------------------|-------|
| Minor (natural minor) | 0, 2, 3, 5, 7, 8, 10 | 7 |
| Major | 0, 2, 4, 5, 7, 9, 11 | 7 |
| Phrygian | 0, 1, 3, 5, 7, 8, 10 | 7 |
| Harmonic minor | 0, 2, 3, 5, 7, 8, 11 | 7 |
| Minor pentatonic | 0, 3, 5, 7, 10 | 5 |

These interval patterns are standard Western music theory. For a textbook treatment, see Kostka and Payne, *Tonal Harmony* (McGraw-Hill, 8th edition, 2017).

## What makes each scale sound the way it does

- Minor has a flat third (3 semitones), which gives the dark, serious feel common in techno.
- Phrygian is minor with a flat second (1 semitone). That close step above the root gives the tense, aggressive sound heard in many hardcore and gabber leads.
- Harmonic minor is minor with a raised seventh (11 semitones). The gap between the 6th and 7th notes gives a dramatic, eastern-sounding lift.
- Major is brighter and used less in hard styles, but works for euphoric hardcore melodies.
- Minor pentatonic drops the 2nd and 6th notes. With only five notes, almost nothing sounds wrong, so it suits riffs.

## How to spell a scale from any root

1. Number the 12 notes from the root: C = 0, C sharp = 1, D = 2, D sharp = 3, E = 4, F = 5, F sharp = 6, G = 7, G sharp = 8, A = 9, A sharp = 10, B = 11.
2. Add the root number to each interval from the chart.
3. If the total is 12 or more, subtract 12.
4. Convert the numbers back to note names.

### Worked example: F phrygian

F is 5. Phrygian is 0, 1, 3, 5, 7, 8, 10.

- 5 + 0 = 5, F
- 5 + 1 = 6, F sharp (G flat)
- 5 + 3 = 8, G sharp (A flat)
- 5 + 5 = 10, A sharp (B flat)
- 5 + 7 = 12, which is 0, C
- 5 + 8 = 13, which is 1, C sharp (D flat)
- 5 + 10 = 15, which is 3, D sharp (E flat)

F phrygian is F, G flat, A flat, B flat, C, D flat, E flat.

## Pitch ratio of each semitone

Transposing a sample by resampling changes its playback speed. In 12-tone equal temperament, each semitone multiplies the frequency by the twelfth root of 2:

ratio = 2^(semitones / 12)

| Semitones | Ratio |
|-----------|-------|
| 0 | 1.0000 |
| 1 | 1.0595 |
| 2 | 1.1225 |
| 3 | 1.1892 |
| 4 | 1.2599 |
| 5 | 1.3348 |
| 6 | 1.4142 |
| 7 | 1.4983 |
| 8 | 1.5874 |
| 9 | 1.6818 |
| 10 | 1.7818 |
| 11 | 1.8877 |
| 12 | 2.0000 |

Negative values go down: -12 semitones gives a ratio of 0.5, half speed and one octave lower. Resampling also changes the length of the sample. A sample played at ratio 2 lasts half as long.

## Worked example: a grid row in A minor

Tekkno Rave DAW maps grid rows to pitch with this rule. Row 0 is the lowest row, and a higher row is a higher pitch. With scale snap on, each row is the next scale degree, so every row is in key. Samples are tuned to C3, which is MIDI note 48, and semitone 0 means C3.

For a scale with n notes:

semitones = root + 12 x octave shift + 12 x (row div n) + interval[row mod n]

Take A minor (root 9, 7 notes), octave shift 0, and row 9:

1. 9 div 7 = 1, so the pattern has gone up one octave: 12 x 1 = 12.
2. 9 mod 7 = 2, and the third interval of minor (index 2) is 3.
3. Total = 9 + 0 + 12 + 3 = 24 semitones.
4. Ratio = 2^(24 / 12) = 4.0.
5. The note is MIDI 48 + 24 = 72, which is C5.

Check by counting A minor degrees up from row 0: A, B, C, D, E, F, G, A, B, C. Row 9 is the tenth note, C. It matches.

With snap off, rows are plain semitones (semitones = root + 12 x octave shift + row) and in-scale rows are only tinted.

## Try it in the app

Tekkno Rave DAW has a pattern grid with 12 rows, 8, 16, 32 or 64 steps, and an octave shift of -2 to +2. Choose minor, major, phrygian, harmonic minor or minor pentatonic with any root note, switch on snap, and every row stays in key. Open a pattern and paint notes to hear the scales from this chart.
