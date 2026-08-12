# RollNote disposable next review - 2026-08-12

## Scope
- Kodak Power Flash 800 single-use camera
- AgfaPhoto LeBox Flash 400 single-use camera
- Ilford HP5 Plus single-use camera
- Ilford XP2 Super single-use camera
- Lomography Simple Use Color Negative 400 camera
- Lomography Simple Use LomoChrome Purple camera

## Accepted assets
- `kodak-power-flash-rollnote-v1.png`: reused from accepted film-raster artwork.
- `agfaphoto-lebox-flash-rollnote-v1.png`: reused from accepted film-raster artwork.
- `ilford-hp5-single-use-rollnote-v1.png`: newly generated against official Harman product reference.
- `ilford-xp2-single-use-rollnote-v1.png`: newly generated against official Harman product reference.
- `lomography-simple-use-color-rollnote-v1.png`: newly generated against public product reference.
- `lomography-simple-use-purple-rollnote-v1.png`: newly generated against public product reference.

## Quality check
- Preview board: `disposable-next-preview-v1.png`
- Alpha validation: `validation-alpha-v1.json`
- Generated finals are RGBA PNGs with transparent corners and no opaque chroma key pixels.
- Visual check: all accepted assets keep a mostly front-facing compact disposable-camera silhouette. Ilford and Lomography assets follow the current rounded RollNote cartoon style closely.
- Caveat: Kodak Power Flash and AgfaPhoto LeBox are reused accepted transition assets with more readable product-label detail than the newer no-text camera-library style. They are connected so users can choose the models now, and can be regenerated later if the library needs stricter style consistency.

## Remote loading
- Target remote base: `https://phathadfeesh.github.io/RollNote-assets`
- App paths remain `/assets/cameras/<file>.png` and are resolved through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL`.
- Do not bundle these original camera PNGs in app builds; run the GitHub-assets sync scripts after data changes.

## Rollback stub
- Remove the six files above from RollNote-assets if rejected.
- In `src/data.js`, remove `DISPOSABLE_NEXT_REVIEW_PREVIEW_URL`, remove the new/extended `CAMERA_VARIANT_ASSETS` mappings, and remove or revert the `imageUrl`/`imageStub` fields for:
  - `cam-kodak-single-use`
  - `cam-agfaphoto-lebox`
  - `cam-ilford-single-use`
  - `cam-lomography-simple-use`
