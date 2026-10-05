# BarChart

Horizontal labelled bars for counts per month or per tag: no chart library, plain divs.

## Use
- Each `.bar-item`: a `.bar-label` row (name left, count right, 0.875rem) above a 24px `gray-200` track with an `accent` fill.
- Fill width = count ÷ the largest count in the set. The count repeats inside the fill in `white` 0.75rem semibold.
- One series, one color. Do not color bars by category.

## Consumer supplies
Rows of label + count, already sorted (months in calendar order, tags by count).

Source classes: `.bar-item`, `.bar-label`, `.bar-track`, `.bar-fill`.
