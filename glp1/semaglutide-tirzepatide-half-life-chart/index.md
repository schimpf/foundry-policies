# Semaglutide, Tirzepatide and Liraglutide Half-Life Chart

> Half-life of semaglutide, tirzepatide and liraglutide, with a decay table, the formula and a worked example of how much is left days after a dose.

- Web: https://apps.schimpf.es/glp1/semaglutide-tirzepatide-half-life-chart/
- App: GLP Mate: GLP-1 Shot Tracker, https://apps.schimpf.es/glp1/index.md
This page gives the half-life of three common GLP-1 ingredients, a table of how much remains after a given time, and the formula behind it. A small calculator is included.

This is general information and gives no medical advice. Do not change your dose or schedule because of a number on this page. Follow your prescriber and the leaflet that comes with your medication.

## Half-life chart

| Ingredient | Example brands | Half-life | Typical schedule |
|---|---|---|---|
| Semaglutide | Ozempic, Wegovy, Rybelsus | about 1 week (168 hours) | once a week (injection) or once a day (Rybelsus pill) |
| Tirzepatide | Mounjaro, Zepbound | about 5 days (120 hours) | once a week |
| Liraglutide | Victoza, Saxenda | about 13 hours | once a day |

Sources: the EU Summaries of Product Characteristics (EMA), section 5.2 "Pharmacokinetic properties", for Ozempic, Mounjaro and Victoza. They give a half-life of about one week for semaglutide, about 5 days for tirzepatide and about 13 hours for liraglutide. Check the current edition of your own leaflet, because labels are updated.

Half-life is the time it takes for the amount of drug in the body to fall by half. After one half-life, half of the drug is still there. Real half-lives also vary from person to person.

## The formula

If you take one dose, the amount left after a time *t* is:

**remaining = dose × 0.5 ^ (t / half-life)**

Use the same unit for *t* and for the half-life, for example hours.

If you take several doses, work out each one separately and add the results. This is the simple model that GLP Mate uses for its estimated level chart. It ignores absorption (how fast the dose enters the blood), so it is only a rough guide.

## How much is left? Decay table

Share of a single dose that remains, using the half-lives above:

| Time after the dose | Semaglutide | Tirzepatide |
|---|---|---|
| 1 day | 90.6 % | 87.1 % |
| 3 days | 74.3 % | 66.0 % |
| 7 days | 50.0 % | 37.9 % |
| 14 days | 25.0 % | 14.4 % |
| 21 days | 12.5 % | 5.4 % |
| 35 days | 3.1 % | 0.8 % |

For liraglutide, with a half-life of 13 hours:

| Time after the dose | Remaining |
|---|---|
| 12 hours | 52.7 % |
| 24 hours | 27.8 % |
| 48 hours | 7.7 % |
| 72 hours | 2.2 % |

## Worked example

You take semaglutide once a week. Half-life: 168 hours (7 days).

1. One week after a dose, 0.5 ^ (7 / 7) = 0.5, so 50 % is left.
2. Two weeks after, 0.5 ^ 2 = 0.25, so 25 % is left.
3. Take the same dose every 7 days. Before your second dose, 50 % of the first is left. Before the third, 50 % + 25 % = 75 %.
4. Before the fourth dose: 50 + 25 + 12.5 = 87.5 %. Before the fifth: 93.75 %.

So the amount on board builds up over the first weeks and then levels off. Right after a dose, the total is the new dose (100 %) plus what was left. At a steady rhythm, the low point before a dose is about half of the high point right after it. The semaglutide label says steady state is reached after about 4 to 5 weeks of weekly dosing.

For tirzepatide, one week is 7 / 5 = 1.4 half-lives. Each week 0.5 ^ 1.4 = 37.9 % is left, so the level swings more between doses than with semaglutide.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/glp1/semaglutide-tirzepatide-half-life-chart/

## What this does not tell you

- It shows the amount relative to the dose and gives no concentration in your blood.
- It does not predict how you feel, how much weight you lose or when side effects start or stop.
- Compounded products can differ from branded pens. Ask your pharmacist.
- The half-life is the same whatever your dose is. A higher dose lasts longer in absolute terms, but the share that remains after a week is the same.

## Track it in GLP Mate

GLP Mate is a private diary for GLP-1 medication on Android. You log each dose with time, amount in mg, injection site, pain and lot number. The app adds up your logged doses with the formula above and draws an estimated level per ingredient, shown as a percentage of its own peak. Premium shows this chart. It is clearly marked as an estimate, and it never recommends a dose.

Your data stays encrypted on your phone. You can also add daily check-ins for food noise and side effects, and share a PDF report with your doctor.
