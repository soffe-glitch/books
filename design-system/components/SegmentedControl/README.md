# SegmentedControl

Joined buttons for picking one of a few mutually exclusive options, with an uppercase caption.

## Use
- Caption in `filter-label` (`gray-500`). Control: `gray-50` ground, 1px `gray-300` border and dividers, `radius-lg`, clipped corners.
- Segments 0.85rem/500 `gray-700`; hover `accent-light`; active `accent` fill + `white`.
- The Dramione option adds `.tbr-seg-dramione`, which turns its active fill `badge-pink`.
- Several controls sit in a `.tbr-filters` strip (white, `radius-xl`, gap 1.25rem).
- Spell out thresholds in the label: "Long (>300 pg)".

Source classes: `.tbr-filters`, `.tbr-filter-group`, `.tbr-filter-label`, `.tbr-segmented`, `.tbr-seg`.
