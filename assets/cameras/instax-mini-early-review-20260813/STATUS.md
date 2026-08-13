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
- [ ] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

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

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and resolve through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.

## Rollback stub
- This batch is not connected yet. If abandoned, remove `public/assets/cameras/instax-mini-early-review-20260813`; no `src/data.js` rollback is required.
