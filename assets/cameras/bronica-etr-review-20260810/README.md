# Bronica ETR Series Image Stub

Generated on 2026-08-11 for RollNote camera-library variant switching.

## App variants

- ETR -> `bronica-etr-rollnote-v1.png`
- ETR-C -> `bronica-etr-c-rollnote-v1.png`
- ETRS -> `bronica-etrs-rollnote-v1.png`
- ETRSi -> `bronica-etrsi-rollnote-v1.png`

## Generation notes

- Built-in `image_gen` was used with the accepted RollNote rounded camera style reference:
  `/Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/call_bmKt0WhEeK4uJOgn3LxOoyHb.png`
- Each source was generated on flat `#00ff00`, then converted to transparent PNG with:
  `${CODEX_HOME:-$HOME/.codex}/skills/.system/imagegen/scripts/remove_chroma_key.py`
- Green source images are preserved in `generated/*-green-v1.png`.
- Final transparent PNGs live in `public/assets/cameras/` locally and should be uploaded to `RollNote-assets/assets/cameras/` before release/simulator sync.
- The older `bronica-etrsi-ai-cutout.png` asset is intentionally kept as a rollback source.

## Primary reference sources

- EMULSIVE Bronica ETR reference: https://emulsive.org/reviews/camera-reviews/the-bronica-etr-40-years-old-but-not-an-old-dog
- Camera Go Camera Bronica ETR-C reference: https://cameragocamera.com/2016/04/25/bronica-etr-c/
- K2 Photography Bronica ETRS reference: https://www.k2-photography.dk/bronica-etrs-a-good-alternative-to-hasselblad-500cm/
- EMULSIVE Bronica ETRSi reference: https://emulsive.org/reviews/camera-reviews/camera-review-zenza-bronica-etrsi-by-denys-trofimchuk
- Bronica overview: https://en.wikipedia.org/wiki/Bronica

## Validation

Alpha validation passed for all four PNGs:

- corner alpha values were `[0, 0, 0, 0]`
- `opaque_green=0`
- all outputs retained substantial non-transparent subject area

Preview boards:

- `references/bronica-etr-reference-board-v1.jpg`
- `bronica-etr-preview-v1.png`

## Rollback

To disconnect this batch from the app, set `cam-bronica-etrsi` back to `imageUrl: "/assets/cameras/bronica-etrsi-ai-cutout.png"`, remove its `imageStub`, remove the `cam-bronica-etrsi` entry from `CAMERA_VARIANT_ASSETS`, and rerun `npm run ios:sync:github-assets` or the matching platform sync.
