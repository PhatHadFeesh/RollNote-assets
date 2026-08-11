# Bronica RF645 RollNote Asset Stub

Date: 2026-08-11

## Scope

- Camera: Bronica RF645
- App id: `cam-bronica-rf645`
- Final asset: `/assets/cameras/bronica-rf645-rollnote-v1.png`
- Review preview: `/assets/cameras/bronica-rf645-review-20260811/bronica-rf645-preview-v1.png`

## References

- Japan Camera Hunter RF645 review: `https://www.japancamerahunter.com/2017/06/camera-geekery-bronica-rf645-review/`
- Luminous Landscape RF645 page: `https://luminous-landscape.com/bronica-rf645/`
- Tamron RF645 archive page: `https://www.tamron.com/jp/consumer/lenses/data/bronica/rf645.html`
- Wikipedia Bronica overview: `https://en.wikipedia.org/wiki/Bronica`
- RollNote accepted style target: `/Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/call_bmKt0WhEeK4uJOgn3LxOoyHb.png`

## Generated Files

- `generated/bronica-rf645-green-v1.png`: built-in image generation output on chroma-key green.
- `../bronica-rf645-rollnote-v1.png`: transparent PNG produced from the green source.
- `references/bronica-rf645-reference-board-v1.jpg`: reference board combining real RF645 photos, official Tamron visual, and the accepted style target.
- `bronica-rf645-preview-v1.png`: review board showing final transparent output, green source, and references.

## Validation

- Transparent output is RGBA, 1536 x 1024.
- Corner alpha values: `[0, 0, 0, 0]`.
- Opaque green residual pixels: `0`.
- The image keeps RF645-specific modern medium-format rangefinder proportions, prominent hand grip, upper viewfinder/rangefinder window cluster, RF645 front mark area, and the 65mm Zenzanon-RF lens.

## Remote Loading

The final PNG and review folder are mirrored to `RollNote-assets` and served by GitHub Pages. The app should resolve `/assets/cameras/bronica-rf645-rollnote-v1.png` through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` when using `ios:sync:github-assets`, `android:sync:github-assets`, or `android:assemble:github-assets`.

## Rollback

Remove `imageUrl` and `imageStub` from `cam-bronica-rf645`, and remove the `cam-bronica-rf645` entry from `CAMERA_VARIANT_ASSETS`. The camera remains selectable without a connected generated asset.
