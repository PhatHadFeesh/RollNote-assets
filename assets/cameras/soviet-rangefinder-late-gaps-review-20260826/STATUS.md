# Status

## Batch

- Name: Soviet rangefinder late gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- FED 5B
- Zorki 6
- Kiev 4A

A full filename, review-document, and App inventory search found no qualified
asset for these exact variants. The models exist as App variant options, but
there is no variant-specific review final. This batch remains separate from
FED 3/FED 4, Zorki 4/Zorki 4K, and generic Kiev family imagery.

## Persisted checkpoint

- Six exact-model reference files are stored in `refs/`.
- Search-result false positives for Minox, Contax, Nikon, Zorki 4, and generic
  Kiev bodies were inspected and excluded before this checkpoint.
- Source URLs and structural distinctions are recorded in `SOURCES.md`.
- Generation constraints are recorded in `PROMPTS.md`.
- `generated/`, `final/`, and `rejected/` are ready.
- `generated/fed-5b-rollnote-raw-v1.png` is persisted. Its exact FED 5B
  structure, straight-on view, hard monochrome linework, moderate depth, and
  local geometric text substitutions passed the first visual check. Its raw
  edge-connected neutral checkerboard was removed during final normalization.
- `generated/zorki-6-rollnote-raw-v1.png` is persisted. Its low chrome band,
  separate left round window, center oval nameplate, right finder and twin
  sockets, ribbed wrap, self-timer, M39-style lens, and Zorki 6 body silhouette
  passed the first visual check. Its neutral edge background was removed during
  final normalization.
- `generated/kiev-4a-rollnote-raw-v1.png` is persisted. Its low non-meter
  Contax-derived body, stepped silver front, separated finder windows, square
  mount plate, self-timer, socket, large knurled top dials, side lugs, and
  mounted lens passed the first visual check. Its generated checkerboard is
  edge-connected and was removed during final normalization.
- Accepted finals are saved as `final/fed-5b-rollnote-v1.png`,
  `final/zorki-6-rollnote-v1.png`, and `final/kiev-4a-rollnote-v1.png`.
- Each final is 1536x1024, 8-bit RGBA with measured alpha range 0/255.
- `soviet-rangefinder-late-gaps-review-board-a-v1.png` correctly pairs FED 5B
  and Zorki 6 with their same-model references.
- `soviet-rangefinder-late-gaps-review-board-b-v1.png` correctly pairs Kiev 4A
  with its same-model reference.
- `npm run build` passed on 2026-08-26 (Vite 8.0.14, 1877 modules transformed,
  completed in 2.17 seconds).
- Accepted finals and review boards were uploaded in RollNote-assets commit `5a6e870`; App mappings were not changed.

## Next action

Upload approved and completed in RollNote-assets commit `5a6e870`. App integration remains pending; preserve existing imageStub and rollback values when connecting.
