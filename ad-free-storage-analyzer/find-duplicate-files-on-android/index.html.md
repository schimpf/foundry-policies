# How to Find Duplicate Files on Android

> How to find exact duplicate files on an Android phone, how checksums prove two files are the same, and which copy to keep when you delete.

- Web: https://apps.schimpf.es/ad-free-storage-analyzer/find-duplicate-files-on-android/
- App: Storage Analyzer: Big Files, https://apps.schimpf.es/ad-free-storage-analyzer/index.md
Duplicate files quietly fill a phone. The same video is saved twice, a download is repeated, or a photo is copied into two folders. This page shows how to find exact duplicates, how to be sure they are real copies, and how to delete them without losing anything.

## What counts as a duplicate

An exact duplicate has the same content, byte for byte. It can have a different name, a different folder, or a different date. Two photos that only look alike are not exact duplicates, because their bytes differ.

Matching by name is unreliable. Two files named `IMG_0042.jpg` can be different photos, and one video saved as `clip.mp4` and `clip (1).mp4` is the same file under two names. Content is what counts.

## Step by step: find duplicates by hand

1. Open a file manager and go to the folder you suspect, such as Downloads.
2. Sort by size, largest first.
3. Look for files with exactly the same size in bytes. Open the file details to see the exact number.
4. Open both files and compare them.
5. Delete the copy you do not need.

This works for a few files. It gets slow with hundreds. It also cannot prove that two files with the same size are identical, because different files can share a size.

## How a checksum proves two files match

A checksum is a short fingerprint calculated from every byte of a file. SHA-256 is a standard hash function (NIST, *FIPS PUB 180-4: Secure Hash Standard*, 2015). It gives a 64-character result, such as `9f86d081…`.

- Identical files always give the same SHA-256.
- If one byte differs, the result is completely different.
- Two different files giving the same result is not a practical concern.

Reading every byte of a large file takes time, so a good scanner does it in two steps:

1. **Group by size.** A file with a size no other file has cannot be a duplicate. Those are skipped.
2. **Hash only the groups.** Files with the same size get a SHA-256 over the full file. Same result means exact copy.

### Worked example

Your phone has these files:

| File | Size |
|---|---|
| `trip.mp4` | 48,201,330 bytes |
| `trip (1).mp4` | 48,201,330 bytes |
| `lecture.mp4` | 48,201,330 bytes |
| `notes.pdf` | 2,310,004 bytes |

1. `notes.pdf` has a unique size, so it is skipped.
2. The three videos share a size, so each gets a SHA-256.
3. `trip.mp4` and `trip (1).mp4` give the same result. `lecture.mp4` gives a different one.
4. Result: one duplicate group of two files. Deleting one copy gives back 48,201,330 bytes, about 48.2 MB.

## Which copy to keep

Keep the newest copy. It is the one you most likely edited or moved on purpose, and old copies are usually leftovers. If two copies share a date, either one is fine, since the content is the same.

Always keep at least one copy of each group. If you delete all of them, the file is gone.

## Find duplicates with Storage Analyzer

Storage Analyzer finds exact duplicates after you tap Scan. It follows the two steps above:

- Only files of 1 MB (1,000,000 bytes) or more are checked. Small files add little space.
- Files with the same size are compared with SHA-256 over the full file. Only true copies are shown.
- Groups are sorted by the space you would gain, with the biggest first.
- The newest copy is preselected as the one to keep. You can change the choice for each file.
- At least one copy is always kept.
- A file the app cannot read is left out of the results. It is not counted as a copy.

Deleted files move to the app's Trash. You can undo right after deleting, or restore them from Trash for 7 days. After that they are deleted for good. Files are moved on the same storage volume, not copied, so it is fast even for large videos. Uninstalling the app empties its Trash, so restore anything you want first.

The app finds exact duplicates only. Similar photos are not matched.

## Quick checklist

- Same size, then same checksum, means same file.
- Keep the newest copy.
- Check the group before you delete.
- Use Trash first, and empty it later.
