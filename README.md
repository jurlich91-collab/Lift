# Lift

A single-file workout tracker PWA. Programs, set logging with last-session prefill, PR detection, rest timer, history and progress charts, editable logged workouts, and a meal plan reference tab. All data stays on the phone (IndexedDB); export a JSON backup from Settings.

## Deploy to GitHub Pages
1. Create a new public repo (e.g. `lift`) and upload every file in this folder to the root.
2. Repo Settings > Pages > Source: Deploy from a branch > `main` / `(root)` > Save.
3. After a minute the app is live at `https://<your-username>.github.io/lift/`.

## Install on iPhone
Open the URL in Safari > Share > Add to Home Screen. Launch from the icon so it runs full-screen and keeps its data.

## Updating
Replace `index.html` and `sw.js` in the repo. The `CACHE` name in `sw.js` is bumped each release so phones pick up the new version (open the app, close it fully, open again).

## Changelog
- **1.4.0** — Edit logged workouts (date, start, duration, sets, exercises, cardio). Reorder or remove exercises mid-workout. Meals tab with the cut plan as a table, editable in-app and included in backups. Merge duplicate exercises. Guard against workouts left open overnight.
- 1.3.0 — Cardio type selector, inverted PRs for assisted work, pull-up progression.
