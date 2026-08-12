# RollNote disposable gap review - 2026-08-12

## Scope
- AgfaPhoto LeBox Ocean 400
- AgfaPhoto LeBox Black&White APX400
- Ilford Ilfocolor Rapid Retro 400
- Lomography Simple Use LomoChrome Metropolis
- Lomography Simple Use Black & White 400

## Accepted assets
- `agfaphoto-lebox-ocean-rollnote-v1.png`
- `agfaphoto-lebox-bw-rollnote-v1.png`
- `ilford-ilfocolor-rapid-retro-rollnote-v1.png`
- `lomography-simple-use-metropolis-rollnote-v1.png`
- `lomography-simple-use-bw-rollnote-v1.png`

## Reference basis
- All five assets were generated from the saved real product references under the existing film-raster review folders.
- The accepted RollNote OM 2000 illustration was used as the style reference for rounded linework, tactile plastic highlights, and collectible app-card polish.
- The two rejected Ocean drafts are retained under `rejected/`: one leaned too much into bulky waterproof-housing hardware; one kept too much photographic label detail. The accepted Ocean v1 uses a simpler illustrated ocean sticker so it sits better in the camera library UI.

## Quality check
- Preview board: `disposable-gap-preview-v1.png`
- Preview board row order: AgfaPhoto LeBox Ocean 400, AgfaPhoto LeBox Black&White APX400, Ilford Ilfocolor Rapid Retro 400, Lomography Simple Use LomoChrome Metropolis, Lomography Simple Use Black & White 400.
- Alpha validation: `validation-alpha-v1.json`
- All five finals are RGBA PNGs with transparent corners and no opaque chroma-key pixels.
- Visual check: all accepted assets use a mostly straight/front-facing viewpoint, keep the real single-use camera proportions and control layout, and avoid readable logos/text in favor of abstract label blocks.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.

## Rollback stub
- Remove the five accepted files above from RollNote-assets if rejected.
- In `src/data.js`, remove `DISPOSABLE_GAP_REVIEW_PREVIEW_URL`, remove the newly expanded mappings for `cam-agfaphoto-lebox`, `cam-ilford-single-use`, and `cam-lomography-simple-use`, and revert their `imageStub.remoteAssetCommit` / `reviewPreviewUrls` to the previous disposable-next state if needed.
