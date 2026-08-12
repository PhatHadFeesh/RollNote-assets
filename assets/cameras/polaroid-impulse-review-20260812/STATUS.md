# RollNote Polaroid Impulse review - 2026-08-12

## Scope
- Polaroid Impulse / Impulse Portrait / Impulse AF representative

## Accepted assets
- `polaroid-impulse-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from Wikimedia Commons Polaroid Impulse references saved under `references/downloads/`.
- Invalid downloads and HTML/placeholder responses were moved to `references/rejected-downloads/` and not used for the final reference board.
- The main reference shows the Impulse family layout: low horizontal wedge body, raised flash tower at upper left, three front windows, broad gray-blue lower film door, bottom film exit slot, thin red accent line, and protruding right grip shape.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `polaroid-impulse-reference-board-v1.jpg`
- Preview board: `polaroid-impulse-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a front-oriented view, keeps the Impulse wedge body and raised flash tower distinct from ordinary 600 box cameras, and abstracts readable labels into non-readable marks.
- Rejected candidate retained: `rejected/polaroid-impulse-v1-rejected-black-background.png`, rejected because the background was black/gradient instead of removable chroma key.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check at 2026-08-12 19:24 CST: GitHub raw URLs and GitHub Pages URLs for the production PNG, preview board, and STATUS all returned 200, and `npm run ios:sync:github-assets` completed with no remote library originals bundled into `dist` or iOS. The batch is fully reachable through the remote asset base.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_IMPULSE_REVIEW_PREVIEW_URL`, remove `cam-polaroid-impulse` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-impulse`.
