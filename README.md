# Lift

A single-file workout tracker PWA. Programs, set logging with last-session prefill, PR detection, rest timer, history and progress charts, editable logged workouts with comments, a daily log (weigh-in, meal tickboxes, comments) and the meal plan. All data stays on the phone (IndexedDB); export a JSON backup from Settings.

## Deploy to GitHub Pages
1. Create a new public repo (e.g. `lift`) and upload every file in this folder to the root.
2. Repo Settings > Pages > Source: Deploy from a branch > `main` / `(root)` > Save.
3. After a minute the app is live at `https://<your-username>.github.io/lift/`.

## Install on iPhone
Open the URL in Safari > Share > Add to Home Screen. Launch from the icon so it runs full-screen and keeps its data.

## Updating
Replace `index.html` and `sw.js` in the repo. The `CACHE` name in `sw.js` is bumped each release so phones pick up the new version (open the app, close it fully, open again).

## Changelog
- **1.8.0** — Diagrams for every mobility exercise and level (start and end positions, what to feel, kit variants), a full illustrated library of the stretches and extras, and a demo-search button on each step.
- **1.7.1** — Dinner yoghurt halved to 90 g.
- **1.7.0** — 1.5.1 meal plan yields merged with the Mobility tab (1.5.1 and 1.6.0 were built in parallel).
- **1.6.0** — Mobility tab: guided nightly stretch, activation and light calisthenics routine with progression ladders, pain check-ins and knee-to-wall re-tests.
- **1.5.1** — Meal plan updated with weighed yields: 670 g chicken meat and 670 g cooked mince per batch, each split into 4.
- **1.5.0** — New Daily tab: morning weigh-in with 7-day average and 4-week chart, tick off each meal from the plan (training-only meals and swaps handled), "Ate as planned" button, and a comments box per day. Comments box on every workout (also editable after). Meal plan updated to the Oct 2026 cut plan (old plan kept in the backup as `mealPlanPrev`). Plan format adds a `| train` flag. Weekly export reminder.
- **1.4.0** — Edit logged workouts (date, start, duration, sets, exercises, cardio). Reorder or remove exercises mid-workout. Meals tab with the cut plan as a table, editable in-app and included in backups. Merge duplicate exercises. Guard against workouts left open overnight.
- 1.3.0 — Cardio type selector, inverted PRs for assisted work, pull-up progression.
