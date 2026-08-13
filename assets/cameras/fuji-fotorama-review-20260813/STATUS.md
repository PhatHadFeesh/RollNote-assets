# RollNote Fujifilm Fotorama review - 2026-08-13

## Scope
- Fujifilm Fotorama FP-1 / FP-14 / FP-100 representative bodies
- Fujifilm Fotorama 800 / 850E / 880 representative bodies
- Fujifilm Fotorama 90ACE / MX800 / SlimACE / Mr. Handy Ace representative bodies

## Progress
- [x] Review folder created.
- [x] RollNote house-style reference copied.
- [x] Initial real references downloaded for FP-1, FP-UL-style folding body, and Fotorama 800AF.
- [x] Download or save additional real references for FP-14 / FP-100, 850E / 880, 90ACE / MX800 / SlimACE / Mr. Handy Ace where available.
- [x] Create real-reference board.
- [ ] Generate RollNote-style sources on removable chroma-key backgrounds.
- [ ] Extract transparent PNGs and validate alpha.
- [ ] Create preview board.
- [ ] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

## Existing references
- RollNote house-style reference: `references/downloads/style-reference-rollnote.png`
- FP-1 reference: `references/downloads/fuji-fotorama-fp1-wikimedia.jpg`
- FP-UL / folding-pack representative reference: `references/downloads/fuji-fotorama-fpul-analogforever.jpg`
- Fotorama 800AF reference: `references/downloads/fuji-fotorama-800af-analogforever.jpg`
- Fotorama 90ACE reference: `references/downloads/fuji-fotorama-90ace-analogforever.jpg`
- Fotorama MX800 reference: `references/downloads/fuji-fotorama-mx800-ebay-front.webp`
- Fotorama SlimACE reference: `references/downloads/fuji-fotorama-slimace-analogforever.jpg`
- Fotorama Mr. Handy MF / Mr. Handy Ace representative reference: `references/downloads/fuji-fotorama-mr-handy-mf-analogforever.jpg`
- Real-reference board: `fuji-fotorama-real-reference-board-v1.png`

## Quality target
- Use real camera references for model identity and RollNote's rounded light-cartoon style for rendering.
- Prefer straight/front-facing views unless folding packfilm bodies need slight depth to read correctly.
- Keep transparent PNG finals; generate on flat chroma-key and remove locally.
- Avoid readable logos, model text, packaging, hands, straps, and baked shadows.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and be resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.
- Do not bundle original camera PNGs in app builds; run GitHub-assets sync scripts after data changes.
- No production assets from this Fotorama batch have been generated, uploaded, or connected yet.

## Rollback stub
- This batch is not connected yet. If abandoned, remove `public/assets/cameras/fuji-fotorama-review-20260813`; no `src/data.js` rollback is required.
