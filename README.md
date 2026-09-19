# Lift

A single-file workout tracker PWA. Programs, set logging with last-session prefill, PR detection, rest timer, history and progress charts. All data stays on the phone (IndexedDB); export a JSON backup from Settings.

## Deploy to GitHub Pages
1. Create a new public repo (e.g. `lift`) and upload every file in this folder to the root.
2. Repo Settings > Pages > Source: Deploy from a branch > `main` / `(root)` > Save.
3. After a minute the app is live at `https://<your-username>.github.io/lift/`.

## Install on iPhone
Open the URL in Safari > Share > Add to Home Screen. Launch from the icon so it runs full-screen and keeps its data.

## Updating
Replace `index.html` in the repo. Bump `CACHE` in `sw.js` (v1 -> v2) so phones pick up the new version.
