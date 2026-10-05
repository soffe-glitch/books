# Button

Every action is a pill: one shape, four tones, three sizes.

| Tone | Classes | Look |
|---|---|---|
| Primary | `.btn-finished`, `.btn-start-reading`, `.btn-resume`, `.btn-save` | `emerald-ink` fill, `paper` label (5.5:1); hover `forest`. |
| Outline | `.btn-pause`, `.btn-pick-again`, `.btn-cancel`, `.btn-quiet` | `paper`, `line-strong` border, `ink-2` label; hover border and label `emerald-ink`. |
| Soft danger | `.btn-dnf` | `danger` label, `danger-line` border; hover `danger-wash`. |
| Destructive | `.btn-delete` | Outline that fills `danger` on hover. Edit modal only. |
| Hero | `.btn-pick-random` | `forest` fill, 1rem, the one big action of a section. |

Sizes: default 0.5rem 1rem; modal footer 0.6rem 1.35rem; `.btn-row` (0.2rem 0.65rem, 0.8rem) for table rows, `.btn-row.primary` for Start/Resume.

## Rules
- One primary per card, first in the row. Lead labels with a plain glyph when it names a state change: ✓ Finished, ⏸ Pause, ▶ Resume.
- Disabled: 50% opacity, `not-allowed`. Focus: the `focus` ring.
- On the forest pick card, primary turns `mint`/`forest` and outline turns a white ghost.
