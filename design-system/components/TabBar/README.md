# TabBar

Sticky, equal-width tabs that switch the dashboard's top-level views.

## Use
- Sits directly under the Header; `position: sticky; top: 0` with `z-tabbar` and `shadow-tabbar`.
- Inactive tabs: `gray-50` ground, `text` label, `gray-100` on hover. Active: `white` ground, `accent` label and a 3px `accent` underline.
- Keep to three or four short nouns (Overview, All Books, Statistics).

## Consumer supplies
Tab labels and which one is active (`.active`).

Source classes: `.tab-bar`, `.tab-button`.
