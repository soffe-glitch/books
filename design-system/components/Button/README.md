# Button

Every clickable action in the dashboard: one shape (`radius-md`, `ui` type) in five tones.

## Variants
| Class | Look | Use |
|---|---|---|
| `.btn-primary` | `accent` fill, `white` label, hover `primary` | The main action in a card or form: Finished, Start reading, Resume, Save. |
| `.btn-outline` | `white`, `gray-300` border, `gray-500` label; hover border and label `accent` | Secondary: Pause, Pick again, Cancel, Edit. |
| `.btn-dnf` | `danger-text` on white, `danger-border`; hover `danger-tint` + `danger` | Did-not-finish, a soft negative. |
| `.btn-delete` | `danger-strong` outline, fills on hover | Destructive delete in the edit modal only. |
| `.btn-hero` | `primary` fill, `radius-lg`, 1rem; hover `accent` and scale 1.02 | The single headline action of a section (Pick a random book). |

Sizes: default 0.5rem 1.25rem; `.btn-lg` 0.6rem 1.5rem (modal footers); `.btn-xs` 0.25rem 0.5rem at 0.8rem with `radius-sm` (inline table actions).

## Rules
- At most one `.btn-primary` per card; put it first.
- Status glyphs lead the label as plain characters: ✓ Finished, ⏸ Pause, ▶ Resume.
- Disabled: `opacity-disabled` (hero: `opacity-disabled-strong`), `cursor: not-allowed`.
- White on `accent` is 3.8:1 — fine for these 14px semibold labels at the source's own standard, but below WCAG AA for small text.

Source classes: `.btn-finished`, `.btn-start-reading`, `.btn-resume`, `.btn-save`, `.export-btn` → `.btn-primary`; `.btn-pause`, `.btn-pick-again`, `.btn-cancel` → `.btn-outline`; `.btn-dnf`; `.btn-delete`; `.btn-pick-random` → `.btn-hero`.
