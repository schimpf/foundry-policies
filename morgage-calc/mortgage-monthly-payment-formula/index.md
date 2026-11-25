# Mortgage Monthly Payment Formula With Example

> How a fixed-rate mortgage payment is calculated, with a worked example for 200,000 euros at 2.60 % over 30 years, and a calculator you can try.

- Web: https://apps.schimpf.es/morgage-calc/mortgage-monthly-payment-formula/
- App: Hipoteca: Mortgage Calculator, https://apps.schimpf.es/morgage-calc/index.md
A fixed-rate mortgage has the same payment every month. It comes from one formula, called the annuity or French amortization formula. This page explains it, works one example by hand, and shows where the money goes.

## The formula

**Payment = L × r / (1 − (1 + r)^−n)**

- **L** is the loan amount.
- **r** is the monthly rate: the annual rate (TIN) divided by 12.
- **n** is the number of monthly payments: years × 12.

If the rate is 0 %, the formula does not work (it divides by zero). The payment is then L / n.

## Worked example

Loan of 200,000 euros, 2.60 % TIN, 30 years.

1. Monthly rate: r = 0.026 / 12 = 0.0021667
2. Number of payments: n = 30 × 12 = 360
3. (1 + r)^−360 = about 0.4588
4. 1 − 0.4588 = 0.5412
5. Payment = 200,000 × 0.0021667 / 0.5412 = about 800.68 euros per month

Over the whole loan:

- Total paid: 360 × 800.68 = about 288,245 euros
- Total interest: about 88,245 euros

## Where each payment goes

Each month the bank charges interest on what you still owe. The rest of the payment reduces the debt.

1. Interest = balance × r
2. Principal repaid = payment − interest
3. New balance = old balance − principal repaid

Month 1 of the example:

- Interest: 200,000 × 0.0021667 = 433.33 euros
- Principal: 800.68 − 433.33 = about 367.35 euros
- New balance: about 199,632.65 euros

Because the balance falls, interest falls too, and more of every later payment goes to principal. The payment stays the same.

| Month | Interest share | Principal share |
|---|---|---|
| 1 | about 54 % | about 46 % |
| Last | under 1 % | over 99 % |

## What changes the payment most

- **Term.** A longer term lowers the payment but raises total interest. At the same 2.60 %, 20 years instead of 30 raises the payment to about 1,070 euros but cuts total interest to roughly 56,700 euros.
- **Rate.** In the example, going from 2.60 % to 3.60 % lifts the payment from about 801 to about 909 euros, around 14 % more.
- **Amount.** The payment is proportional to the loan. Halve the loan and the payment halves.

## Variable and mixed rates

The formula assumes the rate does not change. With a variable mortgage the rate is Euríbor plus a spread, and it is reset at each revision (usually every 12 months). At each reset the bank recalculates the payment with the same formula, using:

- L = the balance you still owe
- r = the new rate divided by 12
- n = the months left

So a variable payment is the same calculation repeated with new inputs. The payment you see today is only valid until the next revision.

## What the formula leaves out

- **TIN and TAE.** The formula uses the TIN, the nominal rate. The TAE (the Spanish APR) also counts fees and required products such as insurance, so it is usually higher than the TIN.
- **Purchase costs.** Taxes, notary, registry and the down payment are paid on top of the loan and are not in the payment.
- **Rounding.** Banks round each payment to the cent. A schedule from your bank can differ from a hand calculation by a few cents.

## Try it

An interactive calculator is on the web page: https://apps.schimpf.es/morgage-calc/mortgage-monthly-payment-formula/

## Do it in the app

Hipoteca applies this formula to your own offer. Enter the price, savings, term and rate type to see the monthly payment, the TIN and TAE, the split between principal and interest, and the cash you need on day one. The yearly schedule and balance chart show how the debt falls, and you can export the schedule as PDF or CSV. For variable and mixed loans, the app can also test what happens to the payment if Euríbor rises.

Results are estimates and do not replace an offer from your bank.
