# Olympus Six / Chrome Six Asset Stub

Date: 2026-08-03

## Scope

Generated separate RollNote-style camera assets for the `cam-olympus-six-chrome-six` parent model:

- Olympus Six
- Olympus Six I
- Olympus Six II
- Super Olympus
- Chrome Six I
- Chrome Six II
- Chrome Six III f/3.5
- Chrome Six III f/2.8
- Chrome Six IVa
- Chrome Six IVb
- Chrome Six V A
- Chrome Six V B
- Chrome Six RII A
- Chrome Six RII B

## References

- Biofos Olympus folding cameras: https://www.biofos.com/coll/subcoll/folder.html
- Guy SmugMug Chrome Six III support page: https://guy.smugmug.com/Walkabout-Film/Walkabout-Camera-Collection/Olympus-Chrome-Six-III
- Wall Photography Chrome Six RIIB page: https://wallphotography.wordpress.com/2011/10/01/olympus-chrome-six-riib-product-of-1955/

Downloaded reference pages and images are kept under `references/`. The reference board is `olympus-six-reference-board.png`.

## Final Assets

Transparent PNGs are kept in `transparent/` and copied one level up for app/server publishing:

- `olympus-six-rollnote-v1.png`
- `olympus-six-i-rollnote-v1.png`
- `olympus-six-ii-rollnote-v1.png`
- `olympus-super-olympus-rollnote-v1.png`
- `olympus-chrome-six-i-rollnote-v1.png`
- `olympus-chrome-six-ii-rollnote-v1.png`
- `olympus-chrome-six-iii-f35-rollnote-v1.png`
- `olympus-chrome-six-iii-f28-rollnote-v1.png`
- `olympus-chrome-six-iva-rollnote-v1.png`
- `olympus-chrome-six-ivb-rollnote-v1.png`
- `olympus-chrome-six-v-a-rollnote-v1.png`
- `olympus-chrome-six-v-b-rollnote-v1.png`
- `olympus-chrome-six-rii-a-rollnote-v1.png`
- `olympus-chrome-six-rii-b-rollnote-v1.png`

Preview board: `olympus-six-preview-v1.png`.

## Rejected

- `rejected/olympus-chrome-six-iii-f35-green-finder-rejected.png`: rejected because the finder glass was generated as chroma green and would be incorrectly removed during background extraction.

## App Wiring

The app should load these assets remotely through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after `npm run ios:sync:github-assets`, `npm run android:sync:github-assets`, or `npm run android:assemble:github-assets`.

Rollback: remove `cam-olympus-six-chrome-six` from `CAMERA_VARIANT_ASSETS`, remove the `imageUrl`/`imageStub` fields from `cam-olympus-six-chrome-six`, and keep this folder as recovery context.
