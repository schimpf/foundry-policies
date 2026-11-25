# Der Monarch feeding and harvest guide with formulas

> How much grain your people need in Der Monarch, how crops and soil set the harvest, and how feeding changes population. With worked examples.

- Web: https://apps.schimpf.es/der-monarch/der-monarch-feeding-and-harvest-guide/
- App: Der Monarch, https://apps.schimpf.es/der-monarch/index.md
How much grain you feed your people and what you plant decide most years in Der Monarch. This guide gives the formulas from the game and works through the starting position.

## How much grain people need

The need is 7 bushels per person, counting serfs, merchants, clergy and nobles.

**need = people × 7**

At the start you have 2,140 people, so the need is 2,140 × 7 = 14,980 bushels. You hold 18,000.

The feeding screen has a slider and quick buttons for 80 %, the need, and 125 %. Grain you set aside for feeding cannot be sold.

## What feeding does to the population

Let ratio = grain fed / need. The game forecasts the yearly change like this:

- **Births:** serfs × 3 % × the ratio, with the ratio capped at 1.2
- **Deaths:** people × 1.5 %
- **Starved:** if the ratio is below 1, people × (1 − ratio) × 25 %
- **Migration:** (ratio capped at 1.5 − 1) × people × 8 %, plus (30 − tax pressure) × people × 0.15 %, plus the justice mood × people

Tax pressure is (customs + income tax) / 2. Justice mood is +0.01 for Milde, 0 for Gerecht, −0.01 for Streng and −0.03 for Grausam. A positive migration result is immigrants, a negative one is people leaving.

### Worked example: three feeding levels

Start position: 1,820 serfs, 2,140 people, customs 20 %, income tax 25 %, justice Gerecht. Tax pressure is 22.5, so the tax part of migration is 7.5 × 2,140 × 0.0015 = 24.

| Fed | Ratio | Births | Deaths | Starved | Migration | Net change |
|---|---|---|---|---|---|---|
| 80 % (11,984) | 0.8 | 44 | 32 | 107 | −10 | **−105** |
| 100 % (14,980) | 1.0 | 55 | 32 | 0 | +24 | **+47** |
| 125 % (18,725) | 1.25 | 66 | 32 | 0 | +67 | **+101** |

Feeding 125 % needs 18,725 bushels, more than the 18,000 you hold, so at the start you cannot reach it without buying grain. The slider stops at the grain you hold. At year end, the grain fed is capped by the grain you hold after rats plus the harvest.

Feeding above 120 % no longer adds births, but it keeps raising migration up to 150 %.

## What you plant

You split your land between potatoes, grain and oats. The rest lies fallow. Each crop is rolled once a year between a low and a high yield per Morgen.

| Crop | Yield per Morgen | Risk | Soil drain |
|---|---|---|---|
| Kartoffeln (potatoes) | 2.6–3.5 | low | 8 |
| Korn (grain) | 1.8–5.2 | high | 6 |
| Hafer (oats) | 2.5–2.7 | none | 3 |

Soil strength runs from 40 to 100 %. Every yield is multiplied by soil / 100. Difficulty bends the roll: Milde gives better years, Hart gives worse ones and a higher rat loss.

### Serfs limit your fields

Each serf can work at most 6 Morgen. If you want more land sown than serfs × 6, every crop is scaled down. With 1,820 serfs you can work 10,920 Morgen.

### Worked example: the default plan

Land 10,000 Morgen, plan 40 % potatoes, 35 % grain, 15 % oats, 10 % fallow, soil 100 %.

1. Sown: 4,000 potatoes, 3,500 grain, 1,500 oats. Total 9,000 Morgen, under the serf limit of 10,920.
2. Lowest harvest: 4,000 × 2.6 + 3,500 × 1.8 + 1,500 × 2.5 = 10,400 + 6,300 + 3,750 = 20,450 bushels
3. Highest harvest: 4,000 × 3.5 + 3,500 × 5.2 + 1,500 × 2.7 = 14,000 + 18,200 + 4,050 = 36,250 bushels
4. Your need is 14,980, so even the worst year feeds everyone, before rats.

Rats then eat a share of the grain you hold, up to 5 % on Milde, 10 % on Normal and 16 % on Hart.

## Soil

Each year the soil changes by:

**fallow % × 0.6 − Σ(crop % × drain / 100)**, rounded

For the default plan: drain = 0.40 × 8 + 0.35 × 6 + 0.15 × 3 = 5.75. Fallow gives 10 × 0.6 = 6. The change is +0.25, which rounds to 0, so the soil stays at 100.

If you plant everything (0 % fallow) with potatoes at 100 %, the soil falls by 8 points a year. After 5 years the soil is at 60 and every yield is 40 % lower. Soil never goes below 40.

## Tips

- Oats are the safe crop. Grain yields anywhere from 1.8 to 5.2 per Morgen.
- Keep some fallow land if you farm hard. Fallow gives back 0.6 soil points per percent.
- Grain also sells. A good harvest turns into Taler for buildings. See the [rank requirements](der-monarch-rank-requirements).
- War costs harvest. Each company you send cuts your harvest by 2 %.

## Play it

Der Monarch is an Android game for one to four players on one device. All in-game text is in German. Open the Volk ernähren and Felder bestellen screens to try these numbers.
