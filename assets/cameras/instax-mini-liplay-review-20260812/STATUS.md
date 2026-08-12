# RollNote instax mini LiPlay review - 2026-08-12

## Scope
- Fujifilm instax mini LiPlay

## Accepted assets
- `instax-mini-liplay-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from official Fujifilm / instax mini LiPlay product imagery saved under `references/downloads/`.
- The official hero reference shows the current mini LiPlay body proportions and color options; the accepted asset uses the soft matcha-green front as the default library image.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `instax-mini-liplay-reference-board-v1.jpg`
- Preview board: `instax-mini-liplay-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a mostly straight/front-facing viewpoint, keeps the real mini LiPlay vertical rounded body, square lens module, and lower round button, and follows the current rounded RollNote cartoon style.
- Rejected candidate retained: `rejected/instax-liplay-rollnote-v1-rejected-readable-microphone-icon.png`, rejected because the lower button included a readable microphone symbol.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `INSTAX_MINI_LIPLAY_REVIEW_PREVIEW_URL`, remove `cam-instax-mini-liplay` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-instax-mini-liplay`.
