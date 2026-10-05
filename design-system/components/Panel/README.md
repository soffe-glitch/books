# Panel

White containers for every Statistics section, plus one larger hero.

- `.stats-panel`: `paper`, `line` border, `radius-lg`, 1.35rem 1.5rem padding; heading in `panel-title` (`forest`), no underline.
- `.stats-hero`: `radius-xl`, larger padding, heading in `section-title`. Holds the Reading Pace figures in `pace-number`, coloured by meaning (actuals `forest`, rate `emerald-ink`, projections `faint`) with `label` captions, and a year-progress bar.
- Stack with `space-4` gaps; two columns above 768px (`.stats-two-col`).
- Empty panels: one `faint` line saying how to fill them.
