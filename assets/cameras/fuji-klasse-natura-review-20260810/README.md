# Fujifilm Klasse / Natura RollNote Assets

Generated on 2026-08-10 for `cam-fuji-klasse-natura`.

## Variants

- Klasse: `fuji-klasse-rollnote-v1.png`
- Klasse W: `fuji-klasse-w-rollnote-v1.png`
- Klasse S: `fuji-klasse-s-rollnote-v1.png`
- Natura S: `fuji-natura-s-rollnote-v1.png`
- Natura Black F1.9: `fuji-natura-black-f19-rollnote-v1.png`
- Natura Classica: `fuji-natura-classica-rollnote-v1.png`
- Tiara / DL Super Mini: `fuji-tiara-dl-super-mini-rollnote-v1.png`

## Reference Sources

- Matt Loves Cameras, Fujifilm Klasse / Klasse S: `source-mattlovescameras-klasse.html`
- 35mmc, Fuji Natura S review: `source-35mmc-natura-s.html`
- Casual Photophile, Fujifilm Natura Black F1.9 review: `source-casualphotophile-natura-black.html`
- Lofi Photog, Fuji Natura Classica review: `source-lofiphotog-natura-classica.html`
- Analog Cafe, Fujifilm Cardia Tiara / DL Super Mini review: `source-analogcafe-tiara.html`
- Kosmo Foto, Fujifilm DL Super Mini review: `source-kosmofoto-dl-super-mini.html`
- 35mmc, Fuji DL Super Mini / Tiara review: `source-35mmc-tiara.html`

## Stored Stubs

- `references/`: source HTML and downloaded reference photos.
- `generated/`: green-screen originals copied from built-in image generation output.
- `fuji-klasse-natura-reference-board-v1.png`: visual reference contact sheet.
- `fuji-klasse-natura-preview-v1.png`: final transparent PNG preview sheet.

## Processing

Green-screen originals were cut out with:

```bash
python "${CODEX_HOME:-$HOME/.codex}/skills/.system/imagegen/scripts/remove_chroma_key.py" \
  --auto-key \
  --soft-matte \
  --transparent-threshold 12 \
  --opaque-threshold 220 \
  --despill
```

Validation on 2026-08-10: all seven final PNGs are RGBA, have transparent corners, and have `opaque_green=0`.

## Rollback

Remove the seven `fuji-*-rollnote-v1.png` files listed above, remove the `cam-fuji-klasse-natura` entry from `CAMERA_VARIANT_ASSETS`, and remove `imageUrl` / `imageStub` from `cam-fuji-klasse-natura` in `src/data.js`.
