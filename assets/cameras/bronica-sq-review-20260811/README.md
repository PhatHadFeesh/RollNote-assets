# Bronica SQ Series Image Stub

Generated on 2026-08-11 for RollNote camera-library variant switching.

## App variants

- SQ -> `bronica-sq-rollnote-v1.png`
- SQ-A -> `bronica-sq-a-rollnote-v1.png`
- SQ-Am -> `bronica-sq-am-rollnote-v1.png`
- SQ-Ai -> `bronica-sq-ai-rollnote-v1.png`
- SQ-B -> `bronica-sq-b-rollnote-v1.png`

## Generation notes

- Built-in `image_gen` was used with the accepted RollNote rounded camera style reference:
  `/Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/call_bmKt0WhEeK4uJOgn3LxOoyHb.png`
- Each source was generated on flat `#00ff00`, then converted to transparent PNG with:
  `${CODEX_HOME:-$HOME/.codex}/skills/.system/imagegen/scripts/remove_chroma_key.py`
- Green source images are preserved in `generated/*-green-v1.png`.
- Final transparent PNGs live in `public/assets/cameras/` locally and should be uploaded to `RollNote-assets/assets/cameras/` before release/simulator sync.
- SQ-Am is intentionally wider than the other variants to preserve its motorized winding/battery grip body.

## Primary reference sources

- Bronica overview and SQ/SQ-A/SQ-Ai image references: https://en.wikipedia.org/wiki/Bronica
- Gregory Owain Bronica SQ-A review: https://www.gregoryowain.co.uk/blog/bronica-sq-a-review
- Tightfisted Photography Bronica SQ-A reference: https://tightfistedphotography.wordpress.com/2013/12/11/zenza-bronica-sq-a-camera/
- Butkus Bronica SQ-Am manual reference: https://butkus.org/chinon/bronica/bronica_sq-a-m/bronica_sq-a-m-splash.htm
- EMULSIVE Bronica SQ-Ai reference: https://emulsive.org/reviews/camera-reviews/camera-review-bronica-sq-ai-by-adrian-vila
- Luis Samaniego Bronica SQ-B reference: https://www.luis-samaniego.eu/zenza-bronica-sqb/
- Randomphoto Bronica SQ-B reference: https://randomphoto.blogspot.com/2017/11/the-bronica-sq-b-perfect-square.html

## Validation

Alpha validation passed for all five PNGs:

- corner alpha values were `[0, 0, 0, 0]`
- `opaque_green=0`
- all outputs retained substantial non-transparent subject area

Preview boards:

- `references/bronica-sq-reference-board-v1.jpg`
- `bronica-sq-preview-v1.png`

## Rollback

To disconnect this batch from the app, remove `imageUrl` and `imageStub` from `cam-bronica-sq-series`, remove the `cam-bronica-sq-series` entry from `CAMERA_VARIANT_ASSETS`, and rerun `npm run ios:sync:github-assets` or the matching platform sync.
