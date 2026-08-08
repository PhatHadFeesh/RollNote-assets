Fujifilm TX panoramic review stub
=================================

Connected group: `cam-fuji-tx-series`
Date: 2026-08-08

Final transparent assets:
- `/assets/cameras/fuji-tx1-rollnote-v1.png`
- `/assets/cameras/fuji-tx2-rollnote-v1.png`

Variant mapping:
- `TX-1` -> `fuji-tx1-rollnote-v1.png`
- `TX-2` -> `fuji-tx2-rollnote-v1.png`

Reference sources retained in `references/`:
- Jonas Rask Fujifilm TX-1 article HTML and TX-1 body detail photos.
- Japan Camera Hunter TX-1 article HTML and front body photos.
- Japan Camera Hunter Fujifilm TX-2 product page HTML and TX-2 body photos.
- Japan Camera Hunter Hasselblad XPan II article HTML and same-body-generation reference photos.

Generation notes:
- Used the accepted RollNote OM 2000 green-screen image as style reference.
- Generated on flat `#00ff00`, then removed the key locally with the imagegen chroma-key helper.
- TX-1 is treated as the warm titanium first-generation body with the large round front dial.
- TX-2 is treated as the black second-generation body without the first-generation front dial.

Validation:
- Transparent PNG corners: all alpha 0.
- Residual opaque green pixels: 0 for both final assets.
- Review preview: `fuji-tx-preview-v1.png`.

Rollback:
- Remove the two final transparent assets from the app and RollNote-assets.
- Remove `FUJI_TX_REVIEW_PREVIEW_URL`, `CAMERA_VARIANT_ASSETS["cam-fuji-tx-series"]`, and the `imageUrl` / `imageStub` fields from `cam-fuji-tx-series` in `src/data.js`.
