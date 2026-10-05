# Header

The forest masthead and its tab bar: one continuous green block at the top of every view.

## Use
- Title in `dashboard-title` (`paper`), subtitle in italic `subtitle` (`mint-on-forest`), left-aligned on a 1200px column.
- Actions sit right, vertically centred: `+ Add Book` is a `mint` pill with `forest` text; `+ Add Dramione` is a ghost pill with a `dramione-on-forest` dot. That dot is the only pink in the masthead.
- The tab bar continues the forest ground and is sticky. Tabs are `tab` type at 72% white; the active tab is `paper` with a 3px `mint-on-forest` underline.
- Mobile (≤768px): actions drop under the subtitle; tabs share the width equally.

Source: `.header`, `.header-actions`, `.header-btn(-dramione)`, `.tab-bar`, `.tab-button`.
