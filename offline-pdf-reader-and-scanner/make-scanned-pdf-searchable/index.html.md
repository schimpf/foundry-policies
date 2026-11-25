# How to Make a Scanned PDF Searchable on Android

> Why a scanned PDF cannot be searched, how OCR adds a hidden text layer, and how to turn a scan into a searchable PDF on your phone.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/make-scanned-pdf-searchable/
- App: PDF Reader & Scanner, https://apps.schimpf.es/offline-pdf-reader-and-scanner/index.md
You scan a contract, open it, type a word into search and get "no matches". The page shows words, yet the file holds only a picture of them. This page explains why, how to check it, and how to fix it on Android without uploading the file anywhere.

## Why a scanned PDF has no searchable text

A PDF page can hold two kinds of content:

- **Text objects.** Real characters with a font and a position. Search, copy and highlight all work on them.
- **Images.** A photo of a page. Your eyes read the words, but the file has no characters at all.

A camera scan produces only an image. A PDF exported from Word or a web page usually has real text. So search fails on scans and works on documents made on a computer.

## How to check if your PDF has a text layer

1. Open the PDF in a reader.
2. Search for a word you can see on the page.
3. Try to select a line with a long press.

If search finds nothing and you cannot select text, the page is image-only.

## What OCR does

OCR means optical character recognition. The software looks at the picture, finds lines of text and works out which characters they are. It then writes those characters into the PDF as an invisible layer on top of the image.

- The page looks exactly the same.
- Search, copy and highlight now work on the page.
- The original image stays in the file.

Accuracy depends on the scan. Sharp, flat, well-lit pages with printed text give the most accurate results. Blurry photos, shadows, handwriting and unusual fonts give more mistakes.

## Make a scan searchable with Offline PDF reader and scanner

The app runs text recognition on your phone with the bundled Google ML Kit Latin model. Nothing is uploaded, and the app has no internet permission. Text recognition is a Pro feature (a one-time purchase).

### Option 1: automatically after each scan

1. Open **Settings** and check that **Make scans searchable** is on. It is on by default once Pro is unlocked.
2. Tap **Scan document** on the home screen.
3. Scan the pages and tap **Save scan**.
4. Text recognition starts after saving. Progress shows on the scan's row in the library.

The result replaces the scan, so you keep one file per scan.

### Option 2: a PDF you already have

1. Open the image-only PDF in the reader.
2. Search for a word. The app tells you there is no text layer and asks if you want to make it searchable.
3. Confirm. The app starts text recognition.

For an imported PDF, the app saves the result as a library copy named "(searchable)". The original file is not changed.

### Option 3: after adding pages

When you add pages to a saved scan in the page editor, the new pages get text recognition too. Saving replaces the scan.

## What happens during recognition

- Each page is rendered at 2480 pixels wide. For an A4 page that is about 300 dpi, a common resolution for OCR.
- The Latin-alphabet model reads each page and returns lines of text with their positions.
- The app writes all lines into the PDF as invisible text, then replaces the file once.
- It runs as normal background work. You can leave the app while it finishes.
- If it takes longer than 30 minutes or fails, the scan is marked as failed. The file stays as it was.

Long documents take longer, because every page is processed one at a time.

## Limits to know about

- **Latin alphabet only.** English, German, Spanish and other languages written in Latin letters work. Cyrillic, Greek, Arabic, Chinese, Japanese and Korean are not supported.
- **Pro only.** Reading, plain scanning and search in PDFs that already have text do not need Pro.
- **Google Play services.** Scanning and Pro need them. Reading PDFs works without them.
- **Check important numbers.** OCR can misread a 5 as a 6. Compare amounts, dates and IDs against the page.

## After recognition: search and highlight

Once a page has a text layer you can:

1. Tap the search icon in the reader and type a word.
2. Use the next and previous buttons to jump between matches.
3. Long-press and drag over text to highlight it. Highlights are standard PDF annotations, so other readers show them. The app saves them as a copy in your library and never changes the original.

## Questions

### Does OCR make the file bigger?

A little. The text layer is small compared with the page images.

### Can I search before OCR?

No. Without a text layer there is nothing to search. Run recognition first.

### Is my scan sent to a server?

No. Recognition runs on the phone, and the app has no internet permission.

## Try it

Offline PDF reader and scanner is on Google Play. Scan a page, wait for recognition to finish and search for a word on it.
