# Average Blood Pressure Calculator for Home Readings

> Average your home blood pressure readings, see the lowest, highest and AHA category, and learn the formula with a worked example.

- Web: https://apps.schimpf.es/health-connect-pdf-reports/average-blood-pressure-calculator/
- App: Health Reports: BP & Sleep PDF, https://apps.schimpf.es/health-connect-pdf-reports/index.md
A doctor usually wants the average of several home readings. This page gives you a small calculator for a list of readings, then explains the formula and a worked example so you can check it by hand.

## Calculator

Type one reading per line as systolic/diastolic, for example `122/78`. Nothing you type leaves your browser.

An interactive calculator is on the web page: https://apps.schimpf.es/health-connect-pdf-reports/average-blood-pressure-calculator/

## The formula

Systolic and diastolic are averaged separately.

- Average systolic = sum of all systolic values ÷ number of readings
- Average diastolic = sum of all diastolic values ÷ number of readings

Each result is rounded to the nearest whole number, with .5 rounding up. The lowest and highest reading are the ones with the lowest and highest systolic value. If two readings have the same systolic value, the diastolic value breaks the tie.

The average is then placed in a category using the AHA limits.

| Category | Systolic | | Diastolic |
|---|---|---|---|
| Normal | below 120 | and | below 80 |
| Elevated | 120–129 | and | below 80 |
| Stage 1 | 130–139 | or | 80–89 |
| Stage 2 | 140 or higher | or | 90 or higher |
| Above 180/120 | above 180 | and/or | above 120 |

Source: Whelton PK, et al. *2017 ACC/AHA/AAPA/ABC/ACPM/AGS/APhA/ASH/ASPC/NMA/PCNA Guideline for the Prevention, Detection, Evaluation, and Management of High Blood Pressure in Adults*. Hypertension, 2018; 71(6): e13–e115.

## Worked example

Seven morning readings over one week:

| Day | Reading |
|---|---|
| Monday | 128/82 |
| Tuesday | 122/78 |
| Wednesday | 135/85 |
| Thursday | 126/80 |
| Friday | 131/84 |
| Saturday | 120/76 |
| Sunday | 124/79 |

### Step 1: add the systolic values

128 + 122 + 135 + 126 + 131 + 120 + 124 = 886

### Step 2: add the diastolic values

82 + 78 + 85 + 80 + 84 + 76 + 79 = 564

### Step 3: divide by the number of readings

- 886 ÷ 7 = 126.57, which rounds to 127
- 564 ÷ 7 = 80.57, which rounds to 81

The average is 127/81.

### Step 4: find the lowest and highest

- Lowest systolic: 120/76
- Highest systolic: 135/85

### Step 5: place the average in a category

Systolic 127 is in the 120–129 row. Diastolic 81 is in the 80–89 row. The two numbers point to different rows, so the higher one wins: Stage 1.

The same week would land in Elevated if the diastolic average had been 79 or lower. One or two points can move an average across a line, so look at the whole list as well as the average.

## Category of the average versus category of each reading

The calculator averages the numbers first and categorizes afterward. You can also categorize each reading on its own. In the example:

- Stage 1: 128/82, 135/85, 126/80, 131/84 (4 readings)
- Elevated: 122/78, 120/76, 124/79 (3 readings)
- Normal, Stage 2 and Above 180/120: 0 readings

The category of the average and the counts per category can differ. Both are useful to show a doctor.

## Tips for a usable average

- Take readings over several days.
- Use the same arm, the same cuff and a similar time of day.
- Include every valid reading. Dropping the high ones makes the average meaningless.
- Do not average readings from different devices without noting it. Cuffs can differ by a few mmHg.

A calculator cannot judge whether a number is a problem for you. Take the list and the average to your doctor.

## Skip the arithmetic with the app

Health Connect PDF Reports for Android does this work for the readings stored in Health Connect. Its summary page shows average, lowest and highest blood pressure, the resting heart rate trend, average sleep length and how many readings fall in each AHA category. The detail pages list every reading with its time and source app. The average uses the same method as above: systolic and diastolic averaged separately and rounded to whole numbers. Readings that two apps recorded for the same event are merged first, so they count once.

You can also add a reading by hand in the app. It is saved to Health Connect. The app shows recorded values only and gives no diagnosis or medical advice.

See also: [Blood pressure categories chart](blood-pressure-categories-chart) and [How to make a blood pressure PDF from Health Connect](health-connect-blood-pressure-pdf).
