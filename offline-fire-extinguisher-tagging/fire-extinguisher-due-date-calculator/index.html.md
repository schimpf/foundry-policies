# Fire Extinguisher Due Date Calculator (NFPA 10)

> Enter an extinguisher's type and last service dates to get its next monthly, annual, 6-year and hydrostatic test dates, with the formulas explained.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/fire-extinguisher-due-date-calculator/
- App: Fire Extinguisher Inspection, https://apps.schimpf.es/offline-fire-extinguisher-tagging/index.md
## Calculate the next service dates

Pick the extinguisher type and enter the dates you have. Leave a field empty if there is no record. The calculator uses the same rules as the app, based on NFPA 10, Standard for Portable Fire Extinguishers (2022 edition).

An interactive calculator is on the web page: https://apps.schimpf.es/offline-fire-extinguisher-tagging/fire-extinguisher-due-date-calculator/

## The formulas

Each next date starts from the last date on record.

| Item | Next due date | Falls back to manufacture date? |
|---|---|---|
| Monthly | last monthly + 31 days | no |
| Annual | last annual + 12 months | no |
| 6-year maintenance | last 6-year + 6 years | yes |
| Hydrostatic test | last hydro + 5 or 12 years | yes |

- 6-year maintenance applies to ABC dry chemical, BC dry chemical and clean agent units. For the other types the row reads "not required".
- The hydro interval is 12 years for ABC, BC, clean agent and Class D dry powder, and 5 years for CO2, water, foam and Class K wet chemical.
- Monthly and annual dates have no fallback. With no last monthly or annual date, the result is "not recorded".

The full list by type is in the [interval chart](../fire-extinguisher-maintenance-and-hydrostatic-test-intervals/).

## How the status is set

The calculator counts the days between today and the due date.

- **Overdue:** fewer than 0 days left.
- **Due soon:** 0 to 7 days for monthly, 0 to 30 days for the other items.
- **OK:** more days than that.

## Worked example

A water extinguisher was made on 14 May 2019. The last monthly check was on 1 November 2026, the last annual check on 20 December 2025, and no hydro test is on record. Assume today is 27 November 2026.

1. **Monthly:** 1 November 2026 + 31 days = 2 December 2026. That is 5 days away, so it is due soon (7 days or fewer).
2. **Annual:** 20 December 2025 + 12 months = 20 December 2026. That is 23 days away, so it is due soon (30 days or fewer).
3. **6-year:** water does not need it, so it is not required.
4. **Hydro:** no hydro date, so 14 May 2019 + 5 years = 14 May 2024. That is past, so it is overdue by 927 days.

The unit shows as overdue, driven by the hydro test, because overdue ranks above due soon.

## Edge cases

- **Month ends:** 31 August + 6 months gives the last day of the target month, 28 February or 29 in a leap year. A 29 February date plus 1 year gives 28 February.
- **A failed inspection:** in the app, a failed latest inspection ranks above overdue in the unit's status. The calculator here only shows dates.
- **Stricter local rules:** your authority having jurisdiction can require shorter intervals. Use the shorter one.

## Doing it for a whole site

Typing dates into a calculator works for one unit. For a site with 40 extinguishers, Offline fire extinguisher tagging stores the dates on the phone, works out each next date from the type with these formulas, and lists the overdue units first. You scan the QR code or barcode on the tag to open a unit. It works without a signal and has no account. The free version holds 25 extinguishers, so a site of 40 needs Pro.

The [NFPA 10 checklist page](../nfpa-10-monthly-annual-inspection-checklist/) covers the monthly and annual checks that update these dates.
