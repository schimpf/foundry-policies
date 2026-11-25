# Copper and PEX Pipe Size Chart by GPM and Velocity

> Maximum GPM for copper Type L and PEX pipe from 1/2 to 4 inch at 5 and 8 fps, with inside diameters and a worked sizing example.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/copper-and-pex-pipe-size-chart-gpm/
- App: Pipe Sizing: IPC & UPC Water, https://apps.schimpf.es/offline-plumbing-pipe-sizing/index.md
A 3/4" copper Type L line carries up to 12.07 GPM at 8 fps and 7.54 GPM at 5 fps. The maximum depends on the velocity limit you accept and on the real inside diameter of the pipe. This page gives a chart of maximum flow by pipe size for copper Type L and PEX, shows how the numbers are made, and sizes a line from a given flow.

## Why velocity sets the size

Most water supply sizing picks the smallest pipe that keeps velocity under a limit. Fast water makes noise and wears pipe, especially in hot lines. Two limits are common:

- 8 fps for cold water.
- 5 fps for hot water in copper.

The IPC does not state a velocity limit for these materials. These values come from guidance by manufacturers and the Copper Development Association (*Copper Tube Handbook*). The UPC (2024 and 2021 editions, Appendix A, section A 105.1) gives 8 fps for cold water. Your local authority decides what applies, so confirm before you rely on any limit.

## The formula behind the chart

Rearrange the velocity equation to find the flow a pipe carries at a given velocity:

**GPM = velocity in fps × d² / 0.4085**

Here d is the inside diameter in inches. At 8 fps, GPM = 19.58 × d². At 5 fps, GPM = 12.24 × d².

## Inside diameters

Inside diameters come from ASTM B88 (copper Type L) and ASTM F876 (PEX, SDR 9). Nominal size is only a label.

## Maximum GPM, copper Type L

| Nominal size | ID (in) | Max GPM at 8 fps (cold) | Max GPM at 5 fps (hot) |
|---|---|---|---|
| 1/2" | 0.545 | 5.82 | 3.64 |
| 3/4" | 0.785 | 12.07 | 7.54 |
| 1" | 1.025 | 20.58 | 12.86 |
| 1-1/4" | 1.265 | 31.34 | 19.59 |
| 1-1/2" | 1.505 | 44.36 | 27.72 |
| 2" | 1.985 | 77.17 | 48.23 |
| 2-1/2" | 2.465 | 119.0 | 74.37 |
| 3" | 2.945 | 169.9 | 106.2 |
| 4" | 3.905 | 298.6 | 186.6 |

## Maximum GPM, PEX (SDR 9)

PEX is not limited to 5 fps for hot water in the guidance used here, so one column at 8 fps covers both.

| Nominal size | ID (in) | Max GPM at 8 fps |
|---|---|---|
| 1/2" | 0.475 | 4.42 |
| 3/4" | 0.671 | 8.82 |
| 1" | 0.862 | 14.55 |
| 1-1/4" | 1.054 | 21.76 |
| 1-1/2" | 1.244 | 30.31 |
| 2" | 1.629 | 51.97 |
| 2-1/2" | 2.011 | 79.20 |
| 3" | 2.400 | 112.8 |
| 4" | 3.162 | 195.8 |

Compare the two tables. At the same nominal size PEX carries less, because its walls are thicker and its inside diameter is smaller. A 1" PEX line carries about 14.5 GPM at 8 fps, while 1" copper L carries about 20.6.

## How to use the chart

1. Find your design flow in GPM. If you have fixture units, convert them with the Hunter curve (see the WSFU to GPM page on this site).
2. Pick the material and the velocity limit.
3. Read down the column to the first size whose maximum GPM is at or above your flow.

## Worked example

A hot water line must carry 14.6 GPM in Type L copper, using the 5 fps hot water limit.

1. 3/4" maxes out at 7.54 GPM, which is too small.
2. 1" maxes out at 12.86 GPM, which is still too small.
3. 1-1/4" maxes out at 19.59 GPM. This is the first size that fits.

Check the velocity: 0.4085 × 14.6 / 1.265² = 3.7 fps. The same flow on a cold line at 8 fps would fit in 1" (5.7 fps).

## Check friction loss too

Velocity is only part of the check, because long runs lose pressure. Hazen-Williams friction loss for the cold example above (14.6 GPM, 1" copper L, C = 130) is about 6.99 psi per 100 ft. Over a 60 ft run that is about 4.2 psi. The Hazen-Williams page on this site shows the full calculation.

## Limits of this chart

- Values are computed and may differ slightly from printed tables.
- Code minimum sizes still apply. For example, the IPC 2024 sets a 3/4" minimum for a water service (section 603.1) and the UPC 2024 sets 3/4" for the building supply (section 610.8). A chart result of 1/2" does not override that.
- Fittings, meters, elevation and street pressure are not part of this chart.

## Use the app instead of the chart

The Offline Plumbing Pipe Sizing app for Android builds this table for your exact flow. Enter GPM or WSFU, choose IPC or UPC and the 2024 or 2021 edition, and pick a material. It marks the smallest size within the velocity limit and lists velocity and psi per 100 ft for every size from 1/2" to 4". You can change the velocity limit and reset it to the default. It works without a connection. Copper L and PEX are available from the first launch. Copper K and M, CPVC, PEX-AL-PEX and PE-RT, plus saved jobs, come with the one-time Pro purchase.

## Sources

- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- Copper Development Association, *Copper Tube Handbook* (velocity guidance for copper).
- International Plumbing Code (ICC), 2024 edition, section 603.1.
- Uniform Plumbing Code (IAPMO), 2024 edition, sections 610.8 and Appendix A, A 105.1.
