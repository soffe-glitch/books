# WrappedGrid

Year-in-review tiles: a label, one answer, and an optional supporting figure.

## Use
- Grid auto-fit min 170px, gap `space-3`. Each `.wrapped-cell`: `accent-light`→`white` 135° gradient, 4px `accent` left rule, `radius-xl`, min-height 90px.
- `micro-label` caption in `gray-500`; `wrapped-value` answer in `primary`; `.w-sub` 0.75rem `gray-500` pinned to the bottom.
- Titles clip at 45 characters with "…". Missing answers show "—".

Source classes: `.wrapped-grid`, `.wrapped-cell`.
