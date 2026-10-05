# Dialog

Two overlay sizes: the compact centered rating dialog, and the form modal for adding and editing books.

## Rating dialog
- `white`, `radius-2xl`, `shadow-dialog`, max 400px, centered text; scrim `overlay`; `z-dialog`. Fades in over 0.2s.
- Title in `dialog-title` (`primary`), a `gray-500` sub-line, 2.5rem stars, a `gray-400` "N stars" readout, then actions.

## Form modal
- `white`, `radius-2xl`, 2rem padding, 560px (max 95vw / 90vh, scrolls inside), `shadow-modal`, scrim `overlay-strong`, `z-modal`.
- `h2` in Playfair `primary`. Fields use Input. Footer: Delete on the left (edit only), Cancel + Save on the right.
- Books in the same series list in `.series-siblings` (`series-tint` ground), the current one in `gray-500` with "← this".

Source classes: `.rating-dialog*`, `.modal*`, `.series-siblings`.
