# RollNote instax SQUARE analog review - 2026-08-12

## Scope
- Fujifilm instax SQUARE SQ1
- Fujifilm instax SQUARE SQ6
- Fujifilm instax SQUARE SQ6 black-gold special abstract variant
- Fujifilm instax SQUARE SQ40

## Accepted assets
- `instax-sq1-rollnote-v1.png`
- `instax-sq6-rollnote-v1.png`
- `instax-sq6-special-black-gold-rollnote-v1.png`
- `instax-sq40-rollnote-v1.png`

## Reference basis
- SQ1 and SQ40 were checked against official instax front-facing product images.
- SQ6 was checked against an official Fujifilm product overview reference.
- The black-gold special asset uses the SQ6 body geometry plus an abstract non-readable black-and-gold manuscript texture. It is intentionally not generated from a public-figure reference image.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `instax-square-reference-board-v2.jpg`
- Preview board: `instax-square-analog-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- All four finals are RGBA PNGs with transparent corners and no opaque chroma-key pixels.
- Visual check: all accepted assets use a mostly straight/front-facing viewpoint, keep the real SQUARE analog silhouettes and lens/finder/flash/control layout, and follow the current rounded RollNote cartoon style.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check at 2026-08-12 14:38 CST: GitHub raw URLs for the new files returned 200, existing GitHub Pages assets returned 200, but the new GitHub Pages URLs still returned 404. Treat this as a Pages propagation/build delay unless it persists across later checks.

## Rollback stub
- Remove the four accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `INSTAX_SQUARE_ANALOG_REVIEW_PREVIEW_URL`, remove `cam-instax-square-analog` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-instax-square-analog`.
