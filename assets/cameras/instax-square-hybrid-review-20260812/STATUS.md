# RollNote instax SQUARE hybrid review - 2026-08-12

## Scope
- Fujifilm instax SQUARE SQ10
- Fujifilm instax SQUARE SQ20

## Accepted assets
- `instax-sq10-rollnote-v1.png`
- `instax-sq20-rollnote-v1.png`

## Reference basis
- SQ10 was checked against a clear front-facing public product image.
- SQ20 was checked against a Fujifilm product reference saved from the Uruguay official product page.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `instax-square-hybrid-reference-board-v1.jpg`
- Preview board: `instax-square-hybrid-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- Both finals are RGBA PNGs with transparent corners and no opaque chroma-key pixels.
- Visual check: both accepted assets use a mostly straight/front-facing viewpoint. SQ10 keeps the large silver lens disk and SQ20 keeps the dark recessed lens bowl and diagonal front buttons, so the two hybrid models remain distinct.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check at 2026-08-12 15:02 CST: GitHub raw URLs for the two new files returned 200, and `npm run ios:sync:github-assets` completed with no remote library originals bundled into `dist` or iOS. The new GitHub Pages URLs still returned 404 immediately after push, so recheck Pages propagation in the next heartbeat.

## Rollback stub
- Remove the two accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `INSTAX_SQUARE_HYBRID_REVIEW_PREVIEW_URL`, remove `cam-instax-square-hybrid` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-instax-square-hybrid`.
