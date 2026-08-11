# Bronica GS-1 RollNote Asset Stub

Date: 2026-08-11

## Scope

- Camera: Zenza Bronica GS-1
- App id: `cam-bronica-gs1`
- Final asset: `/assets/cameras/bronica-gs1-rollnote-v1.png`
- Review preview: `/assets/cameras/bronica-gs1-review-20260811/bronica-gs1-preview-v1.png`

## References

- Ross Jukes Photography: `https://www.rossjukesphoto.co.uk/photographyblog/bronica-gs-1-review`
- EMULSIVE camera review and GS-1 system map: `https://emulsive.org/reviews/camera-reviews/camera-review-bronica-gs1-ladric-stephenson`
- Wikipedia Bronica overview: `https://en.wikipedia.org/wiki/Bronica`
- RollNote accepted style target: `/Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/call_bmKt0WhEeK4uJOgn3LxOoyHb.png`

## Generated Files

- `generated/bronica-gs1-green-v1.png`: built-in image generation output on chroma-key green.
- `../bronica-gs1-rollnote-v1.png`: transparent PNG produced from the green source.
- `references/bronica-gs1-reference-board-v1.jpg`: reference board combining real GS-1 photos/system details and the accepted style target.
- `bronica-gs1-preview-v1.png`: review board showing final transparent output, green source, and references.

## Validation

- Transparent output is RGBA, 1536 x 1024.
- Corner alpha values: `[0, 0, 0, 0]`.
- Opaque green residual pixels: `0`.
- The image keeps GS-1-specific wide 6x7 proportions, waist-level finder, modular back seam, side winding controls, and a large central Zenzanon lens.

## Remote Loading

The final PNG and review folder are mirrored to `RollNote-assets` and served by GitHub Pages. The app should resolve `/assets/cameras/bronica-gs1-rollnote-v1.png` through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` when using `ios:sync:github-assets`, `android:sync:github-assets`, or `android:assemble:github-assets`.

## Rollback

Remove `imageUrl` and `imageStub` from `cam-bronica-gs1`, and remove the `cam-bronica-gs1` entry from `CAMERA_VARIANT_ASSETS`. The camera remains selectable without a connected generated asset.
