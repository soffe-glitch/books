# DataTable

The books list: a bordered card with hairline rows and a frozen, serif title column.

- Wrapper: `paper`, `line` border, `radius-lg`, horizontal scroll with a thin `line-strong` scrollbar.
- Headers in `label` (`muted`) over a `line-strong` rule; sortable headers turn `emerald-ink` on hover.
- Rows: `line` dividers, `bg` on hover, tabular numerals.
- The Title column is `table-title` (Newsreader) and sticky on the left with a hairline edge.
- Computed values (pages from words ÷ 250) show in `emerald-ink`; missing values are a `faint` em dash.
- Row actions are `.btn-row` pills at the end of the row.
