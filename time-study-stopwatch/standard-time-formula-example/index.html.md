# Standard Time Formula With a Worked Example

> How to calculate normal time and standard time from stopwatch readings, rating and allowance, with a worked example and a small calculator.

- Web: https://apps.schimpf.es/time-study-stopwatch/standard-time-formula-example/
- App: Time Study Stopwatch, https://apps.schimpf.es/time-study-stopwatch/index.md
Standard time is the time a trained worker needs for a task at a normal pace, plus time for rest and unavoidable delays. It is the number behind labor standards, line balancing and capacity plans. This page gives the formula, a worked example with real numbers, and a calculator you can use right away.

## The formula

Standard time is built in two steps.

1. Normal time = observed time × rating ÷ 100
2. Standard time = normal time × (1 + allowance ÷ 100)

Where:

- Observed time is what the stopwatch shows for one element.
- Rating is your judgment of the worker's pace. 100% means a normal pace. Above 100% means faster than normal, below 100% means slower.
- Allowance is the extra time for personal needs, fatigue and delays (PF&D), as a percent of normal time.

The method follows the classic work-measurement texts, for example Niebel and Freivalds, *Methods, Standards, and Work Design* (McGraw-Hill, 12th edition, 2009), and the International Labour Office, *Introduction to Work Study* (4th edition, 1992).

### Rules used in the app and in this page

- Normal time is worked out per element. Each observation is multiplied by its rating, then the results are averaged.
- The normal times of all elements are added up to give the normal cycle time.
- The allowance is a markup on normal time. A 15% allowance multiplies normal time by 1.15.
- Allowance is accepted from 0 to 100%.
- Rating is accepted from 50 to 200%.

Some sources define allowance as a share of the whole working time. In that version, standard time = normal time ÷ (1 − allowance ÷ 100), which gives different results. The formula on this page is the markup version.

## Worked example

A packer is timed on a task with two elements, over three cycles. Each observation has a rating.

| Element | Cycle | Observed (s) | Rating (%) | Observed × rating (s) |
|---|---|---|---|---|
| 1. Pick item | 1 | 20 | 110 | 22.00 |
| 1. Pick item | 2 | 22 | 100 | 22.00 |
| 1. Pick item | 3 | 18 | 120 | 21.60 |
| 2. Pack and seal | 1 | 40 | 90 | 36.00 |
| 2. Pack and seal | 2 | 44 | 100 | 44.00 |
| 2. Pack and seal | 3 | 42 | 95 | 39.90 |

### Step 1: normal time per element

- Element 1: (22.00 + 22.00 + 21.60) ÷ 3 = 21.87 s
- Element 2: (36.00 + 44.00 + 39.90) ÷ 3 = 39.97 s

### Step 2: normal cycle time

- 21.87 + 39.97 = 61.83 s

Compare this with the plain observed average: 20 s + 42 s = 62 s. The rating moved the result only a little here because the high and low ratings partly cancel. With a worker who is consistently fast or slow, the gap is larger.

### Step 3: apply the allowance

With a 15% allowance:

- 61.83 × 1.15 = 71.11 s

The standard time for one packing cycle is about 71.1 seconds. At that standard, one operator makes about 50 cycles per hour (3600 ÷ 71.11 = 50.6).

## Calculator

An interactive calculator is on the web page: https://apps.schimpf.es/time-study-stopwatch/standard-time-formula-example/

## Common mistakes

- Rating the worker, not the pace. Rate the speed and effort of the work you see. Rate each observation while you watch it.
- Skipping the rating. Without it, you get the average of how this operator worked on this day, which is not yet a standard.
- Mixing allowance methods. Check whether your company defines allowance on normal time or on the whole shift before you compare numbers.
- Too few cycles. Three cycles are fine for a demo. For a real standard, use more cycles and look at the spread. A large standard deviation means the method or the elements are not stable yet.
- Timing incomplete cycles. Only count cycles in which every element was timed, so the cycle total is not understated.

## Do it in the app

Time Study Stopwatch applies this same formula on the Results screen. You list the work elements once, tap the large lap button each time an element ends, and set a rating per observation. Enter the allowance on the study setup screen, and the app shows normal time per element, the normal cycle time and the standard time.

Average, minimum, maximum and standard deviation per element come with the app. Rating (50 to 200%), allowance and standard time are part of Time Study Pro, a one-time purchase on Google Play. Your data stays on the device, and CSV export lets you move the numbers to a spreadsheet.
