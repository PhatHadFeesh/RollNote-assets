# Olympus Flex TLR Asset Stub

Date: 2026-08-06

## Scope

Generated separate RollNote-style camera assets for the `cam-olympus-flex-tlr` parent model:

- Flex I
- Flex BI
- Flex BII
- Flex A3.5
- Flex A2.8
- Flex A3.5 II

## References

- Biofos Olympus twin-lens reflex lineage: https://www.biofos.com/coll/subcoll/tlr.html
- TLR Cameras Olympus Flex page: https://www.tlr-cameras.com/japanese/Olympus.html

Downloaded reference pages and images are kept under `references/`. The reference board is `olympus-flex-tlr-reference-board.png`.

## Final Assets

Transparent PNGs are kept in `transparent/` and copied one level up for app/server publishing:

- `olympus-flex-i-rollnote-v1.png`
- `olympus-flex-bi-rollnote-v1.png`
- `olympus-flex-bii-rollnote-v1.png`
- `olympus-flex-a35-rollnote-v1.png`
- `olympus-flex-a28-rollnote-v1.png`
- `olympus-flex-a35-ii-rollnote-v1.png`

Preview board: `olympus-flex-tlr-preview-v1.png`.

All final transparent PNGs were normalized to a 1024x1536 transparent canvas to keep app thumbnails stable.

## Rejected And Superseded

- `rejected/olympus-flex-bi-side-angle-rejected.png`: rejected because the first BI output was too side-facing for the current RollNote front-view standard.
- `superseded/olympus-flex-a35-side-angle-superseded.png`: replaced by a straighter front-view A3.5 output for better group consistency.

## App Wiring

The app should load these assets remotely through `VITE_ROLLNOTE_LIBRARY_ASSET_BASE_URL` after `npm run ios:sync:github-assets`, `npm run android:sync:github-assets`, or `npm run android:assemble:github-assets`.

Rollback: remove `cam-olympus-flex-tlr` from `CAMERA_VARIANT_ASSETS`, remove the `imageUrl`/`imageStub` fields from `cam-olympus-flex-tlr`, and keep this folder as recovery context.
