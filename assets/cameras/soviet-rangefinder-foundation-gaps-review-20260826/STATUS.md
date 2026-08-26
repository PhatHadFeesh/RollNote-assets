# Status

## Batch

- Name: Soviet rangefinder foundation gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Selected models

- FED 1g, representing the App's generic FED 1 variant
- Zorki 5
- Kiev III

A full filename, review-document, and App inventory search found no qualified
model-specific asset for these variants. FED 1g is separated from FED 2/3/4/5,
Zorki 5 from Zorki 4/4K/6, and the metered Kiev III from Kiev II/4/4A.

Zorki 2 was researched but deferred because the currently verified retailer
set did not provide two complete same-variant views. No Zorki 2 candidate was
generated.

## Completed outputs

- Six model-specific retailer reference files are stored in `refs/`.
- Source URLs and structural distinctions are recorded in `SOURCES.md`.
- Generation constraints are recorded in `PROMPTS.md`.
- `generated/`, `final/`, and `rejected/` are present.
- `generated/fed-1g-rollnote-raw-v1.png` is persisted. Its compact early body,
  finder block, top controls, collapsible-lens structure, straight-on view,
  hard monochrome linework, moderate depth, and geometric label substitutions
  passed visual QA. The raw edge-connected checkerboard was removed during
  final normalization.
- `generated/zorki-5-rollnote-raw-v1.png` is persisted. Its low common-revision
  body, oval center plate, left round window, right finder and sockets, top
  controls, horizontal wrap, collapsible-lens structure, hard monochrome
  linework, moderate depth, and geometric marks passed the first visual check.
  Its raw edge-connected checkerboard was removed during final normalization.
- `generated/kiev-iii-rollnote-raw-v1.png` is persisted. Its tall metered
  Contax-derived body, raised meter housing and top window, paired rectangular
  finder windows, integrated mount plate, self-timer, stabilizing foot, large
  top dials, hard monochrome linework, moderate depth, and local geometric
  marks passed visual QA. Its raw edge-connected checkerboard was removed
  during final normalization.
- Accepted finals:
  - `final/fed-1g-rollnote-v1.png`
  - `final/zorki-5-rollnote-v1.png`
  - `final/kiev-iii-rollnote-v1.png`
- Review boards:
  - `soviet-rangefinder-foundation-gaps-review-board-a-v1.png`
  - `soviet-rangefinder-foundation-gaps-review-board-b-v1.png`
- All accepted finals are 1536x1024, 8-bit RGBA, with binary alpha values
  0/255 and genuinely transparent backgrounds.
- Visual QA passed for front-view fidelity, complete isolated bodies, early
  RollNote hard black outlines, monochrome-forward shading, moderate depth,
  and local unreadable geometric trademark substitutions.
- `npm run build` passed on 2026-08-26 (`vite build`, 1877 modules,
  completed in 2.24s).
- Accepted finals and review boards were uploaded in RollNote-assets commit `5a6e870`; App mappings were not changed.

## Next action

Upload approved and completed in RollNote-assets commit `5a6e870`. App integration remains pending; preserve existing imageStub and rollback values when connecting.
