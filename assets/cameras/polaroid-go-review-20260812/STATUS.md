# RollNote Polaroid Go review - 2026-08-12

## Scope
- Polaroid Go / Go Gen 2 representative
- Polaroid Go Gen 3 representative

## Accepted assets
- `polaroid-go-gen2-rollnote-v1.png`
- `polaroid-go-gen3-rollnote-v1.png`

## Reference basis
- The accepted assets were generated from official Polaroid Go Gen 2 and Gen 3 front reference images saved under `references/downloads/`.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.
- Gen 2 keeps the compact blue/white Go body, top shutter/viewfinder hump, front flash/lens/viewfinder cluster, lower film slot, and small Go proportions.
- Gen 3 keeps the lavender/purple body, darker top cap, red shutter, top-right viewfinder hump, black front optical band, ribbed central lens surround, flash/viewfinder windows, lower film slot, and tiny Go proportions.

## Quality check
- Reference board: `polaroid-go-reference-board-v1.jpg`
- Preview board: `polaroid-go-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The finals are RGBA PNGs with transparent corners and no baked background after local checkerboard-background removal.
- Visual check: both accepted assets use mostly front-facing views, preserve the real Go family silhouette, remain visibly smaller/squatter than full-size Polaroid Now models, and match the RollNote rounded light-cartoon style closely enough for app-card use.
- Note: the Gen 2 RollNote asset moves the rainbow stripe closer to the center than the official reference. This is acceptable for v1 at card size, but can be tightened in a future variant-specific refresh.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check is pending until this batch is copied to RollNote-assets, committed, pushed, and rechecked through GitHub raw / Pages URLs.

## Rollback stub
- Remove the accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_GO_REVIEW_PREVIEW_URL`, remove `cam-polaroid-go` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-go`.
