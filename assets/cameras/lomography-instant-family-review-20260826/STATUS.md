# Status

## Batch

- Name: Lomography instant family
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Completed models

- Lomo'Instant Automat Glass
- Lomo'Instant Square Glass
- Lomo'Instant Wide Glass
- Diana Instant Square

A fresh full-library filename and data search found inventory variant names but no existing qualified image for these four variants before generation.

## Final assets

- `final/automat-glass-rollnote-v1.png`
- `final/square-glass-rollnote-v1.png`
- `final/wide-glass-rollnote-v1.png`
- `final/diana-instant-rollnote-v1.png`

All four are 1536x1024 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `lomography-instant-family-review-board-a-v1.png`
- `lomography-instant-family-review-board-b-v1.png`

## Quality control

- Two real references from The Camera Store product data are retained for every model, together with exact source URLs.
- Exact front view is used for Automat Glass, Wide Glass, and Diana Instant Square.
- Square Glass uses a restrained near-front angle because its projecting lens board and folding bellows are structurally defining.
- Automat Glass retains its tall black proportions, faceted shell texture, left finder/flash column, front controls, large glass lens, orange identification ring, and lower rectangular button.
- Square Glass retains its broad upper housing, left flash/finder/control cluster, right finder, folding bellows, projecting square lens board, and textured panels.
- Wide Glass retains its very wide silver body, black grip panels, left finder, central flash, two sensors, large glass lens, shutter control, and side lugs.
- Diana Instant Square retains its cyan upper shell, raised finder, square center panel, textured black grips, circular lens plate, and mounted oversized flash.
- Logos, brand wording, model wording, numbers, and instructional labels are replaced locally with crisp unreadable geometric marks. No full-camera blur was applied.
- Edge-connected generated checkerboards were removed. Final dimensions, RGBA encoding, alpha, framing, and review-board model pairing were visually verified.
- The first Automat generation call stalled without producing a file. A later over-wide candidate was retained in `rejected/`; corrected v2 became the accepted raw source. No accepted candidate was regenerated.
- Invalid or redundant references remain in `rejected/` for auditability.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules transformed).

## Next candidates

After a fresh full-library check, the next review group can complete missing child variants under the same inventory parents: original Lomo'Instant, original Lomo'Instant Square, original Lomo'Instant Wide, and Lomography Konstruktor. Lomo'Instant Automat already has a qualified review asset and must not be regenerated.
