# StarRating

Five-star ratings, read-only in tables and clickable in the editor and the finish dialog.

## Sizes
- `.stars` — read-only text stars in `star`, letter-spacing 0.1em, filled ★ and empty ☆.
- `.star-rating` — 1.25rem clickable stars; `.filled` `star`, `.empty` `gray-300`, hover scale 1.2.
- `.rating-star` — 2.5rem stars in the rating dialog; hover/selected `star-active` with scale 1.15.

## Rules
- Ratings are whole stars 1–5; 0 means unrated and shows "—" in tables.
- In summary text, a rating is "★ 4.5" (star glyph, space, number).

Source classes: `.stars`, `.star-rating`, `.rating-star`.
