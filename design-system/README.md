Book Dashboard is a personal reading tracker: what is being read now, what to read next, the whole library, and the statistics behind it. The look is a quiet forest-green dashboard on a mint ground, with Playfair Display carrying every heading and big number, and DM Sans doing everything else. It should feel like a well-kept reading journal, not an analytics product.

## Content fundamentals

- **Voice.** Second person and warm, written for one reader: "Track your reading journey across all platforms", "What should I read next?", "Your TBR list is empty!". An exclamation mark is fine in empty states, nowhere else.
- **Casing.** Title Case for section headings, tabs and buttons ("Currently Reading", "All Books", "Pick a random book" is the one sentence-case exception, kept as-is). Uppercase only through the label styles (`stat-label`, `pace-label`, `filter-label`, `micro-label`), never typed in caps.
- **Reader vocabulary.** Use the reader's terms as written: TBR, DNF, Dramione, AO3, fic, Wrapped, "projected EOY". Genre tags keep their source spelling, including Danish ones (Krimi, Klassiker).
- **Numbers.** Thousands separators always ("383,389 words"). Dates are `YYYY/MM/DD`. Durations read "Day 12 · started 2026/09/23"; hours read "12h 30m", and from 100 hours just "658h". Ratings in prose are "★ 4.5". Join facts with a spaced middle dot " · ".
- **Empty and missing.** A missing value is an em dash "—" in `gray-400`. An empty section says what is missing and what to do next ("Add start dates to your books to see reading speed stats.").
- **Glyphs, not emoji decoration.** Action labels lead with plain Unicode marks: ✓ Finished, ⏸ Pause, ▶ Resume, ← this. The emoji in the source are functional markers: 📚 before a series name, ⚡ fastest read, 🐢 slowest read. Don't add others.

## Visual foundations

### Color
- Page ground is `bg`. Every card, panel, table and dialog is `white`. Don't place content directly on `primary` except in the Header.
- `primary` is the brand: the header band, all Playfair text, big numbers, and the hover state of accent actions.
- `accent` is the action and "active" color: primary buttons, active tabs, chips and segments, bar fills, card rules, focus borders. `accent-light` is its tint for halos, hovers and checked states.
- Text runs `gray-900` (titles) → `text` (body) → `gray-700` (labels, headers) → `gray-500` (secondary) → `gray-400` (tertiary meta only).
- Badge colors are a fixed lookup by platform and ownership (see Badge). Don't reuse them for anything else.
- `badge-pink` is reserved for Dramione: its header button, segmented option, AO3 badge, and the Dramione Corner panel.
- Danger is two-step: soft for DNF (`danger-text`, `danger-border`, `danger-tint`, `danger`), strong for Delete (`danger-strong`).
- The heatmap ramp runs `heat-0` → `heat-5` (gray, then mint to forest). It is the only multi-step scale.
- **Contrast.** These source pairs fall under 4.5:1 and are kept exact: `accent` as small text (3.8:1), `white` on `accent` buttons (3.8:1), `gray-400` meta (2.5:1), and several badge tints (amber 2.0:1, orange 2.5:1, pink 3.1:1, blue 3.3:1). Use `primary` or `gray-500` for small text that must be read; never use `gray-400` for essential information.

### Type
- Two Google-hosted families: `display` (Playfair Display 600/700) and `sans` (DM Sans 400–700). Load both from Google Fonts.
- Playfair is for headings and figures only: `dashboard-title`, `hero-title`, `section-title`, `panel-title`, `dialog-title`, `stat-value`, `pace-number`, `wrapped-value`, and the rank and hours numerals. Always `primary`, except book titles on cards (`gray-900`).
- DM Sans carries everything else at `body` (16px / 1.6). UI controls are `ui` (14px / 600). Meta is `meta` (12.8px). Badges are `badge` (12px / 600).
- Uppercase labels always carry letter-spacing (0.04–0.05em) and come only from the Labels group.

### Spacing and layout
- Content sits in a 1400px max container with `space-8` padding (0.75rem on mobile).
- The rem steps are `space-1` 0.25 · `space-2` 0.5 · `space-3` 0.75 · `space-4` 1 · `space-5` 1.25 · `space-6` 1.5 · `space-8` 2 · `space-12` 3. Cards pad `space-6`, grids gap `space-6`, and items inside a card gap `space-2`.
- Grids use `auto-fit`/`auto-fill` with a minimum per item: stat cards 200px, reading cards 320px, Wrapped 170px, Dramione cells 130px, charts 400px.
- One breakpoint, 768px: two-column stats collapse to one, tables shrink to 0.8rem and scroll sideways, the heatmap shrinks its cells.

### Radii, borders, shadows
- Radius grows with the container: `radius-sm` (tracks, small buttons) → `radius-md` (buttons, inputs) → `radius-lg` (stat cards, tables) → `radius-xl` (reading cards, panels) → `radius-2xl` (hero, dialogs). `radius-pill` is for badges only.
- Emphasis comes from a solid color rule on one edge: 4px top for stat cards, the hero, Wrapped and Dramione panels; 5px left for reading cards (`accent`, `gray-400` paused, `danger` DNF; `primary` for the TBR pick). This is the source's own signature; keep it to those components.
- Shadows are soft and neutral: `shadow-card` at rest, `shadow-soft` for panels, `shadow-raised` for reading cards and the hero, `shadow-menu` for menus and toasts, `shadow-dialog` / `shadow-modal` for overlays.
- Borders: 1px `gray-300` on controls, 1px `gray-100` row dividers, 2px `gray-200` under table headers and the tab bar.

### States and motion
- Hover: outline controls turn their border and label `accent`; filled `accent` controls turn `primary`; the hero button turns `accent` and scales 1.02; rows and tabs go one gray step darker.
- Focus: inputs drop the outline for an `accent` border plus a 3px `accent-light` halo. Buttons have no custom focus style in the source. Add a visible focus ring when you extend this system.
- Disabled: `opacity-disabled` with `cursor: not-allowed`.
- Motion is short and functional: 0.15–0.3s color transitions, a 0.2s fade for dialogs, a 0.3s slide-up for toasts, and a 0.4s rise-and-scale when a random TBR pick appears.

## Iconography

There is no icon set or logo. The product name is set in Playfair Display as type. Icons are Unicode characters inline with text: ★/☆ for ratings, ✓ ⏸ ▶ in action labels, ← in lists, and the three functional emoji 📚 ⚡ 🐢. Keep that approach; don't introduce an icon font or SVG set without a reason.

## Using this system

Load `tokens.css` and `components/bundle.css` (it imports the two Google fonts). Components are plain HTML with class names, no JavaScript bundle: copy the markup in each component's preview. There is one light theme, matching the app.

## Not synced

- Extracted from `index.html` at commit 6474503. Its `:root` variables keep their names. Hard-coded colors were named here (`danger-*`, `star`, `star-active`, `heat-*`, the tints and overlays). Font sizes, rem spacing steps, radii, shadows and z-indexes were collected from the rules. Spacing names are new; their values are exact.
- Component classes were consolidated: the many single-purpose button classes became `.btn` plus a variant. Each component README lists the source classes it covers.
- The app has no dark theme, no logo, and no font files (both faces are Google-hosted), so the system has none either. Internal table editors (`.bulk-*`, `.platform-dropdown-*`) and the inline Start/Edit button styles are folded into Button and DataTable.
