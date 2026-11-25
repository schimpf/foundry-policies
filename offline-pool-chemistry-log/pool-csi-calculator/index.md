# Pool CSI Calculator: Saturation Index Explained

> Calculate the calcite saturation index (CSI) of your pool water with the full formula, a worked example, and what to change when it is off.

- Web: https://apps.schimpf.es/offline-pool-chemistry-log/pool-csi-calculator/
- App: Pool Chem Log: Water Tests, https://apps.schimpf.es/offline-pool-chemistry-log/index.md
The calcite saturation index (CSI) tells you if your pool water tends to dissolve plaster and metal, or to leave scale behind. A CSI near zero means the water is balanced. This page gives you a calculator, the formula and a worked example.

## CSI calculator

An interactive calculator is on the web page: https://apps.schimpf.es/offline-pool-chemistry-log/pool-csi-calculator/

## How to read the result

- **Below -0.3:** corrosive. The water can etch plaster, damage grout and attack metal parts.
- **-0.3 to +0.3:** balanced. This is the range Pool Chem Log treats as the target.
- **Above +0.3:** scaling. Calcium can deposit on tiles, surfaces and in the salt cell or heater.

The -0.3 to +0.3 band is a practical target. Plaster pools gain the most from staying inside it.

## What goes into CSI

CSI uses these test results:

- pH
- Total alkalinity (TA), in ppm
- Calcium hardness (CH), in ppm
- Cyanuric acid (CYA), in ppm
- Borates, in ppm (optional)
- Salt, in ppm
- Water temperature

Warm water is more likely to scale, so temperature matters. Salt has a small effect through ionic strength. If you do not know your salt level, the calculator assumes 1,000 ppm, which is typical for fill water plus chlorine by-products. If you leave CYA or borates blank, they count as 0.

## The formula

The formula is the one used by Trouble Free Pool (TFP) and Pool Math, attributed to the chemist known as "chem geek".

CSI = pH - 6.9395 + log10(CH) + log10(carbonate alkalinity) - 2.56 x sqrt(I) / (1 + 1.65 x sqrt(I)) - 1412.5 / T

Where:

- **Carbonate alkalinity** = TA - 0.38772 x CYA / (1 + 10^(6.83 - pH)) - 4.63 x borates / (1 + 10^(9.11 - pH)). CYA and borates both count toward TA on a test kit, but they do not help the carbonate balance, so they are subtracted.
- **I (ionic strength)** = (1.5 x CH + TA) / 50045 + salt / 58440.
- **T** is the water temperature in kelvin: degrees C + 273.15.

If CH is 0 or carbonate alkalinity comes out at 0 or below, CSI cannot be calculated.

## Worked example

A plaster pool tests like this:

- pH 7.5
- TA 70 ppm
- CH 350 ppm
- CYA 40 ppm
- Borates 0
- Salt 1,000 ppm (assumed)
- Water 80 F, which is 26.67 C or 299.82 K

Step by step:

1. Carbonate alkalinity: 10^(6.83 - 7.5) = 0.2138, so CYA part = 0.38772 x 40 / 1.2138 = 12.78. Carbonate alkalinity = 70 - 12.78 = 57.22.
2. Ionic strength: (1.5 x 350 + 70) / 50045 + 1000 / 58440 = 0.01189 + 0.01711 = 0.02900. Its square root is 0.1703.
3. Ionic term: 2.56 x 0.1703 / (1 + 1.65 x 0.1703) = 0.4360 / 1.2810 = 0.3403.
4. Temperature term: 1412.5 / 299.82 = 4.7112.
5. Logs: log10(350) = 2.5441 and log10(57.22) = 1.7576.
6. Add up: 7.5 - 6.9395 + 2.5441 + 1.7576 - 0.3403 - 4.7112 = -0.19.

CSI is about -0.19. That is inside the balanced band, a little on the soft side.

## What to change when CSI is off

If CSI is too low (corrosive), raise one of these:

- **Calcium hardness:** the biggest lever for plaster pools. Calcium chloride raises it, but slowly, so add it in steps.
- **pH:** raising pH by 0.1 raises CSI by about 0.1.
- **Total alkalinity:** baking soda raises it.

If CSI is too high (scaling), lower pH with acid, or lower TA. Lowering calcium means replacing water, since no product removes it.

Calcium targets in Pool Chem Log depend on the surface:

| Surface | CH range (ppm) |
|---|---|
| Plaster or pebble | 250 to 650 |
| Vinyl or fiberglass | 50 to 350 |
| Acrylic | 150 to 250 (common range) |

The plaster, pebble, vinyl and fiberglass ranges follow TFP guidance. The acrylic range is a common industry range.

## Borates and salt

Borates are optional. Some owners keep 30 to 50 ppm as a pH buffer. If you use them, include them in the calculation, because borates raise the TA reading without helping the balance. Salt water pools should enter their real salt level.

## Limits

CSI is a model, and it depends on accurate tests, especially for TA, CH and pH. A small test error can move CSI by 0.1 or more. Retest before you change anything big, never mix chemicals, wear protection, and follow the product label.

## Track CSI over time

Pool Chem Log is an Android app that works offline. It calculates CSI from every test you enter, with borates and salt included, and it uses your temperature from the last test. It also shows your targets by surface type, calculates doses for calcium, alkalinity and pH, and keeps a history of all your tests. The formula in the app is the same as the one on this page.
