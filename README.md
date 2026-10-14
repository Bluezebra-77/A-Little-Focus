# A Little Focus · v1.6

*One theme. Six ideas. Your pace.*

## What is included

- Daily, Weekly and Monthly choices at the top of the page.
- 365 unique daily themes, each with six approaches and a shooting guide.
- Weekly holds a theme for seven days; Monthly holds one until the same date next month (or the last available date in a shorter month). Each brief shows its date range. The last period is shortened at the end of the 365-day challenge.
- All paces use one saved schedule. Switching does not reset it, photos or completion. If a theme appears in more than one pace, its saved photo and completion are shared. Weekly and Monthly draw from the same 365-theme set.
- Add a photo or screenshot from your phone. A gallery lets you return to each photo's brief.
- Install on iPhone or Android. No ChatGPT login or connection is required.

## Upload to your a-little-focus repository

1. Download and unzip this package.
2. Open the `a-little-focus` repository you have created.
3. Choose Add file → Upload files. Upload the extracted app files, not the ZIP. `index.html` must be in the repository root, alongside the other files. Commit the upload.
4. Open Settings → Pages. Choose Deploy from a branch → main → /(root) → Save.
5. Wait for GitHub to display the website address, then open it and share that link.

Use a NEW repository so you do not overwrite the planner. If you use an existing repository instead, keep this app together in its own subfolder and confirm its Pages publishing folder first.

## Install the mini app

On iPhone: open the live URL in Safari → Share → Add to Home Screen. Choose Open as Web App if offered.
On Android: open in Chrome → Install app / Add to Home screen. A supported browser may also show the Install app button inside the app.
The app opens with its own icon and app-style window. Briefs and saved photos work offline after one online visit.

## Photo storage and backup

Every person's photos stay in their own device/browser profile. There is no shared photo server, login or automatic cross-device syncing. People sharing the same browser profile share that local collection. Safari and a Home Screen app may use separate storage, so transfer using a full backup if needed.

The saved photo copy is at most 1,600 pixels on its longest edge and 200 KB. A separate gallery thumbnail is at most 320 pixels and 16 KB. The original is untouched. Progress and automatic recovery contain references; actual photos and thumbnails are kept separately in IndexedDB image storage, away from the small localStorage allowance. No image bytes are stored in localStorage.

Seven daily recovery snapshots reuse unchanged images, rather than duplicating every image seven times. Older photo versions are kept while a recovery copy needs them. Full Export/Share backups contain progress, pace, schedule, actual photographs and thumbnails in separate ZIP entries. Import restores all of these, keeping a pre-restore safety copy. v1.3 photo backups and original JSON progress backups can also be imported.

Separate image storage STILL uses Safari/device space. A full current collection is at most approximately 77 MiB with thumbnails, plus recovery versions and app files. Safari may clear data when site storage is cleared or space is constrained. Request persistent storage is available, but may be declined. Keep an independent full backup in Files, iCloud Drive or another safe location. Backups do not automatically upload to iCloud.

## Add to a future website

Link to the GitHub app from your website, or host these same files in a folder on your future HTTPS website. All paths are relative. Export a full backup before changing domains, then import it at the new address; browser data does not automatically travel with the code. Linking/opening the app directly is preferable to embedding it in an iframe, because some browsers restrict embedded storage and Home Screen installation.

## Test before sharing widely

Switch between the three paces and reopen: each current brief should stay fixed. Add a screenshot/photo, mark complete, view it in the gallery and return to its brief. Close/reopen the app. Export a full backup, import it on another browser/device, and check the actual photo opens. Install on Home Screen and test offline after one online visit.

Automated checks cover cadence boundaries, month-end/leap dates, fixed/reproducible schedules, mode switching, seasonal ordering, full photo-and-thumbnail backup roundtrips, old backups, damaged backup rejection, seven-day recovery and simulated storage failures. JavaScript and GitHub subfolder paths are checked. Real iPhone/Android installation and IndexedDB behaviour still need device testing.


This release updates the app heading, tagline, browser title, Home Screen name and backup filenames. Saved progress, photos and previous backups remain compatible.


## Update the existing repository to v1.6

Export a full backup from the app first if you have added test photos. Unzip this package, open your a-little-focus repository, choose Add file → Upload files, and upload ALL the extracted files to the existing repository root. Commit changes. GitHub Pages redeploys automatically. Refresh the live site and check Version 1.6 at the bottom.

The chosen smiling blue zebra (option 5) is used in the app header, browser tab, Apple Home Screen icon and Android installation icons. Separate Android maskable artwork includes safe margins. The previous icon files can remain unused in the repository; they do not need deleting. Photos, schedule, progress and backup compatibility are retained.

iOS may keep an already installed Home Screen icon until it refreshes. Do not clear browser data to update an icon. If reinstalling later, keep a full exported backup first, then verify the photo collection after restoration.
