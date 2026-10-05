# DataTable

The sortable book list: white card, sticky first column, horizontal scroll on narrow screens.

## Use
- Wrap in `.table-wrap` (`white`, `radius-lg`, `shadow-card`, `overflow-x: auto`, thin `accent` scrollbar thumb).
- Header cells: `gray-50` ground, `ui` in `gray-700`, 2px `gray-200` underline, hover `gray-100`; clickable headers sort.
- Cells: 0.75rem padding, 1px `gray-100` dividers, row hover `gray-50`.
- The Title column is frozen (`position: sticky; left: 0`, `shadow-frozen`), 140–280px wide.
- Empty values show a `gray-400` em dash. A value computed rather than entered (pages from words ÷ 250) is shown in `accent`.
- Row actions are `.btn-xs` buttons at the row end: Start (TBR), Resume (DNF), Edit.
- Paginate at 50 rows.
- Mobile: 0.8rem text, 0.4rem padding, `nowrap` except the Title column (110–160px).

Source classes: `.books-table`, `.books-table-wrapper`, `.recently-read-table`, `.bulk-table`.
