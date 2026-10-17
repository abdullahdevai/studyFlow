SubjectFlow PWA
================

Files:
- index.html: app UI and application logic
- manifest.json: install metadata and app icons
- sw.js: offline app-shell caching
- icons/: 192px and 512px app icons

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
Use Export to make a backup. In the app, right-click Export to import a JSON backup.
