# RollNote instax WIDE review - 2026-08-12

## Scope
- Fujifilm instax WIDE 100
- Fujifilm instax WIDE 200
- Fujifilm instax WIDE 210
- Fujifilm instax WIDE 300
- Fujifilm instax WIDE 400
- Fujifilm instax WIDE 500AF

## Accepted assets
- `instax-wide100-rollnote-v1.png`
- `instax-wide200-rollnote-v1.png`
- `instax-wide210-rollnote-v1.png`
- `instax-wide300-rollnote-v1.png`
- `instax-wide400-rollnote-v1.png`
- `instax-wide500af-rollnote-v1.png`

## Reference basis
- WIDE 300 and WIDE 400 were checked against official Fujifilm / instax product images.
- WIDE 100, WIDE 200, WIDE 210, and WIDE 500AF were checked against public front-facing product references saved under `references/downloads/`.
- WIDE 200 and WIDE 210 intentionally remain visually close because the real bodies are close relatives; the WIDE 210 keeps the darker body finish and small front-layout differences.

## Quality check
- Preview board: `instax-wide-preview-v2.png`
- Alpha validation: `validation-alpha-v1.json`
- All six finals are RGBA PNGs with transparent corners and no opaque chroma-key pixels.
- Visual check: all accepted assets use a mostly straight/front-facing viewpoint, keep the real camera silhouette and lens/finder/flash layout, and follow the current rounded RollNote cartoon style.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.

## Rollback stub
- Remove the six files above from RollNote-assets if rejected.
- In `src/data.js`, remove `INSTAX_WIDE_REVIEW_PREVIEW_URL`, remove the new `CAMERA_VARIANT_ASSETS` mappings for `cam-instax-wide-analog` and `cam-instax-wide-500af`, and remove the `imageUrl` / `imageStub` fields from those two camera entries.
