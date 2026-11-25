# Gemeinschaftsstunden Ersatzgeld berechnen

> How to calculate the fee for missed community work hours in a German allotment club, with proration for members who join mid-year and an example.

- Web: https://apps.schimpf.es/german-allotment-club-ledger/gemeinschaftsstunden-ersatzgeld-berechnen/
- App: Allotment Club Ledger, https://apps.schimpf.es/german-allotment-club-ledger/index.md
Most allotment clubs (Kleingartenvereine) expect each member to work a number of hours for the community each year: hedges, paths, the clubhouse, shared areas. Members who do not reach the number pay a fee for each missing hour. This page shows how to calculate it, including for members who held a plot for only part of the year.

## Who sets the hours and the fee

The federal allotment garden law (Bundeskleingartengesetz, BKleingG, 1983) does not give a number of hours. The club decides: the required hours and the fee per missing hour usually stand in the bylaws (Satzung) or in a general meeting resolution. Use the numbers your club decided. If the rule is not written down, a fee is hard to enforce, so get it written down first.

## The formula

1. **Required hours** = yearly required hours × months held ÷ 12
2. **Missing hours** = required hours − hours worked (never below zero)
3. **Fee** = missing hours × fee per hour

Hours worked above the requirement do not create a credit in this formula. Missing hours are never negative.

### Example: whole year

- Required: 10 hours
- Worked: 4,5 hours
- Missing: 10 − 4,5 = 5,5 hours
- Fee: 15,00 € per hour
- Fee due: 5,5 × 15,00 € = **82,50 €**

## Members who hold a plot for part of the year

A new member who took over a plot in June cannot do a full year of work. Scale the requirement by the months the member held a plot in that year.

### Example: 7 months

- Required for a full year: 10 hours
- Months held: 7 (June to December)
- Required: 10 × 7 ÷ 12 = 5,83 hours

Round to a practical step. The app rounds to the nearest half hour, half up, so 5,83 hours becomes **6 hours**. The member worked 2,5 hours:

- Missing: 6 − 2,5 = 3,5 hours
- Fee: 3,5 × 15,00 € = **52,50 €**

A member who holds no plot in that year has no requirement and owes no fee. If a member held two plots in different months, count each month once.

## Common cases

| Case | Result |
|---|---|
| Worked more than required | Missing hours are 0, no fee |
| Worked exactly the requirement | No fee |
| Held a plot for 12 months | Full requirement |
| Held a plot for 3 months | 10 × 3 ÷ 12 = 2,5 hours required |
| Left the club mid-year | Count the months held, same as a new member |

### Half hours

Clubs usually track time in half hours. Keep one step for everyone. With 15,00 € per hour, a half hour costs 7,50 €. If the fee per hour has cents, round only the final fee, to whole cents.

## Handling the fee in the books

The fee is club income, usually booked in its own category. Record who owes it and who paid it, so the cash audit (Kassenprüfung) can match payments to charges. Many clubs put it on the same yearly invoice as rent, so that members pay once. See [how to calculate allotment garden rent](kleingarten-pacht-berechnen) for the rent side of that invoice.

## Do it in the app

Allotment Club Ledger keeps the required hours, the hours worked and the fee per hour per year. You enter the worked hours per member on a fast entry screen, in steps of half an hour. The app scales the requirement by months held, rounds to half hours, and creates the fee automatically when hours are missing. The fee appears on the member's yearly invoice PDF and in the open items list.

The app works offline and has no internet permission. Member data stays on your device, and a password-protected backup goes to a file you choose.
