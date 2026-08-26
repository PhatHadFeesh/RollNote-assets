# Status

## Batch

- Name: Soviet rangefinder child gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- FED 4
- Zorki 4K
- Chaika 3

A full filename, review-document, and App inventory search found no qualified
asset for these exact variants. The names are intentionally precise so this
batch does not duplicate or mix the adjacent FED 3, Zorki 4, and Chaika II
variants completed in the preceding batch.

## Final assets

- `final/fed-4-rollnote-v1.png`
- `final/zorki-4k-rollnote-v1.png`
- `final/chaika-3-rollnote-v1.png`

All three files are 1536x1024, 8-bit RGBA PNGs. Alpha-channel analysis reports
both fully transparent and fully opaque pixels for every final.

## Review boards

- `soviet-rangefinder-child-gaps-review-board-a-v1.png`: FED 4 and Zorki 4K
- `soviet-rangefinder-child-gaps-review-board-b-v1.png`: Chaika 3

## Quality control

- Two exact-model structural references are retained for each camera with
  source URLs in `SOURCES.md`.
- Exact straight-on front view is used for all three candidates.
- FED 4 preserves its meter-equipped upper housing, selenium grid, adjacent
  long panel, finder, top controls, textured shell, self-timer lever, stacked
  M39 lens rings, screws, and chrome base. It is not mixed with FED 3 or FED 5.
- Zorki 4K preserves the stepped rangefinder body, window layout, top controls,
  ribbed wrap, self-timer lever, M39 lens, and a clearly visible top-right
  rapid-wind lever. The first candidate without an explicit enough lever is
  retained in `rejected/`; the accepted correction is not a non-4K Zorki 4.
- Chaika 3 preserves its compact boxy half-frame body, left meter/name panel,
  right finder, square release, ribbed front, round lower socket, centered lens,
  top shoe/dial silhouette, and lower feet. It does not use the Chaika II body.
- Early RollNote styling is consistent across the group: hard black contours,
  crisp internal linework, monochrome-forward shading, modest rounding,
  moderate body/lens depth, and only restrained cool glass highlights.
- Brand names, model wording, logos, numbers, lens inscriptions, and instruction
  marks are replaced locally with crisp unreadable geometric marks. No
  whole-camera blur was used.
- Edge-connected generated checkerboards were removed. `sips` confirms 1536 by
  1024, 8-bit PNG, and alpha for every final; alpha minimum/maximum checks are
  0.0/1.0 for all three.
- Comparison-board pairing was visually verified; no model is paired with a
  different variant.
- No assets were uploaded to `RollNote-assets` and no App mapping changed.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules
  transformed, built in 2.06s).

## Next candidates

A useful next same-parent gap group, subject to exact-reference validation at
the start of the next run, is FED 5B, Zorki 6, and Kiev 4A. Filename and App
inventory searches show these variants but no qualified variant-specific
review asset.
