# Status

## Batch

- Name: LOMO compact and TLR child gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- Fisheye Baby 110
- Lubitel 166+
- Smena 35

A full filename, review-document, and App inventory search found no qualified
asset for these exact variants. Chaika was deferred because search results mix
the original Chaika and visibly different Chaika II bodies; no mixed-reference
generation is allowed.

## Final assets

- `final/fisheye-baby-110-rollnote-v1.png`
- `final/lubitel-166-plus-rollnote-v1.png`
- `final/smena-35-rollnote-v1.png`

All three files are 1536x1024, 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `lomo-compact-tlr-gaps-review-board-a-v1.png`: Fisheye Baby 110 and Smena 35
- `lomo-compact-tlr-gaps-review-board-b-v1.png`: Lubitel 166+

## Quality control

- Two exact structural references are retained for each model with source URLs.
- Exact straight-on front view is used for all three candidates.
- Fisheye Baby 110 preserves its tiny wide black body, silver front band,
  centered projecting fisheye lens, raised circular finder, top controls, lugs,
  and shallow metal-body depth.
- Lubitel 166+ preserves the modern tall TLR body, open extended hood, stacked
  silver-ringed lenses, silver front frames, pebbled panels, side knobs, and
  lens controls. Original 166, 166B, and Universal references were not mixed.
- Smena 35 preserves its compact asymmetric shell, upper fascia, offset finder,
  large ribbed lens ring, red top control, side vents, grip seam, and restrained
  blue recognition lines. It remains distinct from Smena 8M and Smena Symbol.
- Early RollNote styling is retained: hard black contours, crisp internal
  linework, monochrome-forward shading, modest rounding, moderate depth, and
  only necessary muted recognition color.
- Brand names, model wording, logos, numbers, lens inscriptions, and instruction
  marks are replaced locally with crisp unreadable geometric marks. No
  whole-camera blur was used.
- Generated edge-connected checkerboards were removed. `sips` confirms alpha,
  and alpha-channel analysis reports both fully transparent and fully opaque
  pixels for every final.
- The first Lubitel 166+ generation call stalled without creating a file. The
  timeout was recorded, the completed Fisheye and Smena assets were preserved,
  and only the missing Lubitel candidate was retried successfully.
- No assets were uploaded to `RollNote-assets` and no App mapping changed.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules
  transformed, built in 2.22s).

## Next candidates

After another exact-reference and full-library duplicate check, a useful next
group is Chaika II, FED 3, and Zorki 4. The generic Chaika inventory label must
not be used until a precise body generation is selected. Original Lubitel 166
also remains deferred until a second trusted exact-body reference is available.
