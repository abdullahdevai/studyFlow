SubjectFlow PWA
================

Files:
- index.html: app UI and application logic
- manifest.json: install metadata and app icons
- sw.js: offline app-shell caching
- icons/: app icons (192, 512, maskable 512, Apple 180)
- screenshots/: images shown in the Android install dialog

Run locally:
1. Extract the ZIP.
2. Open a terminal in the extracted subjectflow-pwa folder.
3. Run: python -m http.server 8000
4. Open http://localhost:8000 in Chrome or Edge.
5. Use the browser's Install app option (or the install icon in the address bar).

For installation on a phone or public hosting, deploy the folder to an HTTPS website.
Opening index.html directly as file:// will not enable service-worker/PWA installation.

Data:
Subject data is stored in this browser's Local Storage. It is not synced across devices.
Use ⋯ → Back up to save a JSON backup (on phones this opens the share sheet,
so you can save it to Drive or send it to yourself). ⋯ → Restore loads one.
The app reminds you if you haven't backed up in 7 days.

Install on a phone:
- Android (Chrome): open the HTTPS site, tap "Install" on the banner or in the ⋯ menu.
- iPhone/iPad (Safari): tap Share, then "Add to Home Screen".
After a new deploy, the installed app picks up the new version on its next launch.
