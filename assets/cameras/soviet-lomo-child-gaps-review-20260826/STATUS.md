# Status

## Batch

- Name: Soviet LOMO child-variant gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- Smena 8M
- Smena Symbol
- Lubitel 2

A fresh filename, review-document, and App inventory search found no qualified
asset for these three variants. Kodak Ultra F9 and Holga 135BC were excluded
because qualified review assets already exist. Plain Holga 135 was also
excluded because its visible body is too close to the accepted 135BC candidate
to justify a duplicate before user review.

Lubitel 166 was deferred: the trusted-retailer source for the exact original
166 body had only one structural image, while the other strong results were
166B or Universal bodies. Those variants must not be mixed into an original
166 generation.

## Final assets

- `final/smena-8m-rollnote-v1.png`
- `final/smena-symbol-rollnote-v1.png`
- `final/lubitel-2-rollnote-v1.png`

All three files are 1536x1024, 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `soviet-lomo-child-gaps-review-board-a-v1.png`: Smena 8M and Smena Symbol
- `soviet-lomo-child-gaps-review-board-b-v1.png`: Lubitel 2

## Quality control

- Two real structural references are retained for each completed model with
  exact source URLs.
- Exact straight-on front view is used for all three candidates.
- Smena 8M preserves its wide low body, silver fascia, upper-right finder,
  ribbed top plate, diamond-textured lower shell, multi-ring lens, top
  controls, and small lens levers.
- Smena Symbol preserves its split silver fascia, upper-right finder,
  horizontal-ribbed shell, large left-extending advance lever, lens rings,
  top shoe, and top controls. It remains clearly distinct from the 8M.
- Lubitel 2 preserves its tall narrow TLR body, open finder hood, curved front
  plate, stacked viewing/taking lenses, toothed silver rings, pebbled panels,
  lens controls, and right-side access-panel structure. The reference strap and
  case are omitted.
- Early RollNote styling is retained: hard black outer contours, crisp internal
  linework, monochrome-forward shading, modest rounding, moderate lens/body
  depth, and only tiny red or cool lens-glass recognition accents.
- Brand names, model wording, logos, Cyrillic/Latin labels, numbers, lens
  inscriptions, and instructional marks are replaced locally with crisp
  unreadable geometric marks. No whole-camera blur was used.
- Edge-connected generated checkerboards were removed. Dimensions, 8-bit RGBA
  encoding, alpha, framing, and review-board model pairing were visually
  verified.
- No assets were uploaded to `RollNote-assets` and no App mapping changed.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules
  transformed, built in 1.75s).

## Next candidates

After another full-library duplicate and source-quality check, useful next
models are Fisheye Baby 110, Lubitel 166+ (modern exact body), Chaika, and Smena
35. Original Lubitel 166 remains deferred until a second trusted exact-body
reference is available.
