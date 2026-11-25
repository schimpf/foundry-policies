# Binaural Beat Frequency Calculator and Formula

> Work out the left and right tone for any binaural beat with one formula, a worked example and a small calculator. Includes how a beat glides over time.

- Web: https://apps.schimpf.es/binaural-beats/binaural-beat-frequency-calculator/
- App: Binaural Beats, https://apps.schimpf.es/binaural-beats/index.md
A binaural beat is made from two pure tones, one per ear. The beat you perceive is the difference between them. This page gives the formula, a worked example and a calculator, then shows how to glide a beat from one rate to another.

## The binaural beat formula

- Left ear tone = carrier frequency
- Right ear tone = carrier frequency + beat frequency
- Beat frequency = right tone − left tone

All values are in hertz (Hz). The carrier is the base tone you actually hear. The beat is the slow pulse you perceive from the difference.

This is the layout the Binaural Beats app uses: left is the carrier and right is the carrier plus the beat.

## Worked example

You want a 10 Hz beat on a 400 Hz carrier.

1. Left ear: 400 Hz.
2. Right ear: 400 + 10 = 410 Hz.
3. Check: 410 − 400 = 10 Hz, so you perceive 10 beats per second.

At 10 Hz the beat falls in the alpha range (8 to below 12 Hz). The app's default preset, Calm Focus, uses exactly these numbers.

Another example: a 4 Hz beat on a 250 Hz carrier gives 250 Hz on the left and 254 Hz on the right. Four Hz is theta (4 to below 8 Hz).

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/binaural-beats/binaural-beat-frequency-calculator/

## Choosing the numbers

### Carrier frequency

Binaural beats are usually made with carriers below about 1000 Hz. The app accepts 100 to 1000 Hz and suggests 200 to 500 Hz as a comfortable range. Lower carriers sound deeper, higher carriers sound brighter. The carrier sets the tone you hear and leaves the beat rate unchanged.

### Beat frequency

The app accepts 0.25 to 45 Hz. Binaural beats become hard to perceive above about 30 Hz, so for rates above that the app suggests a monaural or isochronic beat instead.

| Beat (Hz) | Band |
|---|---|
| below 4 | Delta |
| 4 to below 8 | Theta |
| 8 to below 12 | Alpha |
| 12 to below 30 | Beta |
| 30 and above | Gamma |

### Headphones

A binaural beat only exists when each ear hears its own tone. Use stereo headphones or earbuds. On speakers the two tones mix in the air, and you hear a monaural beat instead. That is a different effect but also a real pulse.

## Other beat types, same beat rate

The beat rate means the same in all four modes:

- **Monaural:** both tones, carrier and carrier plus beat, are added and played to both ears. The pulse is in the sound.
- **Isochronic:** one tone at the carrier, switched on and off at the beat rate.
- **Bilateral:** one tone at the carrier that alternates between ears once per beat cycle.

For isochronic and bilateral beats the pulse can be a smooth sine shape or a soft square shape with sharper edges.

## Gliding a beat over time

A session made of steps can change the beat gradually. The app glides the rate on a geometric scale, so each equal slice of time multiplies the rate by the same factor.

Formula: beat at time t = start × (end ÷ start)^t, where t runs from 0 to 1 across the step.

Worked example: a step glides from 12 Hz to 6 Hz.

1. At the halfway point, t = 0.5.
2. The ratio end ÷ start = 6 ÷ 12 = 0.5.
3. 0.5 raised to the power 0.5 is about 0.707.
4. Beat = 12 × 0.707 ≈ 8.49 Hz.

A plain straight-line glide would give 9 Hz at the halfway point. The geometric version spends equal time on each doubling or halving, so 12 to 6 Hz takes as long as 6 to 3 Hz. This matches how pitch and rate are perceived, and it is why the beat slider in the app is logarithmic as well.

If both ends of a step are equal, the beat is held. After the last step, the final values hold until the session ends.

## What the research says

Evidence that binaural beats change mood, focus or sleep is mixed. The 2019 meta-analysis by Garcia-Argibay, Santed and Reales ("Efficacy of binaural auditory beats in cognition, anxiety, and pain perception: a meta-analysis", Psychological Research) found small to moderate effects, with large differences between studies. Treat beats as a relaxation aid. Keep the volume low and do not listen while driving. Ask your doctor first if you have epilepsy, a pacemaker or another medical condition.

## Make it in the app

Binaural Beats for Android generates these tones live, so you can try any carrier and beat from the examples above.

1. Pick binaural mode, set the carrier and beat, and read the band label.
2. Add optional white, pink or brown noise at its own volume.
3. Start a session of 5 to 90 minutes, or build a session from steps and watch the beat on a chart.

It plays in the background with lock-screen controls and works offline. You can also save a session as a WAV file.
