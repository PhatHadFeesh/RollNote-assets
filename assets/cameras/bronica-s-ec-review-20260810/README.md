# Bronica S / EC Series Image Stub

Generated on 2026-08-10 for RollNote camera-library variant switching.

## App variants

- Zenza Bronica D -> `bronica-d-rollnote-v1.png`
- Z -> `bronica-z-rollnote-v1.png`
- S -> `bronica-s-rollnote-v1.png`
- S2 -> `bronica-s2-rollnote-v1.png`
- S2A -> `bronica-s2a-rollnote-v1.png`
- C -> `bronica-c-rollnote-v1.png`
- EC -> `bronica-ec-rollnote-v1.png`
- EC-TL -> `bronica-ec-tl-rollnote-v1.png`
- EC-TL II -> `bronica-ec-tl-ii-rollnote-v1.png`

## Generation notes

- Built-in `image_gen` was used with the accepted RollNote rounded camera style reference:
  `/Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/call_bmKt0WhEeK4uJOgn3LxOoyHb.png`
- Each source was generated on flat `#00ff00`, then converted to transparent PNG with:
  `${CODEX_HOME:-$HOME/.codex}/skills/.system/imagegen/scripts/remove_chroma_key.py`
- Green source images are preserved in `generated/*-green-v1.png`.
- Final transparent PNGs live in `public/assets/cameras/` locally and should be uploaded to `RollNote-assets/assets/cameras/` before release/simulator sync.
- `source-corsopolaris-bronica.html` is an unrelated earlier mistaken download and was not used.

## Primary reference sources

- Cameraquest Bronica D / S / S2 / EC notes: https://www.cameraquest.com/bronicad.htm
- Craig Camera Bronica model identification: https://www.craigcamera.com/research_trivbronica.htm
- Dirapon Bronica collection references: https://dirapon.be/bronica.htm
- Vintage Camera Digest Bronica overview: https://vintagecameradigest.com/bronica/
- Shoot With Personality Bronica S reference: https://shootwithpersonality.com/2014/12/18/something-borrowed-zenza-bronica-s/
- Mike Eckman Bronica S2 reference: https://mikeeckman.com/2021/05/bronica-s2-1965/
- GotFilm Bronica S2/S2A reference: https://gotfilm.org/2021/04/11/zenza-bronica-s2-a-classic-6x6-camera/
- Stollee Bronica C reference: https://stollee.org/cameras/1965-zenza-bronica-c.html
- Chemical Cameras Bronica C reference: https://chemicalcameras.wordpress.com/bronica-c/
- GotFilm Bronica EC / EC-TL reference: https://gotfilm.org/2021/04/12/zenza-bronica-ec-an-electronic-version-of-the-s2/
- Stollee Bronica EC-II reference: https://stollee.org/cameras/1978-zenza-bronica-ec-ii.html
- Sunrise Camera EC-TL II image references: `downloads/bronica-ec-tl-ii-sunrise-front.jpg`, `downloads/bronica-ec-tl-ii-sunrise-body.jpg`

## Validation

Alpha validation passed for all nine PNGs:

- corner alpha values were `[0, 0, 0, 0]`
- `opaque_green=0`
- all outputs retained substantial non-transparent subject area

Preview boards:

- `references/bronica-s-ec-reference-board-v1.jpg`
- `bronica-s-ec-preview-v1.png`

## Rollback

To disconnect this batch from the app, remove `imageUrl`/`imageStub` from `cam-bronica-s-ec-series` in `src/data.js`, remove the `cam-bronica-s-ec-series` entry from `CAMERA_VARIANT_ASSETS`, and rerun `npm run ios:sync:github-assets` or the matching platform sync.
