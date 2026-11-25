# WSFU to GPM Conversion Chart (Hunter Curve)

> Convert water supply fixture units to gallons per minute with the Hunter curve. Flush tank and flushometer values, plus a worked example.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/wsfu-to-gpm-conversion-chart/
- App: Pipe Sizing: IPC & UPC Water, https://apps.schimpf.es/offline-plumbing-pipe-sizing/index.md
Water supply fixture units (WSFU) rate how much load a fixture puts on a supply pipe. To size pipe you need flow in gallons per minute (GPM). The Hunter curve links the two. This page shows a conversion chart, explains the two curves, and works one example by hand.

## What the Hunter curve is

Not every fixture runs at once. Roy B. Hunter used probability to estimate the peak flow a group of fixtures will really draw. His work, *Methods of Estimating Loads in Plumbing Systems* (National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940), is public domain and still the base for the demand tables in plumbing codes.

There are two curves:

- Flush tank, for systems where toilets use a tank. It gives a lower peak flow.
- Flushometer (flush valve), for systems where toilets use flush valves. It gives a higher peak flow, because a flush valve draws a lot of water fast.

Pick the curve by the type of toilet. A job with flush valves uses the flushometer curve for the whole segment.

## WSFU to GPM chart

Selected points from the curves. Values in between are found by straight-line interpolation.

| Total WSFU | Flush tank (GPM) | Flushometer (GPM) |
|---|---|---|
| 5 | 9.4 | 15.0 |
| 10 | 14.6 | 27.0 |
| 20 | 19.6 | 35.0 |
| 30 | 23.3 | 42.0 |
| 40 | 26.3 | 46.0 |
| 50 | 29.1 | 50.0 |
| 100 | 43.5 | 67.5 |
| 200 | 65.0 | 90.0 |
| 300 | 85.0 | 108.0 |
| 500 | 124.0 | 143.0 |
| 1,000 | 208.0 | 208.0 |

Notes on the ranges:

- The flush tank curve runs from 1 to 5,000 WSFU. At 1 WSFU it is 3.0 GPM, at 2 WSFU 5.0 GPM.
- The flushometer curve runs from 5 to 5,000 WSFU.
- The two curves meet at 1,000 WSFU and above. Large systems have so many fixtures that the toilet type no longer changes the peak.

## How to convert

1. Add up the WSFU of every fixture the pipe serves, using the fixture values from your adopted code.
2. Choose the flush tank or flushometer curve.
3. Find the two chart points on either side of your total.
4. Interpolate between them.

The interpolation is:

**GPM = GPM₁ + (WSFU − WSFU₁) / (WSFU₂ − WSFU₁) × (GPM₂ − GPM₁)**

## Worked example

A bathroom group on a flush tank system totals 22 WSFU.

1. The chart points on each side are 20 WSFU (19.6 GPM) and 25 WSFU (21.5 GPM).
2. The position between them is (22 − 20) / (25 − 20) = 0.4.
3. GPM = 19.6 + 0.4 × (21.5 − 19.6) = 19.6 + 0.76 = 20.36, which rounds to 20.4 GPM.

The same 22 WSFU on a flushometer system:

1. Points: 20 WSFU (35.0 GPM) and 25 WSFU (38.0 GPM).
2. GPM = 35.0 + 0.4 × (38.0 − 35.0) = 36.2 GPM.

The flushometer system needs nearly 16 GPM more for the same fixture units.

## What to do with the GPM

Flow alone does not give a pipe size. Next you compare velocity for each pipe size against a limit, and look at friction loss. See the Hazen-Williams page on this site for the formulas.

For example, 20.4 GPM in Type L copper (inside diameter 1.025 in for 1") gives a velocity of 0.4085 × 20.4 / 1.025² = 7.9 fps. That is just inside an 8 fps cold water limit, so 1" works. At 36.2 GPM the same pipe would run at 14.1 fps, and you would need 1-1/2" (6.5 fps).

## Limits of the method

- The Hunter curve gives a peak estimate for ordinary fixture mixes. Continuous loads such as irrigation or process water are added separately.
- Modern low-flow fixtures often draw less than the curve predicts. Codes still use the curve, so follow the adopted code.
- Your adopted code decides which fixture values and which edition apply. The IPC (2024 edition) covers demand in Appendix E, section E103.3. The UPC (2024 edition) covers it in Appendix A, section A 103.0.
- Printed code tables can differ slightly from curve values computed this way.

## Convert and size in the app

The Offline Plumbing Pipe Sizing app for Android does this conversion for you. Enter the total WSFU, set flush tank or flushometer once, and it converts to GPM with the Hunter curve. It then shows the recommended pipe size, the velocity and the friction loss in psi per 100 ft for every size from 1/2" to 4". It works without a connection and shows the IPC or UPC section for the edition you choose.

## Sources

- Hunter, R. B., *Methods of Estimating Loads in Plumbing Systems*, National Bureau of Standards, Building Materials and Structures Report BMS 65, 1940.
- International Plumbing Code (ICC), 2024 edition, Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, Appendix A.
