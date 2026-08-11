# New Gains+

A daily tracker for fat loss and strength recovery, built around one idea: **adherence beats optimality**.

Live: https://bryantuwagbale.github.io/ng-plus/

Single HTML file, no build step, no dependencies, no account. Saves to your own browser. Installable to the home screen on iOS and Android.

## The idea

Most fitness apps optimize the plan. This one optimizes the odds you actually do it. Every mechanic exists to make a bad day survivable, because a lapse becoming a collapse is the thing that ends most attempts.

## Mechanics

**The Floor.** Three things: a step minimum, protein at lunch, dinner plated in the kitchen. It's the entire plan on your worst day, and it counts as a full success rather than a partial one.

**Runes.** Earned by doing the day's actions. 100 for the Floor, up to 200 for steps, 300 for a lift session, 100 each for a pre-made lunch and plating dinner. A full day is 800.

**Levels.** Runes are temporary until spent. Leveling makes them permanent and raises one stat, and each stat raises its own requirement. The plan gets harder without you deciding to make it harder. Vigor gates Strength and Endurance, so consistency always leads.

**Death and the cache.** A day scoring zero drops your unspent runes into a cache. Score anything the next day and you recover all of them. Miss twice and they're gone permanently. *Never miss twice* stops being advice and becomes a thing you can lose.

**Flasks.** Two per month. One converts a zero day into a Floor day: no runes, but no death and the streak survives. Using one is a correct play.

**Bosses.** Progressive overload on the squat, from 115 up a ladder of five: 135, 155, 185, 205, 225.

**The only weekly target** is beating last week's rune total. Not a number, just more than last time.

## Running your own

Fork or download, then serve the files from any static host. GitHub Pages works: Settings → Pages → Deploy from a branch → `main` / root.

Data lives in `localStorage`, scoped to the domain it's served from. Back up and restore buttons are at the bottom of the app.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire app |
| `manifest.json` | Home screen install metadata |
| `sw.js` | Service worker, offline caching |
| `icon-*.png` | App icons |

MIT licensed. Take it apart.
