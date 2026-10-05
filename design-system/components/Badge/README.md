# Badge

A pill that names where a book lives (platform), how it was got (ownership), or its genre tag.

## Mapping (fixed — a platform always gets its color)
| Kind | Value | Class | Tokens |
|---|---|---|---|
| Platform | Kindle | `.badge-kindle` | `badge-blue` on `badge-blue-tint` |
| | Physical | `.badge-physical` | `badge-amber` |
| | Mofibo | `.badge-mofibo` | `badge-violet` |
| | AO3 | `.badge-ao3` | `badge-pink` |
| | Apple Books / unknown | `.badge-apple` / `.badge-unknown` | `badge-gray` |
| | Saxo | `.badge-saxo` | `badge-orange` |
| | Audiobook | `.badge-audiobook` | `badge-indigo` |
| Ownership | Owned / Streamed / Borrowed / Free | `.badge-owned` … | `accent`, `badge-indigo`, `badge-amber`, `badge-gray` |
| Tag | any genre | `.badge-tag` | `accent` on `accent-tint` |

## Rules
- `badge` type (0.75rem / 600), padding 0.25rem 0.75rem, `radius-pill`. Badges wrap with 0.25rem right/bottom margins.
- A missing value shows a `gray-400` em dash, never an empty badge.
- Several tints fail 4.5:1 (amber 2.0:1, orange 2.5:1); they are kept exact from the source — the text always repeats the value, so color is never the only signal.

Source classes: `.badge`, `.badge-*`.
