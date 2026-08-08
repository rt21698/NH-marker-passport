NH Historical Marker Passport v16.3 — iPhone Photo Picker Fix

WHY
The prior version removed the HTML camera-capture attribute, but iOS can still behave differently when a hidden file input is opened by JavaScript.

FIX
- The app no longer programmatically clicks the photo input.
- "Choose Selfie from Photos" is now a native HTML file-picker label tied directly to the image input.
- No capture/camera attribute exists anywhere in the app.
- Image types are limited to common photo-library formats.
- On iPhone, iOS may still display its own system menu. Choose "Photo Library" there.
- A website cannot force iOS to skip Apple's system picker menu entirely.

Existing photos, progress, notes, navigation, map, Near Me, and Adventure Mode remain compatible.

Upload all files from the ZIP to the root of the existing GitHub repository and replace the older files.
