# Status

## Batch

- Name: Kodak and Lomography parent-variant gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Completed models

- Kodak Ultra F9
- Lomo'Instant
- Lomo'Instant Wide
- Lomography Konstruktor F

A fresh full-library filename and inventory search found no qualified image for these four variants before generation. Lomo'Instant Square was excluded because it is the already completed Square Glass hardware, so another candidate would duplicate an accepted model.

## Final assets

- `final/ultra-f9-rollnote-v1.png`
- `final/lomo-instant-rollnote-v1.png`
- `final/lomo-instant-wide-rollnote-v1.png`
- `final/konstruktor-rollnote-v1.png`

All four files are 1536x1024, 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `kodak-lomo-parent-gaps-review-board-a-v1.png`: Kodak Ultra F9 and Lomo'Instant
- `kodak-lomo-parent-gaps-review-board-b-v1.png`: Lomo'Instant Wide and Lomography Konstruktor F

## Quality control

- Two real references from official, specialist-retailer, or established used-camera retailer pages are retained for every model with exact source URLs.
- All four candidates use an exact front view with one isolated camera and no strap, hands, packaging, floor, or cast shadow.
- Ultra F9 retains the wide yellow-and-black shell, top black module, centered finder, right flash, circular lens, front slider, and left strap lug.
- Lomo'Instant retains its tall portrait body, left finder column, upper flash, round front sensor/button, central lens, and lower controls. Detachable accessory lenses from the reference set are omitted.
- Lomo'Instant Wide retains its broad black body, left finder, central flash, paired sensors, projecting central lens, front control, and side lugs.
- Konstruktor F retains its DIY SLR proportions, waist-level finder hood, twin top knobs, central lens and ribbed focus ring, front control, panel seams, and side hardware.
- The accepted candidates follow the early RollNote treatment: hard black outer contours, crisp internal linework, monochrome-forward shading, modest rounding, moderate lens/body depth, and only necessary recognition color.
- Brand names, model wording, logos, lens inscriptions, and instructional labels are replaced locally with crisp unreadable geometric marks. No full-camera blur was applied.
- Edge-connected generated checkerboards were removed without flattening internal highlights. Dimensions, RGBA encoding, transparency, framing, and review-board model pairing were verified.
- Three Konstruktor packaging/parts references were moved to `rejected/`; only assembled-camera references were used.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules transformed).

## Next candidates

After another full-library duplicate check, a useful next group is original LOMO LC-A, LC-A 120, original Diana, and Diana Baby 110. Existing qualified assets already cover LC-A+, LC-Wide, Diana F+, Diana Mini, and Diana Instant Square and must not be regenerated.
