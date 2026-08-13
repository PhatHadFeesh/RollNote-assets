# RollNote instax mini early review - 2026-08-13

## Scope
- Fujifilm instax mini 10
- Fujifilm instax mini 20 / 20 Cheki
- Fujifilm instax mini 25
- Fujifilm instax mini 30
- Fujifilm instax mini 50 / 50S
- Fujifilm instax mini 55
- Fujifilm instax mini 70

## Progress
- [x] Review folder created.
- [x] RollNote house-style reference copied.
- [x] Download or save real front references.
- [x] Create real-reference board.
- [x] Generate RollNote-style sources on removable chroma-key backgrounds.
- [x] Extract transparent PNGs and validate alpha.
- [x] Create preview board.
- [x] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

## Quality target
- Use real camera references for model identity and RollNote rounded light-cartoon style for rendering.
- Prefer straight/front-facing views unless small depth helps distinguish body forms.
- Keep transparent PNG finals and avoid readable logos/model text.

## Reference basis
- Official instax history references downloaded under `references/downloads/` for mini 10, mini 20, mini 25, mini 30, mini 50, mini 50S, mini 55, and mini 70.
- Reference board: `instax-mini-early-reference-board-v1.png`.
- Board order: mini 10, mini 20, mini 25 original, mini 25 later, mini 30, mini 50, mini 50S, mini 55, mini 70, RollNote style reference.

## Generated assets
- `instax-mini10-rollnote-v1.png`
- `instax-mini20-rollnote-v1.png`
- `instax-mini25-rollnote-v1.png`
- `instax-mini30-rollnote-v1.png`
- `instax-mini50-rollnote-v1.png`
- `instax-mini50s-rollnote-v1.png`
- `instax-mini55-rollnote-v1.png`
- `instax-mini70-rollnote-v1.png`
- Preview board: `instax-mini-early-preview-v1.png`

## Quality check
- All final PNGs have alpha channels and transparent backgrounds.
- Visual preview keeps the real front layouts and rounded RollNote cartoon style. mini 25 is acceptable but appears smaller on the preview board because the source composition is more generously padded; mark it for optional user review before replacing.

## App connection
- Remote asset commit: `RollNote-assets 9f4f4a7`
- App data: `src/data.js` adds `INSTAX_MINI_EARLY_REVIEW_PREVIEW_URL`, `CAMERA_VARIANT_ASSETS["cam-instax-mini-early"]`, parent `imageUrl`, and `imageStub` rollback metadata.
- Variant mapping: mini 10, 20, 25, 30, 50, 50S, 55, and 70 use their own assets; mini 20 Cheki reuses the mini 20 representative.
- GitHub Raw URLs verified 200 immediately after push. GitHub Pages URLs were still 404 during the first post-push check and need a later propagation recheck.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and resolve through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.

## Rollback stub
- Remove `imageUrl` / `imageStub` from `cam-instax-mini-early`, remove `cam-instax-mini-early` from `CAMERA_VARIANT_ASSETS`, and remove this batch's production PNGs if rejected. The previous image state was `prompt-ready` with no `imageUrl`.
