# How to Find Old Unused Files on Android

> Find files you have not changed for more than 90 days: old downloads, screenshots, WhatsApp media and APK installers. See the rules and a worked example.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/find-old-files-on-android/
- App: Storage Analyzer: Big Files, https://apps.schimpf.es/ad-free-storage-analyzer/index.md
Old files pile up in a few predictable places. Downloads you opened once, screenshots you no longer need, chat media, and installer files for apps that are already installed. This page explains where to look, what "old" can mean, and how to clear them safely.

## What "old" means

A file is old when it has not changed for a set time. Android keeps a "last modified" date for every file. Storage Analyzer calls a file old when that date is more than 90 days in the past.

The rule in numbers: 90 days × 24 hours × 60 minutes × 60 seconds × 1,000 milliseconds = 7,776,000,000 ms. A file is old if now minus last modified is larger than that.

### Worked example

Today is 1 November. Check three files:

| File | Last modified | Days ago | Old? |
|---|---|---|---|
| `invoice.pdf` | 15 July | 109 | Yes |
| `setup.apk` | 10 September | 52 | No |
| `meme.jpg` | 3 August | 90 | No, exactly 90 is not more than 90 |

"Last modified" is not "last opened". A file you open often is still old if you never change it.

## Where old files hide

### Downloads

Browsers and apps save here by default. It is the first folder to check.

### Screenshots

Screenshots are made for one moment and rarely used again. They are often stored in a folder named Screenshots.

### WhatsApp media

Chat photos, videos and voice notes are saved in WhatsApp folders. They can grow large over a year.

### APK installers

An APK is an app installer file. After the app is installed, the file is usually not needed any more.

## Step by step: clean up by hand

1. Open a file manager and go to Downloads.
2. Sort by date, oldest first.
3. Check files older than 90 days. Delete what you do not need.
4. Repeat for the Screenshots folder, the WhatsApp folders and any folder with APK files.
5. Before you delete a document you may need again, copy it somewhere safe.

## Find old files with Storage Analyzer

After you tap Scan, the app groups old files for you:

- **Downloads:** old files in the top-level Download or Downloads folder.
- **Screenshots:** old files in any folder named Screenshots.
- **WhatsApp media:** old files in WhatsApp folders, including WhatsApp Business.
- **APK installers:** old installer files (APK, APKS, XAPK and APKM), unless they sit in Downloads, Screenshots or WhatsApp folders, where they go to that group.
- **Other old files:** everything else that is old.

"Other old files" leaves out your own photos, videos and music folders: DCIM, Pictures, Movies, Music, Recordings, Podcasts and Audiobooks. An old holiday photo is not junk. If you want to review those, use the large files list instead.

The home screen shows a reclaimable size. It adds old files, APK installers and every duplicate copy except the newest. Large files do not count, because a large file is not junk by itself.

## Delete without risk

- Deleted files go to the app's Trash. Use the undo option right away, or restore from Trash within 7 days.
- After 7 days the files are deleted for good. The check runs when the app starts and once a day.
- Files are moved, not copied, so deleting is fast.
- Folders are never deleted. Only files are.
- Uninstalling the app also empties its Trash, so restore what you want to keep first.

## Scans are manual

The app scans only when you tap Scan. It never scans in the background. In full mode it uses All files access to check every folder on internal storage and the SD card. In limited mode it looks only at the photos, videos and music that Android shares with apps, so the old files list is smaller.

## Quick checklist

- Old means more than 90 days since last modified.
- Check Downloads, Screenshots, WhatsApp media and APK files first.
- Keep personal photos and music out of the junk pile.
- Delete to Trash first, and empty it later.
