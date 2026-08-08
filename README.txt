NH Historical Marker Passport v16.5 — Stable GPS Fix

This version was rebuilt from the last known-working v16.3 photo-picker build.

FIX
- Restores all buttons/tabs/click behavior.
- Keeps the iPhone Photo Library picker.
- Marker navigation opens the official NH DHR latitude/longitude as an Apple Maps exact pin using ll=lat,lon.
- No directions URL, place-name search, Google fallback, or extra navigation JavaScript was added.
- Once Apple Maps opens on the exact pin, tap Directions and then Go.
- #281 continues to use the written-location fallback because its published longitude is malformed.

QUALITY CHECK
The app JavaScript was syntax-checked before packaging.

Upload all files in this ZIP to the root of the existing GitHub repository and replace the older files.
