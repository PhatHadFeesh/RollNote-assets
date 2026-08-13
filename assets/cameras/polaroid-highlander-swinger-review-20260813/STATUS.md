# RollNote Polaroid Highlander / Swinger review - 2026-08-13

## Scope
- Polaroid Model 80 Highlander / 80A / 80B representative
- Polaroid J33 / J66 Electric Eye representatives
- Polaroid Model 20 Swinger representative
- Polaroid Swinger II / Big Swinger 3000 / Zip representatives

## Progress
- [x] Review folder created.
- [x] RollNote house-style reference copied.
- [x] Existing Swinger Model 20 real reference copied from the Land / packfilm batch.
- [x] Previously rejected Swinger candidate copied into this review folder for recovery context.
- [x] Download or save additional real references for Model 80 Highlander, J33 / J66, Swinger II, Big Swinger 3000, and Zip.
- [x] Generate RollNote-style sources on removable chroma-key backgrounds.
- [x] Extract transparent PNGs and validate alpha.
- [x] Create preview board.
- [x] Upload accepted assets to RollNote-assets and connect app data with imageStub rollback notes.

## Existing references
- Swinger Model 20 reference: `references/downloads/polaroid-swinger-model20-commons.jpg`
- RollNote house-style reference: `references/downloads/style-reference-rollnote.png`
- Model 80 Highlander reference: `references/downloads/polaroid-model80-highlander-appaphot.jpg`
- J33 reference: `references/downloads/polaroid-j33-purephoto.webp`
- J66 reference: `references/downloads/polaroid-j66-museums-victoria.jpg`
- Swinger II reference: `references/downloads/polaroid-swinger-ii-instantoptions.jpg`
- Big Swinger 3000 reference: `references/downloads/polaroid-big-swinger3000-ebay.jpg`
- Zip reference: `references/downloads/polaroid-zip-ebay.png`

## Accepted transparent assets
- `final/polaroid-model80-highlander-rollnote-v1.png`
- `final/polaroid-j33-rollnote-v1.png`
- `final/polaroid-j66-rollnote-v1.png`
- `final/polaroid-swinger-model20-rollnote-v1.png`
- `final/polaroid-swinger-ii-rollnote-v1.png`
- `final/polaroid-big-swinger3000-rollnote-v1.png`
- `final/polaroid-zip-rollnote-v1.png`

## Review boards
- Real references: `polaroid-highlander-swinger-real-reference-board.png`
- RollNote preview: `polaroid-highlander-swinger-preview-v1.png`

## Quality check - 2026-08-13 11:04 CST
- Real references were used per child-body family.
- The generated set keeps RollNote's rounded, light-cartoon app style and uses mostly straight/front views.
- Transparent PNG validation passed with alpha channels and transparent corners for all seven finals.
- No generated asset was connected before upload.
- Uploaded to RollNote-assets commit `ce7c674`.
- App `src/data.js` now maps Highlander / Swinger child variants to remote-resolved `/assets/cameras/*.png` URLs and keeps an `imageStub` rollback note.

## Rejected carryover
- `rejected/polaroid-swinger-rollnote-v1-rejected-display-base-shape.png`: cute style, but it included a large display-base/tray form and departed too far from the real Model 20 compact shape. Do not reuse this candidate.

## Quality target
- Use real camera references for model identity and RollNote's rounded light-cartoon style for rendering.
- Prefer straight/front-facing views unless a specific folding or odd body shape needs slight depth to read correctly.
- Keep transparent PNG finals; generate on flat chroma-key and remove locally.
- Avoid readable logos, model text, packaging, hands, straps, and baked shadows.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and be resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.
- Do not bundle original camera PNGs in app builds; run GitHub-assets sync scripts after data changes.
- Production assets are uploaded to RollNote-assets commit `ce7c674` and connected in the app through remote-resolved asset paths.

## Rollback stub
- Before app connection, remove `public/assets/cameras/polaroid-highlander-swinger-review-20260813` and the seven root-level `public/assets/cameras/polaroid-*-rollnote-v1.png` files for this batch.
- After app connection, also remove `POLAROID_HIGHLANDER_SWINGER_REVIEW_PREVIEW_URL`, remove `cam-polaroid-highlander-swinger` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from the Highlander / Swinger parent entry in `src/data.js`.
