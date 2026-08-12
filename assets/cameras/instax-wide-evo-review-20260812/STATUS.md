# RollNote instax WIDE Evo review - 2026-08-12

## Scope
- Fujifilm instax WIDE Evo

## Accepted assets
- `instax-wide-evo-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from official Fujifilm / instax WIDE Evo product imagery saved under `references/downloads/`.
- The main official reference shows the real WIDE Evo front layout with the wide rectangular black body, central raised front plate, large circular lens, right-side stacked round controls, front lever, WIDE ANGLE switch, and top print slot.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `instax-wide-evo-reference-board-v1.jpg`
- Preview board: `instax-wide-evo-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a straight/front-facing viewpoint, keeps the real WIDE Evo body proportions and distinctive controls, and omits the emerging print so the app library icon stays compact and clean.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Publication check is pending until this batch is copied to RollNote-assets, committed, pushed, and rechecked through GitHub raw / Pages URLs.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `INSTAX_WIDE_EVO_REVIEW_PREVIEW_URL`, remove `cam-instax-wide-evo` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-instax-wide-evo`.
