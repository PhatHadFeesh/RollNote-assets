# RollNote Polaroid Instant Camera Assets - 2026-08-12

## Scope

Connected in this batch:
- Polaroid OneStep / 1000 white rainbow representative
- Polaroid SX-70 Original folding
- Polaroid SX-70 Sonar OneStep
- Polaroid Sun 660 AF / 600 AF representative
- Polaroid Now+ modern i-Type representative

Deferred:
- SX-70 Model 3, The Button, Pronto, ordinary 600 box cameras, OneStep CloseUp, SLR 680 / 690, Spectra, Impulse, Go, I-2, Flip, and other special editions still need their own reviewed artwork.

## Progress

- [x] Reference folder created.
- [x] Reference images downloaded and review board created.
- [x] RollNote-style chroma-key sources generated.
- [x] Transparent PNGs extracted and validated.
- [x] Preview board created for user review.
- [x] Assets uploaded to RollNote-assets.
- [x] App data connected through remote assets with imageStub rollback notes.

## Connected Assets

RollNote-assets commit: `27f3ba7`

- `polaroid-onestep-white-rainbow-rollnote-v1.png`
- `polaroid-sx70-original-rollnote-v1.png`
- `polaroid-sx70-sonar-rollnote-v1.png`
- `polaroid-sun660-af-rollnote-v2.png`
- `polaroid-now-plus-rollnote-v1.png`

Preview board:
- Local: `polaroid-preview-v2.png`
- Remote: `https://phathadfeesh.github.io/RollNote-assets/assets/cameras/polaroid-instant-review-20260812/polaroid-preview-v2.png`

## Validation

- Alpha validation passed for all connected PNGs: RGBA, transparent corners, no visible chroma-key residue.
- Sun 660 AF v1 was kept as a rejected candidate because it had too much readable product text; v2 is the connected no-readable-text asset.

## Recovery Notes

Keep generated sources under `generated/`, final transparent images under `final/`, and do not replace existing accepted assets unless explicitly requested.

To roll back this batch, remove the five production PNGs from RollNote-assets and local `public/assets/cameras/`, then remove `imageUrl` / `imageStub` from the four connected app entries and remove these ids from `CAMERA_VARIANT_ASSETS`: `cam-polaroid-sx70`, `cam-polaroid-sx70-box`, `cam-polaroid-600-af-closeup`, `cam-polaroid-modern-itype`.
