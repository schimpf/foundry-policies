# 12V Wire Size and Voltage Drop Formula, With Example

> How to pick wire gauge for a 12V or 24V run: the voltage drop formula, a worked example, and the maximum length for each wire size.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/12v-wire-size-voltage-drop/
- App: Wire Gauge Calculator: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/index.md
On a 12 V circuit, a small voltage loss is a big share of the supply. A 0.6 V drop is 5 % at 12 V but only 0.25 % at 240 V. That is why 12 V and 24 V runs are usually sized by voltage drop first and checked for ampacity afterward. This page shows the formula, a worked example and a table of maximum lengths.

## The DC voltage drop formula

Current flows out on one conductor and back on the other, so the resistance that counts is that of twice the one-way length.

1. Drop in volts: drop = 2 × L × I × R
2. Drop in percent: drop / supply volts × 100
3. Allowed drop in volts: target % / 100 × supply volts
4. Maximum one-way length: L max = allowed drop / (2 × I × R)

Here L is the one-way length in feet, I is the current in amps and R is the wire resistance in ohms per foot (the chart value per 1000 ft divided by 1000). For DC, watts divided by volts gives amps.

A common target is 3 % for a branch circuit. NFPA 70 (the NEC), 2023 edition, suggests 3 % for a branch circuit and 5 % for feeder plus branch combined, in informational notes in Articles 210 and 215. They are informational notes and carry no requirement. Your own target can be stricter, for example for sensitive electronics or LED lighting.

## Copper resistance used in the examples

These values are for solid copper at 20 °C, computed from the public AWG diameter formula and annealed copper resistivity. See the [AWG to mm² chart](awg-to-mm2-chart) for how they are derived.

| AWG | Ω per 1000 ft |
|---|---|
| 12 | 1.59 |
| 10 | 0.999 |
| 8 | 0.628 |
| 6 | 0.395 |
| 4 | 0.248 |

## Worked example: a 240 W load, 15 ft from the battery

A 12 V load draws 240 W. The run is 15 ft one way. Copper wire, 3 % target.

1. Current: 240 W / 12 V = 20 A.
2. Allowed drop: 3 % × 12 V = 0.36 V.
3. Round-trip length: 2 × 15 ft = 30 ft. Multiply by the current: 30 × 20 = 600 ft·A.
4. Try each size:

| AWG | Drop (V) | Drop (%) | Within 3 %? |
|---|---|---|---|
| 12 | 0.953 | 7.9 | No |
| 10 | 0.599 | 5.0 | No |
| 8 | 0.377 | 3.1 | No, just over |
| 6 | 0.237 | 2.0 | Yes |
| 4 | 0.149 | 1.2 | Yes |

5. The smallest size that passes is 6 AWG. Drop for 6 AWG: 600 × 0.000395 = 0.237 V, or 1.98 %.

8 AWG drops 3.14 % and fails the 3 % target, so check each size before you round.

## Maximum one-way length at 20 A, 12 V, 3 %

This uses L max = 0.36 / (2 × 20 × R).

| AWG | Max length (ft) |
|---|---|
| 10 | 9.0 |
| 8 | 14.3 |
| 6 | 22.8 |
| 4 | 36.3 |

Doubling the voltage to 24 V doubles the allowed drop in volts. The same load takes half the current, so the maximum length is four times as long for the same wire.

## Ampacity still applies

Voltage drop is only one limit. The wire also has to carry the current, and the breaker has to protect the wire. For continuous loads the NEC requires the circuit to be sized for 125 % of the load (NFPA 70, 2023 edition, 210.19(A)(1) and 215.2(A)(1)). A voltage-drop pass does not replace the ampacity check. The larger of the two sizes wins.

## AC circuits

On AC, the formula uses impedance instead of plain resistance:

- Effective ohms per foot: R × cos θ + X × sin θ, where cos θ is the power factor, R is resistance and X is reactance.
- Single-phase: the factor 2 stays.
- Three-phase: the factor 2 becomes √3 (1.732).

The NEC lists R and X in Chapter 9, Table 9. Table 8 holds the DC resistance values. The values in the tables above are the public-formula figures at 20 °C, so they differ slightly from the NEC tables, and results can differ by a size at the edge.

## Use it in the app

Offline Wire Gauge Calculator does this sum for you without a signal. Enter amps, or watts and volts, the length and your target. It checks voltage drop, ampacity, the breaker rules and the terminal rating, then shows which of them set the size. It uses NEC Chapter 9 Table 8 for DC and Table 9 for AC, and it cites the table and edition in each result. The app also has two reverse modes: maximum length for a chosen wire, and maximum load for a chosen wire and length. DC presets cover 12 V and 24 V, and 18 AWG and 16 AWG are offered for DC.

Results are estimates. Verify with local code and the authority having jurisdiction.
