# Plumbing Quote: Sales Tax and Deposit Math

> How to add sales tax to taxable lines only, set a deposit % on the total and find the balance due on a plumbing quote. Worked example and calculator.

- Web: https://apps.schimpf.es/offline-plumber-invoice-app/plumbing-quote-sales-tax-and-deposit/
- App: Plumber Invoice & Quote Maker, https://apps.schimpf.es/offline-plumber-invoice-app/index.md
## The three numbers on a quote

A plumbing quote ends with three amounts: the tax, the total and the deposit. They depend on each other in a fixed order.

1. Add up every line. Each line is quantity × unit price, rounded to the cent. This is the subtotal.
2. Add up only the lines marked taxable. Multiply that amount by the tax rate. This is the tax.
3. Subtotal plus tax is the total.
4. Multiply the total by the deposit percentage. This is the deposit.
5. Total minus what the customer has paid is the balance due.

Offline Plumber Invoice App follows exactly this order. Rounding is half up to the cent, so 223.797 becomes 223.80.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumber-invoice-app/plumbing-quote-sales-tax-and-deposit/

## Worked example: a bathroom repipe

The job has these lines:

| Line | Qty | Unit price | Taxable | Line total |
|------|-----|-----------|---------|-----------|
| PEX pipe, 3/4 in | 100 ft | $1.20 | yes | $120.00 |
| Fittings and valves | 1 | $292.00 | yes | $292.00 |
| Labor | 6 hr | $50.00 | no | $300.00 |

- Subtotal: $120.00 + $292.00 + $300.00 = $712.00
- Taxable base: $120.00 + $292.00 = $412.00
- Tax at 8.25%: $412.00 × 0.0825 = $33.99
- Total: $712.00 + $33.99 = $745.99
- Deposit at 30%: $745.99 × 0.30 = $223.797, rounded to $223.80
- Balance after the deposit: $745.99 − $223.80 = $522.19

The tax rate is a single combined rate, as it appears on your local rate table (state plus county plus city). The app takes one rate per document.

## Tax on the lines, not on the total

Tax applies to the taxable base. In the example, taxing the full $712.00 would give $58.74, which is $24.75 too much. Whether labor is taxable depends on the state and on the kind of work. Some states tax repair labor, others tax only materials, and some treat new construction differently from repair. Look up the rule for your state on your state department of revenue website, or ask your accountant, before you set up your lines.

In the app, each line has its own taxable checkbox. Price book items marked as labor start as not taxable, and other items start as taxable. You can change either on the line. Each quote has its own tax rate and deposit %, and a new quote starts from the defaults in your business profile.

## The deposit is a share of the total

The deposit percentage applies to the total including tax. A 30% deposit on $745.99 is $223.80. Collect it before you order parts or start work on bigger jobs.

The deposit has no document of its own. When you collect it, you record it as a payment on the invoice, with the date and a method: cash, check or other. The invoice then shows the balance due. In the example, a second payment of $200.00 by check leaves $322.19.

## What the app checks for you

- A quote cannot be signed with no lines, or with a line that has no price.
- The tax and deposit update as you type.
- You cannot record a payment larger than the balance due.
- Once the customer signs with a finger, the quote is locked. One tap turns it into an invoice, and the lines are copied over.
- The invoice status moves to Partially paid after the first payment and to Paid when the payments cover the total.

To set the price of a part first, see the [plumbing markup formula and table](../plumbing-markup-calculator/).

The app works with no signal. You can write the quote in a basement, get the signature there and send the PDF later from the Outbox.
