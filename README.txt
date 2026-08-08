NH Historical Marker Passport v17.4 — Road Miles + Custom Names

ROAD DISTANCE
- Trip cards no longer rely on displayed straight-line mileage.
- Tap "Calculate Road Miles" on a trip to get actual road-network distance and estimated drive time between each stop.
- Near Me can calculate road distance from your current location to an individual marker.
- Road distance uses OSRM routing with OpenStreetMap road data.
- It is on-demand because the public routing service can be unavailable or rate-limited.
- Apple Maps still handles actual navigation, traffic, road closures, and turn-by-turn directions.

CUSTOM MARKER NAMES
- Every passport entry now has an optional Custom Marker Name field.
- Your custom name is stored locally with your progress.
- The custom name becomes the main display name in trips, map, nearby results, etc.
- The official NH DHR title remains visible underneath as "Official DHR title."
- Leaving the field blank restores the official title.
- Official markers.json data is never overwritten.

OTHER
- Interactive map, selfies on visited markers, Not Found status, condensed 29 trips, exact Apple pins, photo uploads, notes, favorites, and competition tracking are retained.
- No service worker is included. Keep service-worker.js deleted.

Upload:
index.html
markers.json
trips.json
manifest.json
README.txt
