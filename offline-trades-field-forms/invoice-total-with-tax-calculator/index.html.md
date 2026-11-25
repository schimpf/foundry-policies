# Invoice Total With Tax: Formula and Calculator

> How to work out an invoice subtotal, tax and total from line items, with a worked example, rounding rules and a small calculator.

- Web: https://apps.schimpf.es/offline-trades-field-forms/invoice-total-with-tax-calculator/
- App: Field Forms: Job Sheets & PDFs, https://apps.schimpf.es/offline-trades-field-forms/index.md
Invoices go wrong in small ways: tax added to the wrong figure, a discount applied twice, or a rounding penny that makes the total differ from the client's own sum. This page shows the exact steps, a worked example and a calculator you can use right here.

## The formula

An invoice with one tax rate follows three steps:

1. **Line total** = quantity × unit price, for each line.
2. **Subtotal** = the sum of all line totals.
3. **Tax** = subtotal × tax rate. **Total** = subtotal + tax.

Prices on the lines are entered without tax. Tax is added once, at the bottom, on the subtotal. That keeps the invoice easy to check, with one rate and one tax figure.

## Worked example

A heating engineer bills labor, a part and a goodwill discount. The tax rate is 20%.

| Description | Qty | Unit price | Line total |
|---|---|---|---|
| Labor (hours) | 2.5 | 48.00 | 120.00 |
| Pump | 1 | 86.40 | 86.40 |
| Discount | 1 | -20.00 | -20.00 |

- Subtotal: 120.00 + 86.40 − 20.00 = 186.40
- Tax at 20%: 186.40 × 0.20 = 37.28
- Total: 186.40 + 37.28 = 223.68

The discount is a line with a negative price. Because it sits inside the subtotal, tax is charged on the reduced amount. A deposit already paid works the same way: enter it as a negative line.

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/offline-trades-field-forms/invoice-total-with-tax-calculator/

## Rounding rules

Money has no fractions of a cent or penny, so every step rounds to the smallest currency unit. The app rounds half up: a value ending in exactly half a unit goes away from zero.

- Rounding happens on each line total, then once more on the tax.
- Example: 1.5 × 3.33 = 4.995, which rounds to 5.00.
- Example: tax on a subtotal of 10.03 at 17.5% is 1.75525, which rounds to 1.76.

The app keeps all amounts as whole minor units (cents or pence) and never uses floating point numbers, so the result is the same every time. Rounding the tax once on the subtotal, rather than per line, avoids a drift between the lines and the total.

Some currencies, such as the Japanese yen, have no minor unit. The app reads the number of decimal places from the currency code, so those amounts round to whole units.

## Common mistakes

- **Tax on tax.** Do not add tax to prices that already include it. Enter prices without tax and let the total add it.
- **Discount after tax.** If you subtract a discount from the total instead of the subtotal, the client is charged tax on the discount.
- **Mixed rates.** If part of the job is taxed at a different rate, split it into two invoices, or check with your accountant how to show it. The app uses one rate per document.
- **Quantity in minutes.** Use hours as decimals: 90 minutes is 1.5, 20 minutes is 0.333.

## Which tax rate to use

The rate depends on where you work and what you sell. Look it up with your tax authority, for example HMRC in the UK or your state revenue department in the US. This page does not state a rate for any country. The 20% above is an example only.

## Do it on site with Offline Trades Field Forms

In the Android app **Offline Trades Field Forms**, you add line items with description, quantity and unit price. The app does the sums above, adds tax at the rate you set once in settings, and numbers the document automatically (INV-0001, INV-0002 and so on, with a prefix you can change).

- Set a default tax rate once and change it per document if needed.
- Enter discounts and deposits as negative lines.
- Quotes convert to an invoice in one tap after the client signs on the screen.
- Invoices get a due date, a paid toggle and an overdue marker.
- Everything works offline and the invoice leaves your phone as a PDF through the share sheet.
