# Invoice Due Date and Overdue: How to Work It Out

> How to set invoice payment terms, calculate the due date and tell when an invoice is overdue, with a worked example and a simple routine.

- Web: https://apps.schimpf.es/offline-trades-field-forms/invoice-due-date-and-overdue/
- App: Field Forms: Job Sheets & PDFs, https://apps.schimpf.es/offline-trades-field-forms/index.md
"Payment within 14 days" sounds clear until someone asks when day 14 is, or when the invoice becomes late. This page shows how to count it, what overdue means and how to keep track without a spreadsheet.

## The formula

- **Due date** = invoice date + payment terms (in days).
- **Overdue** = the invoice is unpaid and today is after the due date.

An invoice due on 17 March is still on time on 17 March. It becomes overdue on 18 March. A paid invoice is never overdue, however old it is.

## Worked example

You issue an invoice on 3 March with 14-day terms.

1. Start at 3 March.
2. Add 14 days: 3 + 14 = 17, so the due date is 17 March.
3. On 17 March the invoice is unpaid but not yet overdue.
4. On 18 March it is 1 day overdue.
5. On 25 March it is 8 days overdue.

Crossing a month end works the same way. With 30-day terms from 20 June, the due date is 20 July. With 14-day terms from 25 February in a non-leap year, the due date is 11 March.

| Invoice date | Terms | Due date | First overdue day |
|---|---|---|---|
| 3 March | 14 days | 17 March | 18 March |
| 20 June | 30 days | 20 July | 21 July |
| 25 February (non-leap year) | 14 days | 11 March | 12 March |

## Choosing payment terms

- **Shorter terms suit small jobs.** Seven to fourteen days is common for domestic work.
- **Longer terms suit commercial clients,** who often have their own payment cycle. Agree it before you start.
- **State the terms on the quote,** so the client has already accepted them when the invoice arrives.
- **Check local rules.** Late-payment rights and interest differ by country and by whether the client is a business or a consumer. Look up your own rules, for example the UK's Late Payment of Commercial Debts (Interest) Act 1998, or ask your state or national small-business authority in the US.

## A simple routine to chase payment

1. **Send the invoice the same day** as the work, as a PDF, to the client's own email.
2. **Check unpaid invoices once a week.** A fixed day works well.
3. **On the due date,** do nothing. It is not late yet.
4. **One day overdue,** send a short, friendly reminder with the invoice number and amount.
5. **A week overdue,** call the client.
6. **Mark it paid** the day money arrives, with the paid date.

## What to write on the invoice

Put these on every invoice so there is nothing to argue about later:

- The invoice number and the invoice date.
- The due date, written as a date as well as "14 days".
- The total due, with the tax shown as its own line.
- Your business name, address, phone, email and tax ID.
- How you want to be paid, such as bank transfer details.

Writing the actual date removes any doubt about when counting starts. If the client signs a quote first, the invoice date is the day you issue the invoice.

## Deposits and discounts

A deposit you already received reduces what is due. Enter it on the invoice as a negative line, so the total shows only the balance. Discounts work the same way. See the worked example in the invoice total page for how this affects tax.

## Track it in Offline Trades Field Forms

The Android app **Offline Trades Field Forms** does the date math for you.

- Payment terms are set once in settings. The default is 14 days, and you can change the due date on each invoice.
- A paid/unpaid toggle records the paid date.
- An invoice shows **Overdue** when it is unpaid and past its due date. The badge carries text as well as a color.
- A job shows its most urgent status: overdue, then unpaid, then accepted quote, then draft.
- The home-screen widget shows the total of unpaid and overdue invoices, with a button to start a new job. Amounts are hidden while the app lock is on.
- Invoices are numbered automatically (INV-0001 and so on), and a signed quote converts to an invoice in one tap.
- It works without signal or an account.
