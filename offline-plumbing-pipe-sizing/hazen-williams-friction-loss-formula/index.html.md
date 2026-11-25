# Hazen-Williams Friction Loss Formula With Example

> The Hazen-Williams formula in psi per 100 ft for water pipe, C values for copper and PEX, and a worked example with velocity.

- Web: https://apps.schimpf.es/offline-plumbing-pipe-sizing/hazen-williams-friction-loss-formula/
- App: Pipe Sizing: IPC & UPC Water, https://apps.schimpf.es/offline-plumbing-pipe-sizing/index.md
Hazen-Williams is the standard way to estimate friction loss in water supply pipe. It is simple, it works in US units, and it is accurate enough for sizing cold and hot water lines. This page gives the formula, the C values used for copper and plastic, and a worked example you can follow with a calculator.

## The formula

For water in a full pipe, friction loss in psi per 100 feet of pipe is:

**psi per 100 ft = 100 × 4.52 × Q^1.852 / (C^1.852 × d^4.8704)**

Where:

- Q is the flow in gallons per minute (GPM).
- C is the Hazen-Williams roughness coefficient. A higher C means a smoother pipe.
- d is the actual inside diameter of the pipe in inches. The nominal size does not go in the formula.

The formula comes from the work of Williams and Hazen (*Hydraulic Tables*, 1905). The form above is the common US-unit version found in plumbing and fire protection references.

To get the loss over a run, scale by length:

**loss in psi = psi per 100 ft × length in ft / 100**

This is straight pipe only. Fittings, valves and meters add loss that this formula does not include.

## Velocity

Velocity matters as much as friction. Fast water causes noise and erosion, so most sizing starts from a velocity limit.

**velocity in fps = 0.4085 × Q / d²**

Q is in GPM and d is the inside diameter in inches.

## C values to use

Design values, lower than new-pipe best cases:

| Material | C |
|---|---|
| Copper (Types K, L, M) | 130 |
| PEX, PE-RT, CPVC, PEX-AL-PEX | 150 |

## Use the inside diameter

Nominal size is only a name. Copper tube is sized by nominal diameter, and the real inside diameter changes with the wall type. These are the inside diameters used on this page, from ASTM B88 (copper Type L) and ASTM F876 (PEX, SDR 9):

| Nominal size | Copper L ID (in) | PEX SDR 9 ID (in) |
|---|---|---|
| 1/2" | 0.545 | 0.475 |
| 3/4" | 0.785 | 0.671 |
| 1" | 1.025 | 0.862 |
| 1-1/4" | 1.265 | 1.054 |
| 1-1/2" | 1.505 | 1.244 |
| 2" | 1.985 | 1.629 |

Because friction depends on d to the power 4.87, a small change in inside diameter has a big effect. A PEX line is often one size larger than copper for the same flow.

## Worked example

A branch serves 10 water supply fixture units (WSFU) with flush tank fixtures. Using the Hunter curve, 10 WSFU is 14.6 GPM. The pipe is copper Type L (C = 130) and the cold water velocity limit is 8 fps. The run is 60 ft.

Step 1, check each size. Compute velocity with 0.4085 × 14.6 / d², which is 5.964 / d²:

| Size | ID (in) | Velocity (fps) | Friction (psi/100 ft) | Within 8 fps? |
|---|---|---|---|---|
| 1/2" | 0.545 | 20.1 | 152 | No |
| 3/4" | 0.785 | 9.68 | 25.6 | No |
| 1" | 1.025 | 5.68 | 6.99 | Yes |

Step 2, pick the smallest size within the limit. That is 1".

Step 3, work out the 1" friction loss by hand.

1. 14.6^1.852 = 143.3
2. 130^1.852 = 8,223
3. 1.025^4.8704 = 1.128
4. psi per 100 ft = 100 × 4.52 × 143.3 / (8,223 × 1.128) = 64,785 / 9,274 = 6.99

Step 4, scale to 60 ft. 6.99 × 60 / 100 = 4.19 psi of loss through the straight run.

The same flow in 3/4" copper would lose 25.6 psi per 100 ft and run at nearly 10 fps. That is why the velocity check comes first.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumbing-pipe-sizing/hazen-williams-friction-loss-formula/

The calculator uses the formulas and inside diameters above. Results are computed values and may differ slightly from printed tables.

## What this does not cover

- Fittings and valves. Add their loss separately.
- Elevation change and street pressure.
- Water other than normal potable water at ordinary temperatures.

Check the adopted plumbing code and your local authority for sizing rules and minimum sizes. For example, the IPC (2024 edition) addresses water pipe sizing in section 604.3 and Appendix E, and the UPC (2024 edition) in section 610.1 and Appendix A.

## Do it on site

The Offline Plumbing Pipe Sizing app for Android runs this calculation for every size from 1/2" to 4" at once. Enter WSFU or GPM, pick a material and it shows the recommended size, velocity and psi per 100 ft in one table. With a segment length it adds the total straight-pipe loss. It works without a connection and cites the IPC or UPC section for the edition you pick (2024 or 2021). Copper L and PEX are ready to use from the first launch.

## Sources

- Williams, G. S. and Hazen, A., *Hydraulic Tables*, 1905.
- ASTM B88, Standard Specification for Seamless Copper Water Tube (inside diameters, Type L).
- ASTM F876, Standard Specification for Crosslinked Polyethylene (PEX) Tubing (SDR 9 inside diameters).
- International Plumbing Code (ICC), 2024 edition, section 604.3 and Appendix E.
- Uniform Plumbing Code (IAPMO), 2024 edition, section 610.1 and Appendix A.
