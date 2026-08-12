# RollNote Polaroid i-Zone / Pocket review - 2026-08-13

## Scope
- Polaroid i-Zone original representative
- Polaroid i-Zone 200 representative
- Polaroid Mio / Xiao / Pocket representative

## Accepted assets
- `polaroid-izone-original-rollnote-v1.png`
- `polaroid-izone200-rollnote-v1.png`
- `polaroid-mio-rollnote-v1.png`

## Reference basis
- The accepted assets were generated from real front-view i-Zone original, i-Zone 200, Mio, and Xiao references saved under `references/downloads/`.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, clean outlines, and app-card polish.
- i-Zone original keeps the long low pastel body, black curved bottom, yellow top pop-up button, large left viewfinder/opening, central black oval lens/sensor module, and right flash.
- i-Zone 200 keeps the rounded white compact body, blue textured front grip panel, left flash, central lens in a white raised recess, right viewfinder, and silver top shutter.
- Mio / Xiao keeps the vertical silver rounded body, large right lens ring, upper-left flash/viewfinder cluster, sensor slot, and curved left black grip.

## Quality check
- Reference board: `polaroid-izone-pocket-reference-board-v1.jpg`
- Preview board: `polaroid-izone-pocket-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The finals are RGBA PNGs with transparent corners and no baked background after local checkerboard-background removal.
- Visual check: all accepted assets use mostly front-facing views, keep the real-model silhouettes distinct across i-Zone original, i-Zone 200, and Mio / Xiao, omit packaging/film insert/straps, and remain consistent with the RollNote rounded light-cartoon style.
- Note: the original i-Zone and i-Zone 200 are naturally long and low, so they appear smaller than square instant cameras in a square card. This preserves real proportions.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Uploaded to RollNote-assets commit `c6a2d77`.
- Raw GitHub URLs returned 200 after upload.
- GitHub Pages URLs returned 200 on the 2026-08-13 propagation check for the three production PNGs, preview board, and STATUS file.
- `src/data.js` is connected through `imageUrl`, `variantAssets`, and `imageStub.remoteAssetCommit`.
- `npm run ios:sync:github-assets` completed after connection and confirmed no remote library asset originals were bundled into dist or iOS.

## Rollback stub
- Remove the accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_IZONE_POCKET_REVIEW_PREVIEW_URL`, remove `cam-polaroid-izone-pocket` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-izone-pocket`.
