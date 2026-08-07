# Fujifilm GA645 Review Stub

Date: 2026-08-07

This folder preserves the recoverable review trail for the RollNote-style Fujifilm GA645 group before the generated camera originals are connected through the remote asset repository.

## Connected Variants

- GA645 -> `fuji-ga645-rollnote-v1.png`
- GA645W -> `fuji-ga645w-rollnote-v1.png`
- GA645i -> `fuji-ga645i-rollnote-v1.png`
- GA645Wi -> `fuji-ga645wi-rollnote-v1.png`
- GA645Zi -> `fuji-ga645zi-rollnote-v1.png`

## Source References

- GA645: Shoot It With Film review page, `source-shootitwithfilm-ga645.html`, with local image `shootitwithfilm-ga645-featured.jpg`; MrLeica review page, `source-mrleica-ga645.html`, with local image `mrleica-ga645-pro-lineup.jpg`.
- GA645W: Bonnescape review page, `source-bonnescape-ga645w.html`, with local images `bonnescape-ga645w-front.jpg` and `bonnescape-ga645w-top.jpg`; Superb Japan listing page, `source-superb-ga645w.html`, with local image `superb-ga645w-0001.jpg`.
- GA645i: EMULSIVE review page, `source-emulsive-ga645i.html`, with local images `emulsive-ga645i-front.jpg` and `emulsive-ga645i-top.jpg`.
- GA645Wi: Mike Eckman review page, `source-mikeeckman-ga645wi.html`, with local images `mikeeckman-ga645wi-front.jpg` and `mikeeckman-ga645wi-detail.jpg`.
- GA645Zi: EMULSIVE review page, `source-emulsive-ga645zi.html`, with local images `emulsive-ga645zi-cover.jpg` and `emulsive-ga645zi-flash.jpg`.

The reference board is `fuji-ga645-reference-board.png`.

## Generated Sources

Green-screen originals are kept in `generated/`:

- `generated/fuji-ga645-rollnote-v1-green.png`
- `generated/fuji-ga645w-rollnote-v1-green.png`
- `generated/fuji-ga645i-rollnote-v1-green.png`
- `generated/fuji-ga645wi-rollnote-v1-green.png`
- `generated/fuji-ga645zi-rollnote-v1-green.png`

Final transparent PNGs are stored one level up in `public/assets/cameras/` and mirrored to RollNote-assets before app connection. Chroma-key validation passed with transparent corners and `opaque_green=0` for all final PNGs. The group preview is `fuji-ga645-preview-v1.png`.

## Notes

GA645W and GA645Wi are intentionally separate because their front/body details differ enough for RollNote variant switching. GA645Zi is treated as a separate visual body because the zoom camera shape and silver/black finish are distinct from the fixed-lens GA645 family.

## Rollback

Remove this review folder and these five final PNGs from RollNote-assets, then remove the `cam-fuji-ga645` entry from `CAMERA_VARIANT_ASSETS` and clear `imageUrl` / `imageStub` from the corresponding `src/data.js` camera entry.
