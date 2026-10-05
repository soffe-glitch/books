# EmptyState

What a section shows when it has nothing yet, or while it loads.

## Use
- Section-level: `.cr-empty` — white card, `radius-xl`, 2rem padding, centered italic `gray-400`.
- Inside a panel: one plain line in `gray-400` at 0.85rem.
- Loading: `.loading`, centered `gray-500`, 3rem padding. Load errors: same block in `danger-strong`.
- Copy says what is missing and the next step, in a friendly voice: "Your TBR list is empty!", "No books read in 2026 yet — come back after a few reads!"

Source classes: `.cr-empty`, `.loading`.
