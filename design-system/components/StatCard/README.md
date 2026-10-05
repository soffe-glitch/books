# StatCard

Totals in a single ledger: one bordered card divided by hairlines into cells.

- `.stats-totals` is the card (`paper`, `line` border, `radius-lg`); each `.stat-card` cell draws its own right and bottom hairline, so an uneven last row leaves white space.
- Label in `label`, value in `stat-value` (`forest`, lining tabular numerals). Long numbers wrap rather than overflow.
- Two columns on phones.
- Standalone cards (`.stats-grid .stat-card`) get their own `line` border and `radius-lg`.
