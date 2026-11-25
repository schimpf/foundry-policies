# How to Make a Blood Pressure PDF from Health Connect

> Step-by-step: turn blood pressure, heart rate and sleep stored in Android Health Connect into a PDF report you can share or print for your doctor.

- Web: https://apps.schimpf.es/health-connect-pdf-reports/health-connect-blood-pressure-pdf/
- App: Health Reports: BP & Sleep PDF, https://apps.schimpf.es/health-connect-pdf-reports/index.md
Many blood pressure cuffs, watches and apps write their readings to Health Connect, the data store built into Android. Health Connect stores the data and builds no report you can hand to a doctor. This page shows what you need and how to turn the data into a clean PDF.

## What you need

- An Android phone. Android 14 and newer include Health Connect. On Android 9 to 13, install the Health Connect app from Google Play.
- Readings in Health Connect. They can come from a connected cuff, a watch or a health app that supports Health Connect. You can also add blood pressure readings by hand.
- The app Health Connect PDF Reports.

## Step by step

1. Open the app and connect. On first launch, tap Connect Health Connect and allow the permissions. The app reads heart rate, blood pressure and sleep. It writes blood pressure only, for readings you add by hand.
2. Choose the date range. Pick 7, 30 or 90 days, or set your own dates. Presets end yesterday, so the report holds complete days only.
3. Choose what to include. Blood pressure, heart rate and sleep are all on by default. Switch off what your doctor does not need.
4. Add your name if you want. It is optional. No date of birth is needed. The name is only saved if you ask for that.
5. Check the sources. If two apps record the same readings, set a preferred source app for each metric, or leave it on Auto.
6. Preview. Page through the report before you send it.
7. Share or print. Use the normal Android share sheet to send the PDF by email or message, or use the print dialog.

## What is in the report

The report begins with a summary page, then has one section per metric.

### Summary page

- Blood pressure: average, lowest and highest, and the number of readings.
- Heart rate: average, lowest and highest, and the resting average. For ranges of 14 days or more, the change in resting heart rate between the first 7 and last 7 days.
- Sleep: average, shortest and longest night.
- Blood pressure readings counted by AHA category.

### Blood pressure pages

A table of every reading with time, source app and AHA category. Categories use neutral wording, such as Normal, Elevated, Stage 1, Stage 2 and Above 180/120. The limits are in the [blood pressure categories chart](blood-pressure-categories-chart).

### Heart rate pages

A daily table with resting, lowest, highest and average values, plus a trend chart of the resting heart rate.

### Sleep pages

A nightly table with total time and sleep stages, plus a stage summary averaged per night. The summary page's sleep average counts time in bed minus the awake stage.

## How duplicates are handled

If a cuff app and a second app both save the same reading, you would see it twice. The app treats two blood pressure readings as the same event when:

- they come from different apps,
- they are within 2 minutes of each other, and
- both the systolic and the diastolic values differ by 2 mmHg or less.

The reading from the preferred source is kept. The report notes how many duplicates were merged. Sleep sessions from different apps are merged when they overlap by more than half of the shorter session.

## About the 30-day limit

Health Connect only gives an app the last 30 days of data unless you allow access to history. The app asks for that extra permission only when the range reaches back further than 30 days.

## Privacy

- The app has no internet permission and no account.
- It does not keep a copy of your health data. Health Connect stays the only place the data lives.
- The PDF is created in temporary storage and deleted when you leave the preview. It goes only where you choose to send it.

## Good to know

- One export is available without payment. More exports need a one-time in-app purchase called Unlimited reports. Viewing data, preview, manual entry and the widget do not need a purchase.
- The app shows recorded values only. It gives no diagnosis and no medical advice.
- Units are mmHg for blood pressure and the date format follows your system.

## Tips before the appointment

- Preview the PDF and make sure the date range matches what your doctor asked for.
- Add a few manual readings if your cuff does not sync, so the log has no gaps.
- Bring the report as a printout or have it ready on your phone.

If you want to check numbers on your own first, try the [average blood pressure calculator](average-blood-pressure-calculator).
