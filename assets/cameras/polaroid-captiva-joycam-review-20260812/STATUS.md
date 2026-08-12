# RollNote Polaroid Captiva / JoyCam review - 2026-08-12

## Scope
- Polaroid Captiva / Vision representative
- Polaroid JoyCam / PopShots / 500 representative

## Accepted assets
- `polaroid-captiva-rollnote-v1.png`
- `polaroid-joycam-rollnote-v1.png`

## Reference basis
- The accepted assets were generated from real front-view Polaroid Captiva SLR and JoyCam references saved under `references/downloads/`.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, clean outlines, and app-card polish.
- Captiva keeps the wide matte-black body, left protruding flash block, central lens in a broad oval recess, top latch, right-hand grip, and long horizontal silhouette.
- JoyCam keeps the related wide matte-black body, left flash block, smaller central lens/recess, simpler front panel, top latch, and right-hand grip.

## Quality check
- Reference board: `polaroid-captiva-joycam-reference-board-v1.jpg`
- Preview board: `polaroid-captiva-joycam-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The finals are RGBA PNGs with transparent corners and no baked background after local checkerboard-background removal.
- Visual check: both accepted assets use mostly front-facing views, preserve the real long horizontal Captiva/JoyCam silhouettes, avoid the rejected strap candidate, and remain consistent with the RollNote rounded light-cartoon style.
- Note: these models are naturally long and low, so they appear smaller than square instant cameras in a square card. This preserves real proportions.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Uploaded to RollNote-assets in commit `ddfc0c2`.
- Raw GitHub URLs returned 200 for both production PNGs, the preview board, and STATUS at the 2026-08-12 23:27 CST heartbeat.
- GitHub Pages URLs returned 200 for both production PNGs, the preview board, and STATUS after propagation at the 2026-08-12 23:58 CST heartbeat.
- `npm run ios:sync:github-assets` completed and confirmed `No remote library asset originals found for dist.` and `No remote library asset originals found for ios.`
- `src/data.js` is connected to the remote paths with `imageUrl`, `variantAssets`, and a rollback-capable `imageStub`.

## Rollback stub
- Remove the accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_CAPTIVA_JOYCAM_REVIEW_PREVIEW_URL`, remove `cam-polaroid-captiva-joycam` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-captiva-joycam`.
