Fujifilm GF670 / Voigtlander Bessa III review stub
==================================================

Connected group: `cam-fuji-gf670`
Date: 2026-08-08

Final transparent assets:
- `/assets/cameras/fuji-gf670-rollnote-v1.png`
- `/assets/cameras/fuji-gf670w-rollnote-v1.png`
- `/assets/cameras/voigtlander-bessa-iii-rollnote-v1.png`

Variant mapping:
- `GF670 Professional` -> `fuji-gf670-rollnote-v1.png`
- `GF670W Professional` -> `fuji-gf670w-rollnote-v1.png`
- `Voigtlander Bessa III` -> `voigtlander-bessa-iii-rollnote-v1.png`

Reference sources retained in `references/`:
- Mike Eckman Fujifilm GF670 review HTML and downloaded local reference photos.
- MrLeica GF670 source HTML.
- CameraQuest Bessa III source HTML, retained even though the fetched page was not visually useful due to the challenge page.
- Genotype GF670W source HTML.

Generation notes:
- Used the accepted RollNote OM 2000 green-screen image as style reference.
- Generated on flat `#00ff00`, then removed the key locally with the imagegen chroma-key helper.
- GF670 Professional and Bessa III intentionally keep a slight front three-quarter read so the folding bellows and front standard remain recognizable.
- GF670W Professional is intentionally non-folding and uses a fixed wide-angle lens body.

Validation:
- Transparent PNG corners: all alpha 0.
- Residual opaque green pixels: 0 for all three final assets.
- Review preview: `fuji-gf670-preview-v1.png`.

Rollback:
- Remove the three final transparent assets from the app and RollNote-assets.
- Remove `FUJI_GF670_REVIEW_PREVIEW_URL`, `CAMERA_VARIANT_ASSETS["cam-fuji-gf670"]`, and the `imageUrl` / `imageStub` fields from `cam-fuji-gf670` in `src/data.js`.
