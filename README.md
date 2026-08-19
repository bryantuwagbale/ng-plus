# New Gains+

Fat loss and strength tracker. Single-file HTML PWA. No build step, no dependencies, no backend.

## Files

Replace everything in the repo root with these:

| File | What it is |
|---|---|
| `index.html` | The entire app. All logic, styles, and markup. |
| `manifest.json` | PWA metadata so it installs as a real app |
| `icon-180.png` | iOS home screen icon |
| `icon-192.png`, `icon-512.png` | Android / PWA icons |
| `icon-maskable-512.png` | Android adaptive icon, extra padding for circle masking |
| `favicon.png` | Browser tab icon |

## Deploy

1. Drop all files in the root of the `ng-plus` repo.
2. Commit and push. GitHub Pages serves it at `bryantuwagbale.github.io/ng-plus`.
3. On iPhone: open in Safari, hard refresh, Share > Add to Home Screen.
   Delete the old icon first. iOS caches icons and meta tags aggressively.

## Data

Everything lives in `localStorage` under `ngplus.v3`. Export and import JSON is under Attributes > Rebirth. That is the only way to move data between devices.

Clearing Safari website data wipes it. Export before doing anything drastic.

## The day

- **Morning, after brushing teeth:** weigh in. The number is hidden until Sunday.
- **During the day:** tap the three Floor boxes as they happen.
- **Anything above the Floor** is upside, not obligation.
- **Bad day:** hit the Floor and stop. No making it up. If the day is gone, spend a flask.
- **Sunday:** the Site of Grace. Runes vs last week, weight average unlocks itself, level up.

The one rule the system exists to protect: **never miss twice.**

## Runes

| Action | Runes |
|---|---|
| Floor (steps, protein at lunch, dinner plated) | 100 |
| Base step target | 100 |
| Stretch step target | 200 |
| Went downstairs to the gym | 150 |
| Lift session, top set logged | 300 |
| Lunch was already made | 100 |
| Dinner plated in the kitchen | 100 |
| Named boss cleared | 500 |

Step targets scale with Endurance, starting at 5,000 / 8,000 and rising 1,000 per level. They move only when you level, never on a calendar.

## Tabs

- **Today** — weigh-in, Floor checklist, rune actions, flask
- **Food** — meal and drink log, kitchen rules, standing orders, grocery list
- **Workouts** — A/B session, log top set, boss ladder
- **Remembrances** — editable calendar, tap any day to backfill
- **Attributes** — weight averages, weekly runes, levels, Rebirth (export/reset)

Tap any `i` for the rules behind that section. The `?` on Today opens the About page and the walkthrough.

## Week one

Use Today and Workouts. Ignore everything else. Add the Crafting Kit (Sunday batch) in week two, weight in week three.
