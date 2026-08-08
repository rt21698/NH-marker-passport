NH Historical Marker Passport v17.6 — STARTUP FIX

IMPORTANT FIX
v17.4/v17.5 accidentally lost four JavaScript functions during the road-mileage edit:
- locate()
- roadMilesFromCurrent()
- buildAdventure()
- init()

Because init() was missing, markers.json and trips.json were never loaded. That caused:
- 0 active markers
- "Loading..." forever
- empty Passport/Trips/Map data
- Near Me and Adventure not functioning

v17.6 restores those functions and retains:
- Real NH map with faint town boundaries
- Different status pin shapes/colors
- Visited/unvisited/not-found/unavailable markers
- Selfies on map details
- Custom marker names
- Road-network mileage
- Condensed trips
- Exact Apple Maps coordinates
- Not Found tracking
- Notes, dates, favorites, competition score

Keep service-worker.js deleted.
Upload all five files:
index.html
markers.json
trips.json
manifest.json
README.txt
