# Status

## Batch

- Name: Soviet rangefinder icons
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- Chaika II
- FED 3
- Zorki 4

A full filename, review-document, and App inventory search found no qualified
asset for these exact variants. Chaika II is intentionally named precisely so
its body is not confused with the generic Chaika, Chaika I, or Chaika 3.

## Final assets

- `final/chaika-ii-rollnote-v1.png`
- `final/fed-3-rollnote-v1.png`
- `final/zorki-4-rollnote-v1.png`

All three files are 1536x1024, 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `soviet-rangefinder-icons-review-board-a-v1.png`: Chaika II and FED 3
- `soviet-rangefinder-icons-review-board-b-v1.png`: Zorki 4

## Quality control

- Two exact structural references are retained for each model with source URLs.
- Exact straight-on front view is used for all three candidates.
- Chaika II preserves its slim half-frame body, wide silver upper shell,
  offset finder, small front release, textured lower body, circular lens mount,
  visible screws, lower socket, chrome base, and side lugs.
- FED 3 preserves the knob-wind chrome top, finder and front-window layout,
  pebbled shell, self-timer lever, front screws, and stacked M39 lens rings. It
  is not mixed with FED 2, FED 4, or FED 5.
- Zorki 4 preserves the stepped non-4K chrome body, finder, top knob controls,
  ribbed wrap, self-timer lever, Jupiter-style black lens, mount ring, and thin
  base. No 4K advance lever was added.
- Early RollNote styling is retained: hard black contours, crisp internal
  linework, monochrome-forward shading, modest rounding, moderate depth, and
  only tiny cool lens-glass accents.
- Brand names, model wording, logos, numbers, lens inscriptions, and instruction
  marks are replaced locally with crisp unreadable geometric marks. No
  whole-camera blur was used.
- Edge-connected generated checkerboards were removed. `sips` confirms alpha,
  and alpha-channel analysis reports both fully transparent and fully opaque
  pixels for every final.
- Comparison-board pairing was visually verified; no model is paired with a
  different variant.
- No assets were uploaded to `RollNote-assets` and no App mapping changed.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules
  transformed, built in 2.18s).

## Next candidates

After another exact-reference and full-library duplicate check, a useful next
parent-gap group is FED 4, Zorki 4K, and Chaika 3. Each must remain separate
from the visually adjacent FED 3, Zorki 4, and Chaika II bodies completed here.
