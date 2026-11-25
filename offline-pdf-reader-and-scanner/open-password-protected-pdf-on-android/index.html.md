# Open a Password-Protected PDF on Android

> Why a PDF asks for a password, which Android versions can open it, what to do when it fails, and the difference between the two PDF passwords.

- Web: https://apps.schimpf.es/offline-pdf-reader-and-scanner/open-password-protected-pdf-on-android/
- App: PDF Reader & Scanner, https://apps.schimpf.es/offline-pdf-reader-and-scanner/index.md
You tap a PDF and it asks for a password, or it will not open at all. Whether you can open it depends on the password and on your Android version. This page covers both.

## Two kinds of PDF password

The PDF specification (ISO 32000-1:2008, section 7.6, and ISO 32000-2:2020 for PDF 2.0) defines two passwords:

| Password | What it does |
| --- | --- |
| **User (open) password** | Needed to open the file and read it. |
| **Owner (permissions) password** | Sets limits such as no printing or no copying. The file opens without it. |

A reader asks you for a password only when the file has a user password. The sender chose it. Nobody can read it back from the file, and the app cannot recover a lost one.

## Which Android versions can open them

In Offline PDF reader and scanner, the answer depends on the system PDF engine:

| Android version | Password-protected PDF |
| --- | --- |
| Android 15 (API 35) and newer | Opens after you enter the password |
| Android 14 (API 34) and older | Not supported. The app shows a message. |

On older versions the app tells you "Password PDFs need Android 15" and explains that the device cannot open them. It does not guess or try to work around it.

## How to open one on Android 15 or newer

1. Open the PDF from your files, an email attachment or a cloud app. Use **Open with** and choose the app, or pick it from inside the app.
2. A dialog says **Password required**.
3. Type the password and tap **Open**.
4. If it is wrong, the app says **Wrong password**. Try again.

Passwords are case-sensitive. Check for a trailing space if you copied it from a message.

## If you do not have the password

- Ask the sender. Banks, employers and government offices often use a rule such as a date of birth or a customer number. Their email or letter usually says which.
- Do not look for password-cracking tools for files that are not yours. Many of them are unsafe, and opening someone else's protected file may be illegal.
- If the file is yours and the password is lost, the original source (for example your bank portal) can usually give you a new copy.

## If it fails on an older Android version

You have three choices:

1. Update the phone to Android 15 if the maker offers it.
2. Open the file on a computer, where most PDF readers accept a password.
3. Ask the sender for a copy without a user password, if the content is not sensitive.

## What else works once the file is open

- Continuous vertical scrolling and resuming at the last page.
- The table of contents, if the file has one.
- Text search, if the PDF has a text layer. If it is a scan, text recognition (Pro) adds one.
- Night pages, which invert page colors for reading in the dark.

The app saves where you stopped, so you can come back later. Recent files only remember where a PDF is. The app does not upload or change the original, and you can clear the recent list in Settings.

## Privacy of protected files

Opening happens on the device. The app has no internet permission, so the file and the password you type are not sent anywhere.

## Questions

### Why does the same PDF open in my browser but not here?

Some browsers and desktop readers bring their own PDF engine. On Android, the app uses the system engine, which supports passwords from Android 15.

### Does the owner password stop me from reading?

No. A file with only an owner password opens without a prompt. The limits apply to actions such as printing.

### Does the app remove the password?

No. It only opens the file so you can read it.

## Try it

Offline PDF reader and scanner is on Google Play. Open a protected PDF and enter the password.
