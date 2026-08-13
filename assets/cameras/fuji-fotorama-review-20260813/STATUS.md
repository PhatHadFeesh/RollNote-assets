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
- [x] Generate RollNote-style sources on removable chroma-key backgrounds.
- [x] Extract transparent PNGs and validate alpha.
- [x] Create preview board.
- [x] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

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

## Generated assets
- `fuji-fotorama-fp1-rollnote-v1.png`
- `fuji-fotorama-fpul-rollnote-v1.png`
- `fuji-fotorama-800af-rollnote-v1.png`
- `fuji-fotorama-90ace-rollnote-v1.png`
- `fuji-fotorama-mx800-rollnote-v1.png`
- `fuji-fotorama-slimace-rollnote-v1.png`
- `fuji-fotorama-mr-handy-ace-rollnote-v1.png`
- Preview board: `fuji-fotorama-preview-v1.png`

## App connection
- Remote asset commit: `RollNote-assets 07f6abd`
- App data: `src/data.js` adds `FUJI_FOTORAMA_REVIEW_PREVIEW_URL`, `CAMERA_VARIANT_ASSETS["cam-fuji-fotorama"]`, parent `imageUrl`, and `imageStub` rollback metadata.
- Variant mapping: FP-1 uses its own asset; FP-14 / FP-100 reuse the FP-UL-style folding representative; Fotorama 800 / 850E / 880 reuse the 800AF representative; 90ACE, MX800, SlimACE, and Mr. Handy Ace each use their own asset.
- GitHub Raw URLs verified 200 immediately after push. GitHub Pages URLs were still 404 during the first post-push check and need a later propagation recheck.

## Quality target
- Use real camera references for model identity and RollNote's rounded light-cartoon style for rendering.
- Prefer straight/front-facing views unless folding packfilm bodies need slight depth to read correctly.
- Keep transparent PNG finals; generate on flat chroma-key and remove locally.
- Avoid readable logos, model text, packaging, hands, straps, and baked shadows.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and be resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.
- Do not bundle original camera PNGs in app builds; run GitHub-assets sync scripts after data changes.
- Production assets from this Fotorama batch were uploaded to RollNote-assets and app-connected on 2026-08-13. App paths remain `/assets/cameras/<file>.png` and resolve through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` in GitHub-assets builds.

## Rollback stub
- Remove `imageUrl` / `imageStub` from `cam-fuji-fotorama`, remove `cam-fuji-fotorama` from `CAMERA_VARIANT_ASSETS`, and remove this batch's production PNGs if rejected. The previous image state was `prompt-ready` with no `imageUrl`.
