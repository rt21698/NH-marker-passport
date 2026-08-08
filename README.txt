NH Historical Marker Passport v17.7 — MAP ALIGNMENT FIX

WHAT WAS WRONG
The NH DOT map image requested in v17.5/v17.6 was 720 x 1240 pixels, but the requested
longitude/latitude bounding box has a very different aspect ratio. ArcGIS adjusted the
display extent to fit that tall image. The marker projection still used the original
bbox, which is why many southern markers appeared below New Hampshire.

FIX
- NH DOT boundary image is now requested at 720 x 924, matching the geographic bbox ratio.
- SVG map is 360 x 462 with the same ratio.
- Marker projection uses exactly the same bbox and dimensions as the boundary image.
- Coordinates outside the NH extent are not drawn as valid map pins.

DATA CHECK
Found 1 malformed/out-of-state coordinate record(s) in the current marker data:
- #281 THE BROKEN 1713 TREATY OF PORTSMOUTH: lat 43.06094585, lon 43.06094585

All other v17.6 features remain.

Keep service-worker.js deleted.
Upload:
index.html
markers.json
trips.json
manifest.json
README.txt
