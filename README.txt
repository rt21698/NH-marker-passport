NH Historical Marker Passport v16.1 — Exact GPS Navigation Fix

WHY THIS PATCH EXISTS
Apple Maps was resolving some navigation links by marker/place name instead of strictly using the official NH DHR coordinate.
Turkey Pond (#184) exposed the issue: the DHR coordinate was correct, but Apple Maps navigated toward Turkey Pond itself rather than the roadside marker.

FIX
- Valid markers now send Apple Maps ONLY the raw latitude/longitude as the destination.
- Marker title/name is no longer included in the directions URL.
- Added a separate "View Exact Pin" button so you can inspect the raw coordinate before starting navigation.
- The malformed official coordinate for #281 still falls back to the official written location instead of using bad GPS data.
- Existing progress, selfies, notes, favorites, scores, Near Me, Map, and Adventure Mode remain compatible.

RECOMMENDED WORKFLOW
1. Tap View Exact Pin to sanity-check the roadside location.
2. Tap Navigate Exact GPS to start Apple Maps directions to the raw DHR coordinate.

UPLOAD
Upload all files from this ZIP to the root of the existing GitHub repository and replace older files.
