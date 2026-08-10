# Fujica ST / AX RollNote Assets

Date: 2026-08-10

Group id: `cam-fujica-st-ax-series`

Generated variants:
- ST701 -> `fujica-st701-rollnote-v1.png`
- ST801 -> `fujica-st801-rollnote-v1.png`
- ST901 -> `fujica-st901-rollnote-v1.png`
- ST605 -> `fujica-st605-rollnote-v1.png`
- ST705 -> `fujica-st705-rollnote-v1.png`
- STX-1 -> `fujica-stx1-rollnote-v1.png`
- AX-1 -> `fujica-ax1-rollnote-v1.png`
- AX-3 -> `fujica-ax3-rollnote-v1.png`
- AX-5 -> `fujica-ax5-rollnote-v1.png`

Reference material is kept in `references/`, including downloaded source HTML and local reference images. The accepted RollNote style reference is copied as `references/downloads/style-reference-rollnote.png`.

Generation source files:
- Green-screen originals are in `generated/`.
- A rejected oblique AX-5 draft is preserved in `generated/rejected/`.
- `fujica-st-ax-reference-board-v1.png` shows the visual references.
- `fujica-st-ax-preview-v1.png` shows the accepted transparent assets together.

Transparency workflow:

```sh
python "${CODEX_HOME:-$HOME/.codex}/skills/.system/imagegen/scripts/remove_chroma_key.py" \
  --input generated/<file>-green.png \
  --out ../<file>.png \
  --auto-key border \
  --soft-matte \
  --transparent-threshold 12 \
  --opaque-threshold 220 \
  --despill
```

Validation result before upload:
- All accepted PNGs are RGBA.
- All four canvas corners have alpha 0.
- Bright opaque chroma-green leftovers: 0 for each accepted PNG.

Rollback:
- Remove the nine `fujica-*-rollnote-v1.png` assets from `public/assets/cameras`.
- Remove `FUJICA_ST_AX_REVIEW_PREVIEW_URL` and `cam-fujica-st-ax-series` from `CAMERA_VARIANT_ASSETS`.
- Remove `imageUrl` and `imageStub` from the `cam-fujica-st-ax-series` camera entry.
