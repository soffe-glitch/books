# ReadingCard

A book in progress: title, author, series, size, how long it has been going, and what to do next.

## Anatomy (top to bottom, gap `space-2`)
1. Title — `panel-title` in `gray-900` (Playfair).
2. Author — `author` in `gray-500`; "Unknown author" if missing.
3. Series link (optional) — `.series-line`: 📚 + series + #order, 0.75rem/600 `accent`, underline on hover.
4. Meta — pages · words · format, `meta` in `gray-400`, joined with " · ".
5. Duration — "Day 12 · started 2026/09/23" in `accent` 500.
6. Actions — `.btn-primary` first, then outline, then DNF.

## States
- Active: 5px `accent` left rule.
- `.paused`: `gray-400` rule, `gray-50` ground, duration "⏸ Paused on day N" in `gray-500`; actions become ▶ Resume + ✓ Finished.
- `.dnf`: `danger` rule, `opacity-dnf`, duration in `danger-text`.

## Related
- `.tbr-pick-card` — the random TBR pick: same anatomy with a 5px `primary` rule, `shadow-pick`, max 500px, revealed with a 0.4s rise-and-scale; actions Start reading + Pick again.
- Lay cards in a grid of `minmax(320px, 1fr)` with gap `space-5`. Paused cards sort last.

Source classes: `.cr-card*`, `.tbr-pick-card`, `.series-line`.
