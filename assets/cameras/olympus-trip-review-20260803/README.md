# Olympus Trip Series Review Assets

Generated on 2026-08-03 for RollNote.

This folder keeps recoverable review material for the Olympus Trip series camera assets:

- `references/`: real-camera references and source URL notes.
- `generated/`: chroma-key source generations.
- `transparent/`: local alpha cutout drafts.
- `trip-preview-v1.png`: review contact sheet for the generated cutouts.
- `rejected/`: rejected generations kept for traceability.

Final app/remote assets are copied to `/assets/cameras/olympus-trip-*-rollnote-v1.png`.

Reference sources used:

- Olympus Museum official images: Trip 35, Trip Junior, Trip AF, Trip AF31, Trip AF50, Trip AF Mini, Trip MD2, Trip XB3.
- FOQUS product photo: Trip 500.
- ManualsLib product photo: Trip 600.
- LensFayre product photos: Trip AF 30 and Trip MD.
- eBay product photo: Trip XB40 AF.
- The Analog Club product photo: Trip XB400.

Note: the existing app variant named `Trip XB` does not appear to have a clear standalone model page in the checked sources. It is preserved as a selectable library variant and uses a separate XB-family representative illustration based on Trip XB3 visual references. It can be renamed or removed later without touching the generated files.

Rollback:

1. Remove `imageUrl` and `imageStub` from `cam-olympus-trip-series` in `src/data.js`.
2. Remove `cam-olympus-trip-series` from `CAMERA_VARIANT_ASSETS`.
3. Remove `OLYMPUS_TRIP_REVIEW_PREVIEW_URL` if unused.
4. The generated source, reference, and transparent files in this folder can be reused to restore or regenerate any variant.
