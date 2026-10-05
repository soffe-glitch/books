# Input

Text fields, selects and checkbox chips for search and the add/edit book form.

## Use
- `.input` / `.select`: 1px `gray-300` border, `radius-md`, 0.6rem 0.75rem, 0.9rem. Focus: border `accent` plus a 3px `accent-light` halo, no outline.
- `.input-search`: full-width, 0.75rem padding, 1rem text. Placeholder names the fields searched ("Search by title or author...").
- Labels above inputs in `meta` 600 `gray-500` (`.form-group`); pair fields with `.form-row` (two columns).
- Hints sit inside the label in `gray-400`, weight 400: "Pages (auto from words)".
- Multi-select platforms use `.platform-checks`: bordered chips that turn `accent-light` with an `accent` border when checked.

Source classes: `.search-box input`, `.form-group`, `.form-row`, `.platform-checks`.
