# Pizza Dough Baker's Percentage Calculator, Worked Example

> Turn baker's percentages into grams of flour, water, salt, oil, sugar and yeast for any dough weight. Formula, worked example and calculator.

- Web: https://apps.schimpf.es/pizza-calc/pizza-dough-baker-percentage-calculator/
- App: Pizza Calc: Dough Calculator, https://apps.schimpf.es/pizza-calc/index.md
Pizza recipes are often written in baker's percentages: every ingredient is a percent of the flour weight. It is the easiest way to scale a recipe up or down, and to compare styles. This page shows the formula, a worked example and a small calculator that turns percentages into grams.

## What baker's percentage means

Flour is always 100 %. Everything else is measured against the flour:

- Hydration 62 % means 62 g of water per 100 g of flour.
- Salt 2.2 % means 2.2 g of salt per 100 g of flour.
- The percentages add up to more than 100 %. That is normal.

See Jeffrey Hamelman, *Bread: A Baker's Book of Techniques and Recipes*, 2nd edition, 2012, for the standard description of the method.

## From percentages to grams

You know how much dough you want and the percentages. You need the flour weight first.

1. **Total dough weight** = number of balls × weight per ball × (1 + bowl loss ÷ 100).
2. **Sum of percentages** = hydration + salt + oil + sugar + yeast.
3. **Flour** = total dough weight ÷ (1 + sum of percentages ÷ 100).
4. **Each other ingredient** = flour × its percentage ÷ 100.

Bowl loss is the dough that sticks to the bowl and your hands. Adding about 2 % means you do not come up short.

For pans, the dough weight is pan area × thickness × number of pans. Thickness is in grams per cm². A rectangular pan of 40 × 30 cm at 0.6 g/cm² needs 40 × 30 × 0.6 = 720 g of dough.

## Worked example: two New York–style pizzas

Two balls of 340 g each, 2 % bowl loss. Percentages: hydration 62 %, salt 2.2 %, oil 2 %, sugar 1.5 %, yeast 0.2 %.

1. Total dough: 2 × 340 × 1.02 = **693.6 g**.
2. Sum of percentages: 62 + 2.2 + 2 + 1.5 + 0.2 = **67.9 %**.
3. Flour: 693.6 ÷ 1.679 = **413.1 g**.

| Ingredient | Percent | Grams |
|---|---|---|
| Flour | 100 | 413.1 |
| Water | 62 | 256.1 |
| Salt | 2.2 | 9.1 |
| Oil | 2 | 8.3 |
| Sugar | 1.5 | 6.2 |
| Yeast | 0.2 | 0.8 |
| **Total** | 167.9 | **693.6** |

The grams add up to the total dough weight, which is a good check.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/pizza-calc/pizza-dough-baker-percentage-calculator/

## Typical percentages by style

Starting values from Pizza Calc's style presets. Hydration ranges are the span the app treats as normal for the style.

| Style | Hydration | Salt | Oil | Sugar |
|---|---|---|---|---|
| Neapolitan | 60 % (58–65) | 2.8 % | 0 | 0 |
| New York | 62 % (58–65) | 2.2 % | 2 % | 1.5 % |
| Roman | 55 % (50–60) | 2.2 % | 4 % | 0.5 % |
| Detroit | 75 % (70–78) | 2.2 % | 1 % | 0 |
| Focaccia | 80 % (75–90) | 2.2 % | 4 % | 1 % |
| Deep dish | 50 % (45–55) | 1.8 % | 15 % | 2 % |

Use these as starting points. Flour strength changes how much water the dough takes.

## Common mistakes

- **Using total dough weight as 100 %.** Percentages always refer to the flour weight.
- **Forgetting yeast in the sum.** It is small but it is part of the total.
- **Mixing yeast types.** Fresh, active dry and instant yeast need different amounts for the same effect. State which one your percentage is for.
- **Ignoring preferments.** If part of the flour sits in a poolish or biga, the final dough holds less flour and water. The totals stay the same.

## Use it in Pizza Calc

Pizza Calc does these steps for you. Pick one of 16 styles or start blank, then set hydration, salt, oil and sugar with sliders. Choose dough balls or pans, and set bowl loss. The totals panel lists grams of flour, water, salt, yeast or starter, oil and sugar. With a poolish, biga or starter, it splits the dough into the preferment and the final dough. Yeast is worked out from your fermentation schedule, and you can override it by hand.

It works offline on Android and can save your recipes and back them up to a file.
