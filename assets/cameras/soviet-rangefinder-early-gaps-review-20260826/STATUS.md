# Status

## Batch

- Name: Soviet rangefinder early gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- FED 2
- Zorki 1C, representing the App's generic Zorki 1 variant
- Kiev II

A full filename, review-document, and App inventory search found no qualified
model-specific asset for these exact variants. The models are kept separate
from FED 3/4/5, Zorki 4/4K/6, and Kiev 4A imagery.

## Persisted checkpoint

- Six exact-model retailer reference files are stored in `refs/`.
- Source URLs and structural distinctions are recorded in `SOURCES.md`.
- Generation constraints are recorded in `PROMPTS.md`.
- `generated/`, `final/`, and `rejected/` are ready.
- `generated/fed-2-rollnote-raw-v1.png` is persisted. Its exact FED 2
  proportions, finder arrangement, controls, M39-style mounted lens,
  straight-on view, hard monochrome linework, moderate depth, and local
  geometric text substitutions passed the first visual check. Its
  edge-connected raw checkerboard was removed during final normalization.
- `generated/zorki-1c-rollnote-raw-v1.png` is persisted. Its compact early
  body, three-window finder block, large top knobs, collapsible-lens structure,
  hard monochrome linework, moderate depth, and pseudo-glyph markings passed
  the first visual check. Its edge-connected raw checkerboard was removed
  during final normalization.
- `generated/kiev-ii-rollnote-raw-v1.png` is persisted. Its meterless
  Contax-derived stepped body, paired rectangular finder windows, integrated
  mount plate, self-timer, large top dials, hard monochrome linework, moderate
  depth, and local geometric marks passed the first visual check. Its
  edge-connected raw checkerboard was removed during final normalization.
- Accepted finals are saved as `final/fed-2-rollnote-v1.png`,
  `final/zorki-1c-rollnote-v1.png`, and `final/kiev-ii-rollnote-v1.png`.
- Each final is 1536x1024, 8-bit RGBA with measured alpha range 0/255.
- `soviet-rangefinder-early-gaps-review-board-a-v1.png` correctly pairs FED 2
  and Zorki 1C with their same-model references.
- `soviet-rangefinder-early-gaps-review-board-b-v1.png` correctly pairs Kiev II
  with its same-model reference.
- Final visual inspection passed: isolated complete bodies, exact front views,
  hard black linework, monochrome-forward metal/leather shading, moderate
  three-dimensional depth, and local geometric trademark substitutions.
- `npm run build` passed on 2026-08-26 (Vite 8.0.14, 1877 modules transformed,
  completed in 2.34 seconds).
- Accepted finals and review boards were uploaded in RollNote-assets commit `5a6e870`; App mappings were not changed.

## Next action

Upload approved and completed in RollNote-assets commit `5a6e870`. App integration remains pending; preserve existing imageStub and rollback values when connecting.
The next deduplicated early-family candidates are FED 1, Zorki 2, and Kiev III.
