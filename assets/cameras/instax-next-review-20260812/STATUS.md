# RollNote instax Next Camera Assets - 2026-08-12

## Scope

Connected in this batch:
- Fujifilm instax mini 40
- Fujifilm instax mini 41
- Fujifilm instax mini 90 Neo Classic
- Fujifilm instax mini 99

Already connected and not regenerated:
- Fujifilm instax mini 12
- Fujifilm instax mini Evo

Deferred:
- instax mini early / 7 / 8 / 9 / 11 / 13, mini LiPlay, WIDE, SQUARE, Pal, and printer families still need their own reviewed artwork.

## Progress

- [x] Review folder created.
- [x] Official/reference images downloaded where available.
- [x] Reference board created.
- [x] RollNote-style chroma-key sources generated.
- [x] Transparent PNGs extracted and validated.
- [x] Preview board created for user review.
- [x] Assets uploaded to RollNote-assets.
- [x] App data connected through remote assets with imageStub rollback notes.

## Connected Assets

RollNote-assets commit: `862fb28`

- `instax-mini40-rollnote-v1.png`
- `instax-mini41-rollnote-v1.png`
- `instax-mini90-rollnote-v1.png`
- `instax-mini99-rollnote-v1.png`

Preview board:
- Local: `instax-next-preview-v2.png`
- Remote: `https://phathadfeesh.github.io/RollNote-assets/assets/cameras/instax-next-review-20260812/instax-next-preview-v2.png`

## Validation

- Alpha validation passed for all connected PNGs: RGBA, transparent corners, no visible chroma-key residue.
- mini 41 and mini 99 were checked against official instax product imagery.
- mini 40 used official instax imagery, but the available product reference is more limited.
- mini 90 was checked against a clear external front product reference plus official instax navigation imagery.

## Recovery Notes

Keep generated sources under `generated/`, final transparent images under `final/`, and do not replace existing accepted assets unless explicitly requested.

To roll back this batch, remove the four production PNGs from RollNote-assets and local `public/assets/cameras/`, then remove `imageUrl` / `imageStub` from these app entries and remove these ids from `CAMERA_VARIANT_ASSETS`: `cam-instax-mini-40-41`, `cam-instax-mini-90`, `cam-instax-mini-99`.
