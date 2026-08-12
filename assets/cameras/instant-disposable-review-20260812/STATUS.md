# RollNote Instant / Disposable Camera Assets - 2026-08-12

## Scope

First calibration batch:
- Kodak FunSaver
- Kodak Sport Waterproof
- Fujifilm QuickSnap Flash
- Fujifilm QuickSnap Waterproof / Active
- Fujifilm instax mini 12
- Fujifilm instax mini Evo

Next groups:
- Polaroid SX-70 folding
- Polaroid 600 box / OneStep
- Polaroid Now / Now+
- Fujifilm instax mini 40 / 41
- Additional disposable cameras after user review.

## Progress

- [x] Review folder created.
- [x] Thread heartbeat created: 30-minute progress/stuck checks, 4-hour staged summary cadence.
- [x] Official/reference images downloaded.
- [x] Reference board created.
- [x] RollNote-style chroma-key sources generated.
- [x] Transparent PNGs extracted and validated.
- [x] Preview board created for user review.
- [x] Assets uploaded to RollNote-assets.
- [x] App data connected through remote assets with imageStub rollback notes.

## Connected Assets

RollNote-assets commit: `d259ca5`

- `kodak-funsaver-rollnote-v1.png`
- `kodak-sport-rollnote-v1.png`
- `fujifilm-quicksnap-rollnote-v1.png`
- `fujifilm-quicksnap-active-rollnote-v1.png`
- `instax-mini12-rollnote-v2.png`
- `instax-minievo-rollnote-v1.png`

Preview board:
- Local: `instant-disposable-preview-v2.png`
- Remote: `https://phathadfeesh.github.io/RollNote-assets/assets/cameras/instant-disposable-review-20260812/instant-disposable-preview-v2.png`

## Validation

- Alpha validation passed for all connected PNGs: RGBA, transparent corners, no visible chroma-key residue.
- GitHub Pages returned HTTP 200 for all six production PNGs and the preview board on 2026-08-12 11:39 CST.
- `src/data.js` import check passed and confirmed the connected camera ids:
  `cam-kodak-single-use`, `cam-fujifilm-quicksnap`, `cam-instax-mini-11-12-13`, `cam-instax-mini-evo`.

## Recovery Notes

Keep generated sources under `generated/`, final transparent images under `final/`, and do not replace existing accepted assets unless explicitly requested.

To roll back the first calibration batch, remove the six production PNGs from RollNote-assets and local `public/assets/cameras/`, then remove `imageUrl` / `imageStub` from the four connected app entries and remove these ids from `CAMERA_VARIANT_ASSETS`: `cam-kodak-single-use`, `cam-fujifilm-quicksnap`, `cam-instax-mini-11-12-13`, `cam-instax-mini-evo`.
