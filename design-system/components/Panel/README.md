# Panel

The white containers that hold every Statistics section: a plain panel, an emphasized hero, and accent-topped variants.

## Variants
- `.stats-panel` — `white`, `radius-xl`, `shadow-soft`, padding `space-6`. Its `h3` is `panel-title` in `primary` with a 1px `gray-100` underline.
- `.stats-hero` — the one hero per view: `radius-2xl`, `shadow-raised`, 2rem padding, 4px `accent` top rule, `h2` in `hero-title`. Holds the Reading Pace numbers (`pace-number` / `pace-label`) and a 10px year-progress bar.
- `.wrapped-panel` adds the 4px `accent` top rule; `.dramione-panel` uses a 4px `badge-pink` rule.

## Rules
- Stack panels with `space-6` between; use a two-column grid (`.stats-two-col`) above 768px, one column below.
- Pace numbers color by meaning: actuals `primary`, rate `accent`, projections `gray-400`.
- Empty panels show one line in `gray-400` at 0.85rem saying how to fill them ("Add start dates to your books to see reading speed stats.").

Source classes: `.stats-panel`, `.stats-hero`, `.pace-*`, `.chart-container`, `.recently-read`.
