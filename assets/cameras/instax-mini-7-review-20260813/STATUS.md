# RollNote instax mini 7 review - 2026-08-13

## Scope
- Fujifilm instax mini 7
- Fujifilm instax mini 7S
- Fujifilm instax mini 7+
- Fujifilm instax mini 7+ Popn Toy
- Fujifilm instax mini 7+ Popn Pastel

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
- Official instax history references downloaded under `references/downloads/` for mini 7, mini 7+ Popn Toy, mini 7+ Popn Pastel, and mini 7S.
- Reference board: `instax-mini-7-reference-board-v1.png`.
- Board order: mini 7 blue, mini 7 pink, mini 7 pearl white, mini 7 orange, mini 7 mint, Popn Toy, Popn Pastel, mini 7S choco, mini 7S white, RollNote style reference.
- Generation plan: use one representative for basic mini 7 color variants, one for mini 7S, and separate representatives for Popn Toy and Popn Pastel because the front graphics/color layouts are visibly different.

## Generated assets
- `instax-mini7-rollnote-v1.png`
- `instax-mini7s-rollnote-v1.png`
- `instax-mini7-popn-toy-rollnote-v1.png`
- `instax-mini7-popn-pastel-rollnote-v1.png`
- Preview board: `instax-mini-7-preview-v1.png`

## Quality check
- All final PNGs have alpha channels and transparent backgrounds.
- Visual preview keeps the real front layouts and rounded RollNote cartoon style. mini 7 and mini 7+ share the blue mini 7 representative for now; Popn Toy and Popn Pastel use separate representative art because their front graphics and color layouts are distinct.

## App connection
- Remote asset commit: `RollNote-assets 0ca593e`
- App data: `src/data.js` adds `INSTAX_MINI_7_REVIEW_PREVIEW_URL`, `CAMERA_VARIANT_ASSETS["cam-instax-mini-7-series"]`, parent `imageUrl`, and `imageStub` rollback metadata.
- Variant mapping: mini 7 and mini 7+ use the blue mini 7 representative; mini 7S, mini 7+ Popn Toy, and mini 7+ Popn Pastel switch to their own assets.
- GitHub Raw URLs verified 200 immediately after push. GitHub Pages URLs initially returned 404 during propagation, then returned 200 for all production PNGs, the preview board, and STATUS on follow-up.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and resolve through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.

## Rollback stub
- Remove `imageUrl` / `imageStub` from `cam-instax-mini-7-series`, remove `cam-instax-mini-7-series` from `CAMERA_VARIANT_ASSETS`, and remove this batch's production PNGs if rejected. The previous image state was `prompt-ready` with no `imageUrl`.
