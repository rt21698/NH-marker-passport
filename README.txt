NH Historical Marker Passport v19 — SHARED SELFIES

SUPABASE
Project:
https://rbeuouarrcirvsbocxgc.supabase.co

The browser uses the Supabase publishable key only. No database password or secret/service key is included.

NEW SHARED FEATURES
- First-run team picker: Our Team or In-Laws.
- Live score for both couples.
- Scores update from shared Supabase marker_progress records.
- Realtime subscription updates both phones when either team changes a marker.
- Shared statuses:
  visited
  unvisited
  visited site / marker not found
  visit date
  notes
  custom marker name
- Live recent-activity feed.
- Map mode: My Team / Other Team / Both Teams.
- Both-team map colors:
  green = this phone's team
  purple = other team
  gold = both teams visited
  orange X = checked/not found
  hollow = neither
  warning triangle = officially unavailable
- Tap a map pin to see both teams' status side-by-side.
- One-time importer brings existing local iPhone passport progress into the selected Supabase team.

PHOTOS
Selfies now upload to the public Supabase Storage bucket marker-selfies and photo_url is saved in marker_progress.
Photos are compressed in-browser before upload. Existing local IndexedDB selfies are migrated when importing this phone's progress.
Map marker details can show both teams' shared selfies. Replacing a selfie overwrites that team/marker object.
Removing a selfie clears photo_url from shared progress; the old Storage object may remain because DELETE access is not required for this version.

IMPORTANT
The existing database policies are intentionally simple for this private family challenge.
They allow the browser publishable key to read/write marker_progress. A later login/security pass can tighten this.

The app still includes:
- zoomable real NH/town-boundary map
- road mileage
- exact Apple Maps pins
- 29 condensed trips
- Near Me / Adventure
- local photo picker
- notes/favorites
- Not Found status

Keep service-worker.js deleted.
Upload:
index.html (use index-v19.html contents)
markers.json
trips.json
manifest.json (use manifest-v19.json contents)
README.txt
