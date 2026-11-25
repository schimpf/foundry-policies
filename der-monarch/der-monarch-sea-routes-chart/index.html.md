# Der Monarch sea routes chart: cost, return and odds

> All 10 sea routes in Der Monarch with cost, years, chance of return and loot, plus the expected gain of each voyage.

- Web: https://apps.schimpf.es/der-monarch/der-monarch-sea-routes-chart/
- App: Der Monarch, https://apps.schimpf.es/der-monarch/index.md
In Der Monarch, ships are a way to turn Taler into more Taler, grain or settlers. They can also sink. This chart shows all ten sea routes and which ones pay best on average.

## How ships work

- Each year the game offers 3 of the 10 routes, picked at random.
- You can send one ship per route per year. The ship costs its route price at once.
- A ship comes back after 1 to 4 years, depending on the route. It shows up in your year report.
- On arrival it returns with the route's chance of return. If it does not, the ship and its cargo are lost. The price you paid is gone either way.
- Loot is rolled evenly between the minimum and maximum of the route.

## The chart

| Route | Cost | Years | Return chance | Gold | Grain (bushels) | Settlers |
|---|---|---|---|---|---|---|
| Nordsee (North Sea) | 600 | 1 | 95 % | none | 1,200–1,950 | none |
| Ostsee (Baltic) | 800 | 1 | 90 % | 200–400 | 1,100–2,100 | none |
| Archangelsk | 1,000 | 1 | 80 % | 800–1,200 | 800–1,400 | none |
| Mittelmeer (Mediterranean) | 1,200 | 1 | 85 % | 1,400–2,100 | none | none |
| Grönland (Greenland) | 1,200 | 2 | 60 % | 2,000–3,000 | none | none |
| Levante (Levant) | 1,500 | 2 | 75 % | 2,000–3,000 | none | none |
| Neue Welt (New World) | 2,000 | 2 | 70 % | 2,200–3,200 | 0–2,000 | 20–60 |
| Kapland (Cape) | 2,500 | 3 | 60 % | 4,000–5,300 | none | 30–80 |
| Ostindien (East Indies) | 3,500 | 3 | 50 % | 7,000–10,500 | none | none |
| China | 5,000 | 4 | 40 % | 12,500–18,750 | none | none |

## Expected value

The app rates a voyage by its average worth, counting the chance of losing the ship. It values one bushel of grain at 0.5 Taler and one settler at 10 Taler.

**expected value = return chance × (average gold + average grain × 0.5 + average settlers × 10)**

### Worked example: Neue Welt

1. Average gold: (2,200 + 3,200) / 2 = 2,700
2. Average grain: (0 + 2,000) / 2 = 1,000, worth 1,000 × 0.5 = 500
3. Average settlers: (20 + 60) / 2 = 40, worth 40 × 10 = 400
4. Sum: 2,700 + 500 + 400 = 3,600
5. Times 70 % return chance: 2,520 Taler
6. Minus the 2,000 Taler cost: +520 Taler on average

## Average gain per route

Gain is the expected value minus the cost. The last column divides it by the years at sea.

| Route | Expected value | Average gain | Gain per year at sea |
|---|---|---|---|
| Nordsee | 748 | +148 | +148 |
| Ostsee | 990 | +190 | +190 |
| Archangelsk | 1,240 | +240 | +240 |
| Mittelmeer | 1,488 | +288 | +288 |
| Grönland | 1,500 | +300 | +150 |
| Levante | 1,875 | +375 | +188 |
| Neue Welt | 2,520 | +520 | +260 |
| Kapland | 3,120 | +620 | +207 |
| Ostindien | 4,375 | +875 | +292 |
| China | 6,250 | +1,250 | +313 |

Values are rounded. The "gain per year" column is a rule of thumb that ignores that the cost is tied up while the ship is away.

## What the numbers mean

- Every route has a positive average gain, so on average a ship pays. One voyage can still lose everything.
- The long routes pay most per voyage but risk the most. China loses the ship six times in ten.
- Short routes with high return chances suit a small treasury. Nordsee returns 95 % of the time.
- Grain routes help in a bad harvest year. Nordsee and Ostsee mostly bring grain. See the [feeding and harvest guide](der-monarch-feeding-and-harvest-guide).
- Neue Welt and Kapland bring settlers, which add to your people count for the next rank. See the [rank requirements](der-monarch-rank-requirements).
- Only 3 routes are offered per year, so you pick the best of what you get.

## Timing

A ship sent in year Y on a 1-year route is settled at the end of year Y and appears in your report for year Y+1. A 3-year route sent in 1725 is reported in 1728. The game ends after 1760, so ships still at sea then bring nothing.

## Play it

Der Monarch is an Android game for one to four players on one device. All in-game text is in German. Open the app and try the Expeditionen screen in your next year.
