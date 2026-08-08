NH Historical Marker Passport v16.4 — Exact Apple Maps Pin Fix

WHY THIS PATCH EXISTS
Recent Apple Maps behavior can change a raw daddr=latitude,longitude directions
destination to a nearby named place. Turkey Pond #184 exposed the problem even
though the NH DHR coordinate itself was correct.

APPLE MAPS FIX
- "Open Exact Pin" now uses Apple's documented ll=latitude,longitude map-pin format.
- It does NOT use daddr for coordinate navigation.
- It does NOT search for the marker title/place.
- Apple Maps opens the official DHR coordinate as a pin.
- From that pin, tap Directions and then Go in Apple Maps.

ONE-TAP FALLBACK
- "GPS Directions" uses Google's universal directions URL with the raw
  latitude/longitude as the destination.
- This can open Google Maps if installed, or Google Maps on the web otherwise.

WHY TWO STEPS IN APPLE MAPS?
Apple's current URL directions handling may snap coordinate destinations to nearby
mapped entities. Opening an ll coordinate pin avoids that resolution step and preserves
the exact location.

OTHER FEATURES
- iPhone Photo Library picker from v16.3 remains included.
- Adventure Mode, Near Me, statewide map, official DHR data, progress, notes,
  selfies, favorites, and competition tracking remain compatible.
- #281 still uses its written-location fallback because the state's published
  longitude is malformed.

UPLOAD
Upload all files from this ZIP to the root of your existing GitHub repository and
replace the older files.
