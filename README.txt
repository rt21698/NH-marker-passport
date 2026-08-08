NH Historical Marker Passport v11 — Structured Database Foundation

WHAT CHANGED
- Marker records moved out of index.html into markers.json.
- Day-trip route definitions moved into trips.json.
- The app now loads both data files dynamically.
- Existing completion progress, notes, favorites, competition scores, and selfie storage remain unchanged.
- PWA offline cache now includes markers.json and trips.json.

DATABASE FIELDS
Each marker record can now hold:
- marker number
- official title
- town
- region
- county
- status
- latitude / longitude
- official marker text
- source note
- title_verified
- location_verified

CURRENT VERIFICATION STATUS
- 207 / 291 marker titles currently have non-placeholder titles.
- 31 / 291 marker records currently have exact coordinates in the database.
- All 1–291 numbers remain represented.
- Retired / repair / construction statuses remain excluded from active completion totals.

WHY THIS MATTERS
From this version forward, a title correction or GPS update only requires editing markers.json.
The same database can power:
- interactive map pins
- distance calculations
- true route optimization
- nearest-marker recommendations
- official marker history pages

UPLOAD
Upload ALL files from this version to the ROOT of the same GitHub repository:
- index.html
- markers.json
- trips.json
- manifest.json
- icon.svg
- service-worker.js
- README.txt

Replace older files when prompted.
