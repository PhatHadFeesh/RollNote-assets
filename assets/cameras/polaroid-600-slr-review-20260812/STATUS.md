# RollNote Polaroid 600 SLR review - 2026-08-12

## Scope
- Polaroid SLR 680 / SLR 680 SE / SLR 690 representative

## Accepted assets
- `polaroid-600-slr-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from public Polaroid SLR 680 / 680 SE / 690 front-view product references saved under `references/downloads/`.
- The main reference shows the 600 SLR family layout: black folding body in open shooting position, upper flash panel, rectangular flash window, central gold sonar disk, ribbed texture on the upper body, lower central lens, red shutter button, dark round button, hinge details, and bottom 600 film door.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `polaroid-600-slr-reference-board-v1.jpg`
- Preview board: `polaroid-600-slr-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a straight/front-facing viewpoint, keeps the SLR 680 / 690 flash-and-sonar folding form distinct from SX-70 Original, Sun 660 AF, and ordinary 600 box cameras, and abstracts readable labels into non-readable marks.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check is pending until this batch is copied to RollNote-assets, committed, pushed, and rechecked through GitHub raw / Pages URLs.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_600_SLR_REVIEW_PREVIEW_URL`, remove `cam-polaroid-600-slr` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-600-slr`.
