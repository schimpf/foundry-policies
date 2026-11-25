# Allotment water meter cost: formula and example

> How to bill water or electricity in an allotment club from meter readings: formula, base fee, worked example and what to do with odd readings.

- Web: https://apps.schimpf.es/german-allotment-club-ledger/allotment-water-meter-cost-calculation/
- App: Allotment Club Ledger, https://apps.schimpf.es/german-allotment-club-ledger/index.md
In many allotment clubs (Kleingartenvereine) each plot has its own water meter, and some have an electricity meter too. The treasurer reads them once a year and bills each plot for what it used. This page gives the formula, a worked example, and rules for readings that look wrong.

## The formula

**Consumption = end reading − start reading**

**Cost = consumption × price per unit + base fee**

- Water is billed per cubic metre (m³), electricity per kilowatt hour (kWh).
- The price per unit is set by the club. It usually follows what the club pays its supplier, plus meter and maintenance costs.
- The base fee (Grundgebühr) is optional. It is a flat amount per plot and year that covers fixed costs, whatever the consumption.

### Example: one plot, one year

- Start reading, 1 January: 1.204 m³
- End reading, 31 December: 1.236,5 m³
- Consumption: 1.236,5 − 1.204 = **32,5 m³**
- Price: 4,20 € per m³
- Base fee: 12,00 €

Cost: 32,5 × 4,20 € = 136,50 €, plus 12,00 € = **148,50 €**.

German notation uses a dot for thousands and a comma for decimals, so 1.236,5 is one thousand two hundred thirty-six and a half. The prices above are examples only. Use your own club's figures.

## Where the end reading becomes the next start reading

The end reading of one year is the start reading of the next. If the two do not match, something happened between the readings: a typo, a meter swap, or someone read the wrong meter. Check this before you bill.

| Situation | What to check |
|---|---|
| End reading lower than start reading | Typo, meter swap, or a meter that rolled over |
| Start reading differs from last year's end reading | Typo, or the meter was replaced |
| Very high consumption | Leak, or a hose left running |

### Meter swap

When a meter is replaced, the new meter starts at or near zero, so a plain subtraction gives a negative number. Do not bill a negative amount. Treat it as zero and bill the real consumption from the old meter's final reading and the new meter's first reading, which you note by hand. Allotment Club Ledger bills a negative result as zero, so it never creates a credit by accident.

## When the tenant changes mid-year

Water and electricity are a plot charge, so they follow the same month-based split as rent. The consumption is not read on the handover day, so the club divides the yearly amount by the months each tenant held the plot. Both tenants share the base fee in the same way.

If your club reads the meter on the handover day instead, bill each tenant for their own consumption. Agree on one rule and write it into your bylaws, so that nobody is surprised.

### Example: split after June

- Yearly cost: 148,50 €
- Tenant A: January to June, 6 months: 148,50 € × 6 ÷ 12 = 74,25 €
- Tenant B: July to December, 6 months: 148,50 € − 74,25 € = 74,25 €

See [how to calculate allotment garden rent](kleingarten-pacht-berechnen) for how rounding is handled when the shares do not divide evenly.

## Checklist for reading day

1. Read every meter on the same day, near the end of the year.
2. Write down the number with all digits after the comma.
3. Take a photo of the meter face if you can.
4. Compare each start reading with last year's end reading.
5. Look into every plot with an end reading lower than the start reading.
6. Bill only after the checks.

## Do it in the app

Allotment Club Ledger has a fast entry screen for meter readings, plot by plot, in order. It stores readings with three decimals, so 1.236,5 is exact. It warns you when an end reading is lower than the start reading, or when a start reading does not match the previous end reading. The warnings do not block saving, because a meter swap is a valid reason.

You set the price per m³ or per kWh and an optional base fee once per year. The app then adds the water and electricity lines to every plot's charges, splits them by month for tenant changes, and puts them on the yearly invoice PDF.

The app has no internet permission, so readings and prices stay on your device.
