# Heatmap

The Reading Journey: a month × year grid shaded by how many books were finished.

## Use
- Rows are months (Jan–Dec labels, 0.72rem `gray-500`), columns are years (headers 0.72rem/600).
- Cells 36×22px, gap 3px, `radius-sm`; levels `heat-0` (none) through `heat-5`, scaled to the busiest month: ≤15%, ≤35%, ≤55%, ≤80%, above.
- Hover: 2px `accent` outline, scale 1.15, and a `gray-900` tooltip with the month, count and up to five titles.
- A Less → More legend of 14px squares sits bottom-right.
- Mobile: 24×18px cells inside a horizontal scroller.

Source classes: `.journey-*`.
