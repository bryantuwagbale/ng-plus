# climb

A 15 lb fat loss and strength recovery run, framed as a ranked climb back to a former peak. No build step, single-file PWA, deployed on GitHub Pages.

## What this is

The user hit Diamond before (peak lifting strength, a 2-plate squat) and dropped out of ranked. This app isn't a new account, it's the climb back. Every day resolves into one match result:

| Result | Requirement | LP |
|---|---|---|
| S-Tier | Floor + lift session + 7,000 steps | +30 |
| Autopilot | Floor: 2,000 steps, protein at lunch, home-cooked dinner | +15 |
| Loss | Floor not completed | -20 |

100 LP promotes a division. The ladder runs Iron through Diamond (4 divisions each), then Master, Grandmaster, Challenger, uncapped. Start position is Silver IV, so there's room to fall. Doing nothing is a Loss, silence is the worst outcome on the board.

Two "Loss Mitigated" tokens per month turn a bad day into a no-match: 0 LP change, no demotion, streak intact.

## Structure

- `index.html` — the entire app. All markup, styles, and logic in one file, no bundler, no dependencies.
- `manifest.json` — PWA manifest, installable on iOS/Android as a home screen app.
- `sw.js` — service worker, network-first with cache fallback for offline use.
- `icon-*.png` — app icons.

## Tabs

- **Today** — weigh-in, rank card, the Floor checklist, Loss Mitigated
- **Food** — kitchen rules, meal log, Sunday batch cook tracker, grocery list, standing orders
- **Lift** — Friday/Saturday sessions, 30-minute session clock with 90-second rest timers between lifts, squat ladder (+10 lb per session, deloads to 85% after two stalls)
- **Matches** — calendar history, color-coded by day result, tap any day to backfill or edit
- **Rank** — weight trend (7-day rolling average), waist tracking, the full ladder, export/import/reset

A "?" in the header runs a guided tour that navigates to and highlights each section.

## Data

Everything lives in `localStorage` under the key `climb.v1`. No backend, no account, no sync between devices. Export/import JSON from the Rank tab (Reset Account section) to move data or back it up.

## Deploying

Push to `main`, GitHub Pages serves straight from the repo root. No build step. If you rename the repo, update your home screen install afterward, the PWA's `start_url`/`scope` are tied to the URL.
