# AWG to mm² Chart: Wire Size, Area and Resistance

> Convert AWG to mm² with a chart of area, nearest metric size and copper resistance, plus the formula and a worked example.

- Web: https://apps.schimpf.es/offline-wire-gauge-calculator/awg-to-mm2-chart/
- App: Wire Gauge Calculator: NEC, https://apps.schimpf.es/offline-wire-gauge-calculator/index.md
An AWG size is a position on a scale. The larger the number, the thinner the wire. This page gives a conversion chart from 18 AWG to 250 kcmil, the formula behind it, and a small calculator for any size.

## AWG to mm² chart (copper)

The "next metric size" column is the smallest standard metric cross-section that is at least as large as the AWG wire. It matches sizes only and does not size a circuit.

| AWG | Area (mm²) | Next metric size (mm²) | Ω/km | Ω/1000 ft |
|---|---|---|---|---|
| 18 | 0.823 | 1 | 20.9 | 6.39 |
| 16 | 1.31 | 1.5 | 13.2 | 4.01 |
| 14 | 2.08 | 2.5 | 8.29 | 2.53 |
| 12 | 3.31 | 4 | 5.21 | 1.59 |
| 10 | 5.26 | 6 | 3.28 | 0.999 |
| 8 | 8.37 | 10 | 2.06 | 0.628 |
| 6 | 13.3 | 16 | 1.30 | 0.395 |
| 4 | 21.2 | 25 | 0.815 | 0.248 |
| 2 | 33.6 | 35 | 0.513 | 0.156 |
| 1/0 | 53.5 | 70 | 0.322 | 0.0983 |
| 2/0 | 67.4 | 70 | 0.256 | 0.0779 |
| 3/0 | 85.0 | 95 | 0.203 | 0.0618 |
| 4/0 | 107 | 120 | 0.161 | 0.0490 |
| 250 kcmil | 127 | 150 | 0.136 | 0.0415 |

Resistance is for a solid copper conductor at 20 °C. Aluminum has about 1.64 times the resistance of copper at the same size, because its conductivity is 61 % of copper's.

## How AWG works

Each step down in AWG number makes the wire thicker. Every 6 steps roughly halves the diameter, and every 3 steps roughly doubles the area. That gives some quick mental checks:

- 10 AWG is about 5.3 mm². Three steps thicker (7 AWG) would be about 10.6 mm², twice the area.
- Going from 12 AWG to 6 AWG roughly quadruples the area (3.31 to 13.3 mm²).
- Sizes above 4/0 are given in kcmil. One kcmil is 0.5067 mm².

## The formula

The AWG diameter is defined by a geometric progression between 36 AWG and 0000 (4/0) AWG. Standard ASTM B258, *Standard Specification for Standard Nominal Diameters and Cross-Sectional Areas of AWG Sizes of Solid Round Wires Used as Electrical Conductors*, uses it.

1. Diameter in mm: d = 0.127 × 92^((36 − n) / 39), where n is the gauge number. Use n = 0 for 1/0, −1 for 2/0, −2 for 3/0 and −3 for 4/0.
2. Area in mm²: A = π / 4 × d².
3. For kcmil sizes: A = kcmil × 0.5067.
4. Resistance in Ω/km: ρ / A × 1000, with ρ = 1/58 Ω·mm²/m for annealed copper (100 % IACS, the International Annealed Copper Standard) and ρ = (1/58) / 0.61 for aluminum (61 % IACS).
5. Ω per 1000 ft = Ω/km × 0.3048.

### Worked example: 10 AWG copper

1. n = 10, so d = 0.127 × 92^(26 / 39) = 0.127 × 92^0.6667 = 0.127 × 20.38 = 2.588 mm.
2. A = π / 4 × 2.588² = 5.26 mm².
3. Resistance = (1 / 58) / 5.26 × 1000 = 3.28 Ω/km.
4. In feet: 3.28 × 0.3048 = 0.999 Ω per 1000 ft.
5. The smallest metric size at or above 5.26 mm² is 6 mm².

## Metric sizes

The "next metric size" column uses the nominal cross-sections of IEC 60228, *Conductors of insulated cables*. They run 0.5, 0.75, 1, 1.5, 2.5, 4, 6, 10, 16, 25, 35, 50, 70, 95, 120, 150, 185, 240, 300, 400, 500, 630, 800 and 1000 mm². AWG and metric sizes rarely match exactly, so a wire swap usually means rounding up to the next metric size. Check the current rating of the metric cable separately. Area alone does not give the ampacity, because insulation, installation method and ambient temperature all change it.

## Convert any size

An interactive calculator is on the web page: https://apps.schimpf.es/offline-wire-gauge-calculator/awg-to-mm2-chart/

## Limits of this chart

- The chart shows a solid conductor. Stranded conductors have the same nominal area but a slightly larger overall diameter and slightly higher resistance.
- Resistance is at 20 °C. Copper resistance rises about 0.39 % per °C, so a wire at 75 °C has about 22 % more resistance.
- NEC voltage-drop calculations use the resistance values in NFPA 70, Chapter 9, Table 8 (2023 edition), which are for a different temperature and for uncoated conductors. They differ slightly from the figures above. This page does not reproduce NEC tables.

## Use it in the app

Offline Wire Gauge Calculator has this table built in under Reference, for copper and aluminum, in mm² and Ω per km and per 1000 ft. It works without a signal. The same app also sizes wire by NEC ampacity, voltage drop and breaker rules. Each result shows which limit set the size and which NEC table and edition it comes from. Results are estimates; verify with local code and the authority having jurisdiction.
