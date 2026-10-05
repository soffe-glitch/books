# Header

The full-width `primary` band that opens the page: the dashboard name in `dashboard-title`, one line of subtitle, and the add actions as ghost buttons.

## Use
- One per page, at the very top, above the TabBar.
- Text is `white` on `primary`. The title is the only `dashboard-title` on the page.
- Actions are `.header-btn` (white ghost: `header-btn-fill` ground, `header-btn-border` border). The Dramione action adds `.header-btn-dramione` (pink ghost) — it is the only place pink appears in the header.

## Consumer supplies
Title text, subtitle, and 1–2 buttons. Labels start with "+ " for create actions ("+ Add Book").

## Mobile (≤768px)
Padding 1.25rem 1rem, title 1.5rem, subtitle 0.8rem, buttons 0.4rem 0.75rem at 0.75rem.

Source classes: `.header`, `.header-actions`, `.header-btn`, `.header-btn-dramione`.
