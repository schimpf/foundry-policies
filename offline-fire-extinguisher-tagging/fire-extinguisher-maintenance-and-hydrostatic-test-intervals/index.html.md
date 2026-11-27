# Fire Extinguisher Hydrostatic Test Interval Chart

> Chart of NFPA 10 monthly, annual, 6-year maintenance and hydrostatic test intervals for ABC, CO2, water, foam, wet chemical and other extinguishers.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/fire-extinguisher-maintenance-and-hydrostatic-test-intervals/
- App: Fire Extinguisher Inspection, https://apps.schimpf.es/offline-fire-extinguisher-tagging/index.md
## Interval chart by extinguisher type

NFPA 10, Standard for Portable Fire Extinguishers (2022 edition), sets how often each portable extinguisher needs inspection, maintenance and a hydrostatic test. The intervals depend on the type. The table lists the ones the app uses.

| Type | Monthly inspection | Annual maintenance | 6-year maintenance | Hydrostatic test |
|---|---|---|---|---|
| ABC dry chemical | every 31 days | 12 months | yes | every 12 years |
| BC dry chemical | every 31 days | 12 months | yes | every 12 years |
| Clean agent | every 31 days | 12 months | yes | every 12 years |
| Dry powder (Class D) | every 31 days | 12 months | no | every 12 years |
| CO2 | every 31 days | 12 months | no | every 5 years |
| Water / water mist | every 31 days | 12 months | no | every 5 years |
| Foam (AFFF/FFFP) | every 31 days | 12 months | no | every 5 years |
| Wet chemical (Class K) | every 31 days | 12 months | no | every 5 years |

Sources: NFPA 10 (2022), section 7.2 for monthly inspection, section 7.3 for annual and 6-year maintenance, and section 8.3 for hydrostatic testing. Your authority having jurisdiction (AHJ) may require shorter intervals.

## What each interval means

### Monthly: every 31 days

A quick visual check of location, seal, gauge, condition and tag. The app counts 31 days from the last monthly date.

### Annual: 12 months

A fuller maintenance check, including mechanical parts, agent condition and the hose and nozzle. The next date is 12 months after the last annual date. The [checklist page](../nfpa-10-monthly-annual-inspection-checklist/) lists every item.

### 6-year maintenance

Applies to the ABC dry chemical, BC dry chemical and clean agent types in the table above. The unit is emptied and examined inside. The next date is 6 years after the last 6-year maintenance. If none is on record, the app counts 6 years from the manufacture date.

### Hydrostatic test: 5 or 12 years

The cylinder is pressure tested to check it still holds. The next date is the test interval after the last hydro date. If none is on record, the app counts from the manufacture date.

## Worked example

An ABC dry chemical extinguisher was made on 2 March 2016. Nothing else is on record, except a monthly check on 10 January 2026 and an annual check on 15 June 2025.

- **Next monthly:** 10 January 2026 plus 31 days is 10 February 2026.
- **Next annual:** 15 June 2025 plus 12 months is 15 June 2026.
- **Next 6-year:** no 6-year date on record, so 2 March 2016 plus 6 years is 2 March 2022. That date is long past, so the unit is overdue.
- **Next hydro:** no hydro date on record, so 2 March 2016 plus 12 years is 2 March 2028.

Now take a CO2 unit made on 20 August 2021 with no other dates. CO2 has no 6-year maintenance, so that row is not required. Its hydro date is 20 August 2021 plus 5 years, which is 20 August 2026.

The date arithmetic uses calendar months and years. A date that lands on a day the target month does not have moves to the last day of that month, so 31 August plus 6 months gives 28 February (or 29 in a leap year).

## How the app marks status

For each due date the app compares the date with today:

- **Overdue:** the due date has passed.
- **Due soon:** monthly items 7 days or fewer away, all other items 30 days or fewer away.
- **OK:** anything later.
- **Not recorded:** no date to count from.

An extinguisher shows its worst item. A failed latest inspection ranks above overdue, then overdue, due soon and OK. A unit with nothing recorded shows as new.

## Calculate it for one unit

Use the calculator on the [due date calculator page](../fire-extinguisher-due-date-calculator/) to enter the dates for one extinguisher and see all four next dates.

## Tracking it for a whole site

Offline fire extinguisher tagging stores the last monthly, annual, 6-year and hydro dates for every extinguisher and works out the next dates from the type, using the rules above. Each unit, site and client shows OK, due soon or overdue. It sends one reminder per site once a day, and the home screen widget shows the overdue and due soon counts and the next site to visit. It records the dates only. It has no checklists for the 6-year and hydro work.
