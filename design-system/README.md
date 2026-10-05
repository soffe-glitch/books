Book Dashboard is a personal reading tracker: what is being read now, what to read next, the whole library, and the statistics behind it. Version 2 keeps the brand greens and renews everything around them. It should feel like a reading room, not an analytics tool: Newsreader gives titles, authors and figures the voice of a printed book, Hanken Grotesk keeps the controls plain, and depth comes from hairlines and white space instead of coloured edges and heavy shadows.

## Content fundamentals

- **Voice.** Second person and warm, written for one reader: "Track your reading journey across all platforms", "What should I read next?", "Your TBR list is empty!". Exclamation marks only in empty states and confirmations.
- **Casing.** Title Case for headings, tabs and most buttons ("Currently Reading", "Start Reading"). Uppercase only through the `label` style, never typed in caps.
- **Reader vocabulary.** Keep the reader's own words: TBR, DNF, Dramione, AO3, fic, Wrapped, "projected EOY". Genre tags keep their spelling, including Danish ones (Krimi, Klassiker).
- **Numbers.** Thousands separators always ("383,389 words"); dates `YYYY/MM/DD`; durations "Day 12 · started 2026/09/23"; hours "12h 30m", and from 100 hours just "658h"; ratings in prose "★ 4.5". Join facts with a spaced middle dot " · ". Figures use lining, tabular numerals.
- **Missing values** are an em dash "—" in `faint`. Empty sections say what is missing and what to do next.
- **Glyphs, not decoration.** Action labels may lead with ✓ ⏸ ▶. The only emoji are functional markers: 📚 series, ⚡ fastest read, 🐢 slowest read.

## Visual foundations

### Color
- Three greens with separate jobs: `forest` is the brand (masthead, headings, figures, active states, the pick card); `emerald-ink` is the action colour (primary buttons, links, focus); `emerald` is for graphics only (bar fills, heatmap). `mint` is the tint for chips, halos and checked states.
- Neutrals lean green: `bg` page, `paper` surfaces, `wash` tracks, `line` / `line-strong` borders. Text runs `ink` → `ink-2` → `muted` → `faint`.
- On forest, use `paper`, `mint-on-forest` and `sage-on-forest` only.
- `dramione` (pink) belongs to Dramione alone. Danger is `danger` with `danger-wash` and `danger-line`.
- Badge colours are a fixed lookup by platform and ownership (see Badge).
- **Contrast.** Every text pair reaches 4.5:1 on its ground: `faint` 4.6:1 on `paper`, white on `emerald-ink` 5.5:1, all badge text ≥5:1. Keep `faint` off `wash`. `line` is decorative; control borders use `line-strong`, and the focus ring is solid `emerald-ink`.

### Type
- `display` = Newsreader (optical sizes on): the dashboard title, all headings, book titles, authors (italic), and every big figure. Weight 600 for words, 500 for numbers.
- `sans` = Hanken Grotesk: body 16px / 1.55, buttons and tabs at 600, meta at 12.8px.
- Uppercase captions all use one style, `label` (11.5px / 700 / 0.08em).
- Authors are always italic Newsreader. That one detail is what makes a card read as a book.

### Shape, space and depth
- Every interactive element is a pill (`radius-pill`): buttons, chips, segments, badges, search, pagination. Containers use `radius-lg` (cards, panels, tables) or `radius-xl` (TBR picker, stats hero, dialogs). Fields use `radius-md`.
- Cards are `paper` with a 1px `line` border and `shadow-card`. Only the TBR pick (`shadow-lift`) and overlays (`shadow-overlay`) float.
- State is shown in content, not edges: a status chip on reading cards, a dashed outline for paused or empty, a filled pill for active.
- Layout: content on a 1200px column with 1.5rem gutters, `space-4` between cards and panels, `space-12` between the big Overview sections. One breakpoint at 768px.

### States and motion
- Hover: outline controls turn `emerald-ink`; filled actions darken to `forest`; table rows take `bg`.
- Focus: `focus` ring (paper gap + 2px `emerald-ink`) on every control; fields add a `mint` halo.
- Disabled: 50% opacity, `not-allowed`.
- Motion is brief: 0.15s colour changes, 0.2s fades for dialogs, 0.25s toast slide, 0.4s rise for the random pick. All of it switches off under `prefers-reduced-motion`.

## Iconography

No icon set and no logo: the name is set in Newsreader. Icons are Unicode characters inline with text (★ ✓ ⏸ ▶ ← → and the three functional emoji), plus two inline SVGs: the search magnifier and the select chevron, both drawn in `muted`. Use plain glyphs before reaching for an icon library.

## Using this system

Load `tokens.css` and `components/bundle.css`. The bundle imports Newsreader and Hanken Grotesk from Google Fonts and is the same stylesheet the dashboard ships, minus its `:root` tokens. Components are plain HTML with class names and no JavaScript, so copy the markup from each preview. One light theme. The tokens `primary`, `accent`, `accent-light`, `white`, `text`, `gray-400` and `gray-500` are aliases kept for inline styles in the app's script; new work should use the v2 names.
