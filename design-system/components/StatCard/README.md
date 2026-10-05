# StatCard

A single headline figure with an uppercase label, on a white card capped by a 4px `accent` rule.

## Use
- Group in `.stats-grid` (auto-fit, min 200px, gap `space-6`).
- Label in `stat-label` (`gray-500`, uppercase, 0.05em); value in `stat-value` (`primary`, Playfair).
- `.compact` variant (3px rule, 1.5rem value, 0.75rem label, 1rem padding) for the totals row in Statistics, grid min 140px.

## Consumer supplies
Label and a pre-formatted value (thousands separators, abbreviations like 48.2M).

Source classes: `.stat-card`, `.stats-grid`, `.stats-totals`.
