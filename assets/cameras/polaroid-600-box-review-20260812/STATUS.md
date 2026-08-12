# RollNote Polaroid 600 box review - 2026-08-12

## Scope
- Polaroid 600 box cameras representative

## Accepted assets
- `polaroid-600-box-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from public Polaroid OneStep 600 / Spirit 600 / Sun 600 family references saved under `references/downloads/`.
- The main reference shows the common 600 box front layout: black top flash housing, upper-right flash window, upper-left brand panel, bridge gap, silver lower front plate, lens/sensor module, right viewfinder/control module, red side shutter button, and bottom film exit slot.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `polaroid-600-box-reference-board-v1.jpg`
- Preview board: `polaroid-600-box-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a straight/front-facing viewpoint, keeps the 600 box camera family proportions and distinctive front modules, and abstracts readable labels into non-readable marks.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check at 2026-08-12 18:26 CST: GitHub raw URLs for the new file, preview board, and STATUS returned 200, and `npm run ios:sync:github-assets` completed with no remote library originals bundled into `dist` or iOS. The new GitHub Pages URLs still returned 404 immediately after push, so recheck Pages propagation in the next heartbeat.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_600_BOX_REVIEW_PREVIEW_URL`, remove `cam-polaroid-600-box` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-600-box`.
