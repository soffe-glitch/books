# Dialog

Overlays on a forest-tinted scrim: the compact rating dialog and the Add/Edit Book modal.

- Rating dialog: `paper`, `radius-xl`, `shadow-overlay`, max 420px, centred. Title in Newsreader `forest`, 2.4rem stars (`star` when selected, `line-strong` when not), "4 / 5" readout, then actions.
- Modal: 580px, `radius-xl`, heading in `modal-title`, fields per Input, footer under a `line` hairline (Delete left on edit; Cancel + Save right). Series siblings list on `bg`, the current book in `ink` with "← this".
- Both fade in over 0.2s.
