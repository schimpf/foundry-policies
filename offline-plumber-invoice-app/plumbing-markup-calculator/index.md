# Plumbing Markup Calculator and Formula

> Work out the sell price of pipe, fittings and parts from your cost and markup %, and see the margin it gives. Formula, worked example and table.

- Web: https://apps.schimpf.es/offline-plumber-invoice-app/plumbing-markup-calculator/
- App: Plumber Invoice & Quote Maker, https://apps.schimpf.es/offline-plumber-invoice-app/index.md
## Markup formula for plumbing parts

Markup is the percentage you add on top of what a part costs you. The sell price is:

**sell price = cost × (1 + markup ÷ 100)**

A 35% markup on a part that costs $42.50 gives $42.50 × 1.35 = $57.375, which rounds to $57.38. Your profit on the part is about $14.88.

Round half up to the nearest cent. 57.375 becomes 57.38, and 57.374 becomes 57.37.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumber-invoice-app/plumbing-markup-calculator/

## Markup and margin are different numbers

Markup is measured against your cost. Margin is measured against the sell price. The same sale gives two different percentages.

- Markup = profit ÷ cost
- Margin = profit ÷ sell price

With a $100 cost and a 30% markup, the sell price is $130 and the profit is $30. The markup is 30%. The margin is $30 ÷ $130 = 23.1%.

This matters when a supplier, an accountant or a business book talks about "margin". If you want a 30% margin, a 30% markup is too low. Use this instead:

**markup = margin ÷ (1 − margin)**

For a 30% margin that is 0.30 ÷ 0.70 = 42.9% markup.

## Markup to margin table

All rows use a $100 cost.

| Markup | Sell price | Profit | Margin |
|--------|-----------|--------|--------|
| 10% | $110.00 | $10.00 | 9.1% |
| 20% | $120.00 | $20.00 | 16.7% |
| 30% | $130.00 | $30.00 | 23.1% |
| 40% | $140.00 | $40.00 | 28.6% |
| 50% | $150.00 | $50.00 | 33.3% |
| 75% | $175.00 | $75.00 | 42.9% |
| 100% | $200.00 | $100.00 | 50.0% |

Margin never reaches 100%, however high the markup goes.

## Worked example: a water heater swap

Say you buy these parts for one job:

| Part | Qty | Cost each | Markup | Sell each | Line total |
|------|-----|-----------|--------|-----------|-----------|
| 50 gal water heater | 1 | $540.00 | 25% | $675.00 | $675.00 |
| Flex connector | 2 | $11.40 | 40% | $15.96 | $31.92 |
| Expansion tank | 1 | $38.75 | 40% | $54.25 | $54.25 |

The line total is the quantity times the sell price, rounded to the cent. Parts add up to $761.17 before tax and labor.

Different parts often carry different markups. Big, easy-to-compare items such as a water heater usually get a lower percentage than small fittings, because the customer can look up the big item online.

## What to include in the cost

Start with the price you pay the supplier. Then add the costs you carry for every part, or they eat your profit:

- The trip to the supply house, in your time or fuel
- Returns you eat when a part is wrong
- Warranty callbacks on parts you supplied

A small markup on a $3 fitting rarely covers a 40 minute trip. Many plumbers set a higher markup on small parts for that reason.

## How the app handles markup

Offline Plumber Invoice App has a price book with about 120 common plumbing items in eight categories: pipe, fittings, valves, water heaters, fixtures, drains, gas and labor. The items come without prices.

1. Open an item and enter your unit cost.
2. Enter a markup % for that item, or leave it empty to use the default markup from your business profile. The default starts at 0%.
3. The item shows the sell price, for example "Sell price $57.38 / each".
4. Add the item to a quote. The line takes the sell price, and you can still change the price on the line.

The app uses the formula above with whole cents and rounds half up. A markup can go up to 1000%. An item without a cost has no price, and the quote cannot be signed until every line has one.

Labor items are marked as labor and are not taxable by default. See [how a quote adds sales tax and a deposit](../plumbing-quote-sales-tax-and-deposit/) for what happens after the price is set.
