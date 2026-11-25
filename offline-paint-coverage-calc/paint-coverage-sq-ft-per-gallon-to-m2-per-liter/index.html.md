# Paint Coverage Converter: sq ft per Gallon to m² per Liter

> Convert paint coverage between sq ft per US gallon and m² per liter, with a table, the formula and a worked example for a room.

- Web: https://apps.schimpf.es/offline-paint-coverage-calc/paint-coverage-sq-ft-per-gallon-to-m2-per-liter/
- App: Paint Calc: Room Paint Amount, https://apps.schimpf.es/offline-paint-coverage-calc/index.md
Paint cans in the US print coverage in square feet per gallon. Most of the rest of the world prints square meters per liter. To convert, use the exact factors below. 350 sq ft per gallon is 8.59 m² per liter, and 10 m² per liter is 407 sq ft per gallon.

## The conversion

The app uses these exact constants:

- 1 ft = 0.3048 m, so 1 sq ft = 0.09290304 m²
- 1 US gallon = 3.785411784 L

### sq ft per gallon to m² per liter

m²/L = sq ft/gal × 0.09290304 ÷ 3.785411784

Or, close enough for a quick check: multiply by 0.02454.

### m² per liter to sq ft per gallon

sq ft/gal = m²/L × 3.785411784 ÷ 0.09290304

Or multiply by 40.746.

## Conversion table

| sq ft per gallon | m² per liter |
| --- | --- |
| 250 | 6.14 |
| 300 | 7.36 |
| 350 | 8.59 |
| 400 | 9.82 |

| m² per liter | sq ft per gallon |
| --- | --- |
| 8 | 326 |
| 10 | 407 |
| 12 | 489 |

## What coverage means

Coverage is how much surface one unit of paint covers in a single coat, on a normal, previously painted, smooth surface. It is printed on the can or the product data sheet. Real coverage drops on:

- Bare plaster, new drywall or wood, which soak up paint (primer helps)
- Rough or textured surfaces
- Strong color changes that need extra coats

The app handles texture with a factor: smooth 1.00, light texture 1.10, heavy texture 1.20. Primer has its own coverage setting, because primer cans often state a different figure than the topcoat.

## Worked example in both units

A room measures 4 × 5 m with 2.5 m walls. It has one door (0.9 × 2.1 m) and one window (1.0 × 1.2 m). You want two coats of smooth paint at 10 m² per liter with 10% waste.

1. Gross walls: 2 × (4 + 5) × 2.5 = 45 m²
2. Openings: 1.89 + 1.20 = 3.09 m²
3. Net walls: 41.91 m²
4. Paint: 41.91 × 2 ÷ 10 = 8.38 L
5. With waste: 8.38 × 1.10 = 9.22 L

The same paint sold in US gallons has a coverage of 407 sq ft per gallon, and the room is 451 sq ft of net wall. The result is the same volume: 451 × 2 ÷ 407 × 1.10 = 2.44 gal, which is 9.22 L.

### Round up to tins

Metric tins come in 5 L, 2.5 L, 1 L and 0.5 L. The app rounds up to the next half liter, so 9.22 L becomes 9.5 L. It then fills that with the largest tins first: one 5 L, one 2.5 L and two 1 L tins.

In gallons, the app rounds up to the next quart. 2.44 gal is 9.76 quarts, so 10 quarts: 2 gallons and 2 quarts. If the rounding ends on 3 quarts, you get one more gallon instead, since a gallon usually costs less than three quarts.

## Which unit to use

Switch the unit to match the can in your hand. The app starts with your device's locale and you can change it in settings. Internally it stores lengths in meters and converts for display, so a room entered in feet and one entered in meters give the same answer.

Allowed coverage values in the app range from 0.5 to 50 m² per liter. The app does not accept values outside that range.

## Skip the conversion

Offline Paint Coverage Calc for Android takes the coverage in whichever unit your can uses, converts it for you, and gives the answer in gallons and quarts or in liter tins. It works fully offline, with no account.

Results are estimates. Always check the coverage printed on your paint can.
