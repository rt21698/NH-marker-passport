NH Historical Marker Passport v13 - OFFICIAL NH DHR DATABASE REBUILD

SOURCE OF TRUTH
This version rebuilds all 291 marker records directly from the two uploaded
New Hampshire Division of Historical Resources inventory PDFs dated February 19, 2025:
- highway-markers-by-number.pdf
- highway-markers-by-town.pdf

OFFICIAL FIELDS NOW STORED FOR ALL 291 MARKERS
- marker number
- official inventory title
- town
- written roadside location
- official status
- GPS north / west coordinates
- source metadata

QUALITY CHECKS
- 291 / 291 marker numbers parsed with no gaps.
- Both PDFs were cross-checked for GPS and status agreement.
- 290 / 291 published coordinate pairs pass a New Hampshire geographic sanity check.
- #281 has a malformed positive GpsWest value in BOTH official PDFs. The value is preserved
  as published and flagged; Apple Maps falls back to the official written location for that marker.
- County is left blank because these inventory PDFs do not provide county.
- Full inscription text is left blank because these inventory PDFs provide inventory titles/locations,
  not the full historical marker inscription.

OFFICIAL STATUS COUNTS
- INSTALLED: 282
- OUT FOR REPAIR: 4
- REMOVED FOR CONSTRUCTION: 1
- RETIRED: 4

APP CHANGES
- Marker cards now show the official roadside location.
- Apple Maps uses official GPS coordinates when valid.
- Invalid official coordinates use the official written location instead.
- Previous checkoffs, selfies, notes, favorites, and competition scores remain compatible.

UPLOAD ALL FILES FROM THIS ZIP TO THE ROOT OF YOUR EXISTING GITHUB REPOSITORY.
