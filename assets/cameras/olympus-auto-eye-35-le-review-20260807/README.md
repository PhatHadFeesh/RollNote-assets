# Olympus Auto Eye / 35 LE Review Stub

Date: 2026-08-07

This folder preserves the recoverable review trail for the RollNote-style Olympus Auto Eye / 35 LE group before the generated camera originals are connected through the remote asset repository.

## Connected Variants

- Auto -> `olympus-auto-rollnote-v1.png`
- Auto Eye -> `olympus-auto-eye-rollnote-v1.png`
- 35 LE -> `olympus-35-le-rollnote-v1.png`
- 35 LC -> `olympus-35-lc-rollnote-v1.png`
- 35 ED -> `olympus-35-ed-rollnote-v1.png`

## Source References

- Auto / Electro Set: Flickr reference, `references/flickr-auto-electro-set.jpg`, source page archived as `references/source-flickr-auto.html`.
- Auto Eye: Shutterlogue reference, `references/shutterlogue-auto-eye-front.jpg`, source page archived as `references/source-shutterlogue-auto-eye.html`.
- 35 LE: 35mmc reference, `references/35mmc-35-le-front.jpg`, source page archived as `references/source-35mmc-35-le.html`.
- 35 LC: Mike Eckman reference, `references/mikeeckman-35-lc-front.jpg`, source page archived as `references/source-mikeeckman-35-lc.html`; Camera Go Camera source page is also archived.
- 35 ED: msogavt WordPress reference, `references/wordpress-35-ed-front.jpg`, source page archived as `references/source-wordpress-35-ed.html`.

The reference board is `olympus-auto-eye-35-le-reference-board.png`.

## Generated Sources

Green-screen originals are kept in `generated/`:

- `generated/olympus-auto-rollnote-v1-green.png`
- `generated/olympus-auto-eye-rollnote-v1-green.png`
- `generated/olympus-35-le-rollnote-v1-green.png`
- `generated/olympus-35-lc-rollnote-v1-green.png`
- `generated/olympus-35-ed-rollnote-v1-green.png`

Final transparent PNGs are stored one level up in `public/assets/cameras/` and mirrored to RollNote-assets before app connection. Chroma-key validation passed with transparent corners and `opaque_green=0` for all five final PNGs.

## Notes

The Auto variant is treated as the early Olympus Auto / Auto Electro Set body based on the local Flickr reference set. The Auto Eye, 35 LE, 35 LC, and 35 ED use direct visual references from the local review set. No rejected or superseded generated images are currently retained for this group.

## Rollback

Remove this review folder and these five final PNGs from RollNote-assets, then remove the `cam-olympus-auto-eye-35-le` entry from `CAMERA_VARIANT_ASSETS` and clear `imageUrl` / `imageStub` from the corresponding `src/data.js` camera entry.
