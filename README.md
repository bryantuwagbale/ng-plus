# New Gains+

Single-file HTML PWA. No build step, no dependencies, no backend.

## Deploy

1. Replace `index.html` in the root of the `ng-plus` repo.
2. Commit and push. GitHub Pages serves it at `bryantuwagbale.github.io/ng-plus`.
3. On iPhone: open in Safari, hard refresh, Share > Add to Home Screen.
   If you had an older icon, delete it first. iOS caches meta tags.

## Data

Everything lives in `localStorage` under the key `ngplus.v3`.
Export and import JSON is at the bottom of the Stats tab. That is the only way to move data between devices.

Clearing Safari website data wipes it. Export before you do anything drastic.

## Tabs

- **Today** — Floor checklist, rune actions, cache and streak, flask
- **Food** — meal log, kitchen rules, Sunday batch, standing orders, grocery list
- **Workouts** — A/B session, log top set, boss ladder
- **History** — editable calendar for backfill
- **Stats** — weight averages, weekly runes, levels and stats

Tap any `i` for the rules behind that section.

## Walkthrough

The `?` at the top right of the Today tab runs a 10-step guided tour. It spotlights each part of the app in turn and switches tabs as it goes. It runs itself once on first launch, then never again unless you press the `?`.

## Week one

Use the Today tab and the Workouts tab. Ignore everything else.
Add the Sunday batch in week two. Add weight entry in week three.
