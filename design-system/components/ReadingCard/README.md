# ReadingCard

A book in progress. State is a chip at the top, not a coloured edge.

## Anatomy
1. Status chip (`.cr-card-duration`, `chip` type) — `mint`/`forest` "Day 12 · started …" while reading; `wash`/`ink-2` "⏸ Paused on day N" when paused; `danger-wash`/`danger` for DNF. It is placed last in the markup and moved to the top with CSS `order`.
2. Title in `book-title` (`ink`).
3. Author in italic `author` (`muted`).
4. Series link (optional): 📚 + series + "#n of N" in `emerald-ink`.
5. Meta: pages · words · format in `meta` (`faint`).
6. Actions under a `line` hairline.

## States
- Reading: `paper`, `line` border, `radius-lg`, `shadow-card`.
- `.paused`: `bg` ground, dashed `line-strong` border, no shadow; title drops to `ink-2`. Paused cards sort last.
- `.dnf`: 92% opacity with the danger chip.

Lay out in a grid of `minmax(320px, 1fr)` with `space-4` gaps.
