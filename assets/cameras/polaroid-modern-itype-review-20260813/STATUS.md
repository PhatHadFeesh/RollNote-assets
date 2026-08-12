# RollNote Polaroid modern i-Type review - 2026-08-13

## Scope
- Impossible / Polaroid I-1 representative
- Polaroid Originals OneStep 2 representative
- Polaroid I-2 representative
- Polaroid Flip representative

## Accepted assets
- `polaroid-impossible-i1-rollnote-v1.png`
- `polaroid-onestep2-rollnote-v1.png`
- `polaroid-i2-rollnote-v1.png`
- `polaroid-flip-rollnote-v1.png`

## Reference basis
- The accepted assets were generated from real front-view references saved under `references/downloads/` where available.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, clean outlines, and app-card polish.
- I-1 keeps the black trapezoid body, large circular ring-flash lens module, top roll/door shape, side control panel, and lower print slot.
- OneStep 2 keeps the white rounded box body, black lower print-slot area, large central lens, flash/viewfinder blocks, red shutter, and rainbow accent. Minor note: the generated rainbow accent sits lower than the real product, but the model identity remains recognizable at card size.
- I-2 keeps a premium dark graphite body, large central lens, red shutter button, upper finder/flash cluster, and lower print slot. Minor note: the generated body is slightly more generic rounded than the real I-2, but it remains distinct from Now+ / Go / OneStep 2.
- Flip keeps the raised flip-up flash lid, rounded white/black body, central lens, front control details, color accent, and lower print slot.
- OneStep+ is not separately generated in this batch because reliable front reference capture was not available; it reuses OneStep 2 as a temporary close-family representative.

## Quality check
- Preview board: `polaroid-modern-itype-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The finals are RGBA PNGs with transparent corners and no opaque chroma-key residue after local background removal.
- Visual check: all accepted assets use mostly front-facing views, keep the real-model silhouettes distinct, omit packaging/film insert/straps, and remain consistent with the RollNote rounded light-cartoon style.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check is pending until this batch is committed, pushed, and rechecked through GitHub raw / Pages URLs.

## Rollback stub
- Remove the accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_MODERN_ITYPE_REVIEW_PREVIEW_URL`, remove or revert the new `cam-polaroid-modern-itype` entries in `CAMERA_VARIANT_ASSETS`, and restore `cam-polaroid-modern-itype.imageStub` to the previous `POLAROID_INSTANT_REVIEW_PREVIEW_URL` / `RollNote-assets 27f3ba7` state if needed.
