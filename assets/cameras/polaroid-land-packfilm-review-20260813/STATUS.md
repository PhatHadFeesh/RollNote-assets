# RollNote Polaroid Land / packfilm review - 2026-08-13

## Scope
- Polaroid Land Camera Model 95 representative
- Polaroid Automatic 100 representative
- Polaroid 600SE representative
- Polaroid Colorpack 80 representative
- Polaroid Passport / Miniportrait 402 representative

## Progress
- [x] Review folder created.
- [x] RollNote house-style reference copied.
- [x] Public reference search started.
- [x] Model 95 and Swinger Model 20 references downloaded from Wikimedia Commons.
- [x] Model 95 RollNote-style source generated.
- [x] Swinger Model 20 first candidate generated and rejected.
- [x] Model 95 alpha validation and preview board.
- [x] Automatic 100 and 600SE references downloaded from Wikimedia Commons.
- [x] Automatic 100 and 600SE RollNote-style sources generated.
- [x] Automatic 100 and 600SE transparent PNGs extracted and validated.
- [x] Colorpack and Passport / ID references and generation.
- [x] Colorpack and Passport / ID transparent PNGs extracted and validated.
- [x] Full five-camera v2 preview board and alpha validation.
- [ ] Remote upload and app connection.

## Accepted assets so far
- `polaroid-model95-rollnote-v1.png`
- `polaroid-automatic100-rollnote-v1.png`
- `polaroid-600se-rollnote-v1.png`
- `polaroid-colorpack80-rollnote-v1.png`
- `polaroid-passport402-rollnote-v1.png`

## Rejected assets
- `polaroid-swinger-rollnote-v1-rejected-display-base-shape.png`: cute style, but the generated body included a large display-base/tray form and departed too far from the real Model 20 compact shape.
- `polaroid-colorpack80-rollnote-v1-rejected-swinger-popup-shape.png`: pretty rendering, but the generated body leaned too much toward a Swinger / pop-up finder silhouette instead of the stricter Colorpack 80 box body.

## Reference basis
- Model 95 reference: `references/downloads/polaroid-model95-front-commons.jpg`
- Swinger Model 20 reference: `references/downloads/polaroid-swinger-model20-commons.jpg`
- Automatic 100 reference: `references/downloads/polaroid-automatic100-commons.jpg`
- 600SE reference: `references/downloads/polaroid-600se-commons.jpg`
- Colorpack 80 reference: `references/downloads/polaroid-colorpack80-commons.jpg`
- Passport / ID reference: `references/downloads/polaroid-passport402-commons.jpg`

## Quality notes
- Preview board: `polaroid-land-packfilm-preview-v2.png`
- Alpha validation: `validation-alpha-v2.json`
- Model 95 candidate keeps the tall brown leather rear body, black bellows, silver front board, folding bed, and metal support struts. Its slight depth angle is acceptable for a folding camera because it reveals the bellows and bed structure.
- Automatic 100 candidate keeps the black packfilm folding body, bellows, metal cross struts, top viewfinder/rangefinder, and front lens board. The front board is slightly simplified/polished but not a huge model mismatch at app-card size.
- 600SE candidate keeps the professional black rangefinder body, large lens, upper finder windows, hand grip, and packfilm back thickness.
- Colorpack 80 v2 candidate keeps the rigid black packfilm box, left film-door/latch strip, silver front faceplate, central lens, secondary circle, lower red stripe, and top finder. The top finder is still slightly more prominent than the real camera, but the accepted v2 no longer reads as Swinger / modern instant at app-card size.
- Passport 402 candidate keeps the four-lens ID camera face, side grip, black body, finder panel, and compact passport-camera identity.
- Swinger candidate is not accepted and must not be connected to the app.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths should remain `/assets/cameras/<file>.png` and be resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after upload.
- Do not bundle original camera PNGs in app builds; run GitHub-assets sync scripts after data changes.
- Production upload pending for this Land / packfilm batch.

## Rollback stub
- Before app connection, rejection requires removing the five production PNGs above and the review folder outputs from RollNote-assets. No `src/data.js` rollback is required until the imageUrl / variantAssets / imageStub changes are applied.
