# RollNote Polaroid Spectra / Image review - 2026-08-12

## Scope
- Polaroid Spectra / Image System representative

## Accepted assets
- `polaroid-spectra-rollnote-v1.png`

## Reference basis
- The accepted asset was generated from Wikimedia Commons Polaroid Spectra / Image references saved under `references/downloads/`.
- Invalid downloads and HTML/empty responses were moved to `references/rejected-downloads/` and not used for the final reference board.
- The main reference shows the Spectra family layout: very wide low wedge body, open recessed gap behind the front module, front optical block with perforated grille, large lens window, smaller sensor/viewfinder windows, far-right flash, broad front film door, bottom exit slot, and right-side sloped grip form.
- The accepted RollNote house-style camera illustration was used as the style reference for rounded linework, tactile highlights, and collectible app-card polish.

## Quality check
- Reference board: `polaroid-spectra-reference-board-v1.jpg`
- Preview board: `polaroid-spectra-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- The final is an RGBA PNG with transparent corners and no opaque chroma-key pixels.
- Visual check: the accepted asset uses a front-oriented slight-side-depth view, keeps the Spectra / Image wide low body distinct from ordinary 600 box, Impulse, SLR 680, and modern Go cameras, and abstracts readable labels into non-readable marks.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.
- Uploaded to RollNote-assets in commit `91998dd`.
- Raw GitHub URLs returned 200 for the production PNG, preview board, and STATUS at the 2026-08-12 21:26 CST heartbeat.
- GitHub Pages URLs returned 200 for the production PNG, preview board, and STATUS after propagation at the same heartbeat.
- `npm run ios:sync:github-assets` completed and confirmed `No remote library asset originals found for dist.` and `No remote library asset originals found for ios.`
- `src/data.js` is connected to the remote path with `imageUrl`, `variantAssets`, and a rollback-capable `imageStub`.

## Rollback stub
- Remove the accepted file above from RollNote-assets if rejected.
- In `src/data.js`, remove `POLAROID_SPECTRA_REVIEW_PREVIEW_URL`, remove `cam-polaroid-spectra` from `CAMERA_VARIANT_ASSETS`, and remove the `imageUrl` / `imageStub` fields from `cam-polaroid-spectra`.
