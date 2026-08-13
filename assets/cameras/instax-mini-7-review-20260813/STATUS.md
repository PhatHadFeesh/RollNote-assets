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
- [ ] Generate RollNote-style sources on removable chroma-key backgrounds.
- [ ] Extract transparent PNGs and validate alpha.
- [ ] Create preview board.
- [ ] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

## Quality target
- Use real camera references for model identity and RollNote rounded light-cartoon style for rendering.
- Prefer straight/front-facing views unless small depth helps distinguish body forms.
- Keep transparent PNG finals and avoid readable logos/model text.

## Reference basis
- Official instax history references downloaded under `references/downloads/` for mini 7, mini 7+ Popn Toy, mini 7+ Popn Pastel, and mini 7S.
- Reference board: `instax-mini-7-reference-board-v1.png`.
- Board order: mini 7 blue, mini 7 pink, mini 7 pearl white, mini 7 orange, mini 7 mint, Popn Toy, Popn Pastel, mini 7S choco, mini 7S white, RollNote style reference.
- Generation plan: use one representative for basic mini 7 color variants, one for mini 7S, and separate representatives for Popn Toy and Popn Pastel because the front graphics/color layouts are visibly different.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and resolve through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.

## Rollback stub
- This batch is not connected yet. If abandoned, remove `public/assets/cameras/instax-mini-7-review-20260813`; no `src/data.js` rollback is required.
