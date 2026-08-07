# Olympus Ace Review Stub

Date: 2026-08-07

This folder preserves the recoverable review trail for the RollNote-style Olympus Ace group before the generated camera originals are connected through the remote asset repository.

## Connected Variants

- Ace -> `olympus-ace-rollnote-v1.png`
- Ace-E -> `olympus-ace-e-rollnote-v1.png`

## Source References

- Ace: Mike Eckman Olympus Ace reference page, `source-mikeeckman-olympus-ace.html`, with local reference images such as `mikeeckman-olympus-ace-1.jpg` and `mikeeckman-olympus-ace-7.jpg`.
- Ace-E: Olympus Ace-E instruction manual PDF, `source-olympus-ace-e-manual.pdf`, with the front-layout crop saved as `olympus-ace-e-manual-front-crop.png`.
- Ace-E supplemental camera character reference: Flickr image, `flickr-olympus-ace-e-front.jpg`.

The reference board is `olympus-ace-reference-board.png`.

## Generated Sources

Green-screen originals are kept in `generated/`:

- `generated/olympus-ace-rollnote-v1-green.png`
- `generated/olympus-ace-e-rollnote-v1-green.png`

Final transparent PNGs are stored one level up in `public/assets/cameras/` and mirrored to RollNote-assets before app connection. Chroma-key validation passed with transparent corners and `opaque_green=0` for both final PNGs.

## Notes

The Ace asset is matched to the plain, non-metered Olympus Ace body. The Ace-E asset is separately matched to the manual's front illustration and keeps the viewer-left honeycomb selenium meter window that distinguishes it from the plain Ace. The Ace-E Flickr image is angled, so the generated asset intentionally follows the manual crop for front-facing UI consistency.

## Rollback

Remove this review folder and these two final PNGs from RollNote-assets, then remove the `cam-olympus-ace` entry from `CAMERA_VARIANT_ASSETS` and clear `imageUrl` / `imageStub` from the corresponding `src/data.js` camera entry.
