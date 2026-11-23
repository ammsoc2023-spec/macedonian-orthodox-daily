# Macedonian Orthodox Daily

Static PWA of the daily Orthodox calendar app.

Live site: https://ammsoc2023-spec.github.io/macedonian-orthodox-daily/

## Updates
The app updates itself: every deploy changes `sw.js`/`version.json`, and the open or home-screen app picks the new
version up on its next start or return to the foreground (it waits if read-aloud is playing). Deploy = rebuild
`sw.js` + `version.json` with the app's `mksw.py` (bumps the cache name automatically), then push to `main`.
