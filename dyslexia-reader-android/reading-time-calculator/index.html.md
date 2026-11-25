# Reading Time Calculator: How Long to Read a Book

> Work out how long a book takes to read from its word or character count. Formula, worked examples and a small calculator.

- Web: https://apps.schimpf.es/dyslexia-reader-android/reading-time-calculator/
- App: Dyslexia Reader: Book Reader, https://apps.schimpf.es/dyslexia-reader-android/index.md
You can get a good estimate of reading time with one division. This page shows the formula, three worked examples and a calculator you can use right here.

## The quick answer

- Assume about 200 words a minute.
- A word counts as six characters: five letters and one space.
- That makes 1,200 characters a minute.
- Divide the characters left by 1,200, then round up to whole minutes.

Dyslexic readers often read slower than 200 words a minute, and speed changes with the text. Treat the result as a planning number. If you read at 100 words a minute, double it.

An interactive calculator is on the web page: https://apps.schimpf.es/dyslexia-reader-android/reading-time-calculator/

## The formula

minutes left = ceil( (total characters - characters already read) / 1,200 )

- Total characters counts letters, digits, punctuation and spaces.
- Characters already read is where you stopped.
- ceil rounds up. Even 1 character left shows as 1 minute.
- If you have finished the book, the result is 0.

If you only know the word count, multiply it by 6 to get characters.

characters = words x 6

This is an average for English text. Books with many short words come out a little high, and books with long words a little low. Over a whole book the error is usually small.

## How to find the word count

- A TXT file: open it in a word processor and read the count in its status bar.
- A word processor document: use its word count tool.
- A published book: the publisher page often lists it. Otherwise, estimate from pages. A paperback page holds about 250 to 300 words.
- In Dyslexia Reader Android, you do not need the count. The import screen shows the size of the text and the time to read it before you add the book.

## Percent read

Progress is the characters read divided by the total, times 100, rounded down.

percent = floor( characters read x 100 / total characters )

Rounding down means you only see 100% when you have really reached the end.

## Worked examples

### A 90,000-word novel

1. Characters: 90,000 x 6 = 540,000.
2. Minutes: 540,000 / 1,200 = 450.
3. 450 minutes is 7 hours 30 minutes.

### A short story, partly read

You have a text with 54,000 characters and you stopped at character 20,000.

1. Characters left: 54,000 - 20,000 = 34,000.
2. Minutes: 34,000 / 1,200 = 28.33. Round up to 29 minutes.
3. Progress: 20,000 x 100 / 54,000 = 37.03. Round down to 37%.

### Almost done

You have 1,000 characters left.

1. 1,000 / 1,200 = 0.83.
2. Round up: 1 minute.

## Quick table

Each row uses the 200 words a minute rule.

| Words | Characters | Reading time |
|---|---|---|
| 5,000 | 30,000 | 25 min |
| 20,000 | 120,000 | 1 h 40 min |
| 50,000 | 300,000 | 4 h 10 min |
| 90,000 | 540,000 | 7 h 30 min |
| 120,000 | 720,000 | 10 h |

## Fit it to your own speed

To use your own pace, divide the words by your words per minute instead of 200.

1. Read a page you know the word count of for one minute.
2. Count the words you read. That is your pace.
3. Divide the book's words by that number.

Example: a 60,000-word book at 120 words a minute is 60,000 / 120 = 500 minutes, or 8 hours 20 minutes.

## Where the app does this for you

Dyslexia Reader Android works out this number for every book in your library. It uses the same 1,200 characters a minute rule and the same rounding. You see the progress and the time left on each book and in the reader. A home-screen widget shows the same for the book you are reading and takes you back to your place.

- Import TXT, EPUB or PDF files from your device.
- Everything stays on your device. The app has no internet permission.
- A short sample book is included so you can see the numbers before you add your own.

Search for Dyslexia Reader: Book Reader on Google Play.
