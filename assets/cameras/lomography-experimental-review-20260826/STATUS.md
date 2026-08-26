# Status

## Batch

- Name: Lomography experimental cameras
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Completed models

- Lomography Fisheye No.2
- Lomography La Sardina DIY
- Lomography ActionSampler Clear
- Lomography SuperSampler

Full-library filename and data searches found no existing qualified asset for these variants before generation.

## Final assets

- `final/fisheye-no2-rollnote-v1.png`
- `final/la-sardina-rollnote-v1.png`
- `final/actionsampler-rollnote-v1.png`
- `final/supersampler-rollnote-v1.png`

All four are 1536x1024 RGBA PNGs with true alpha.

## Review boards

- `lomography-experimental-review-board-a-v1.png`
- `lomography-experimental-review-board-b-v1.png`

## Quality control

- Two real references retained for every model; sample photographs were rejected.
- Exact front view used for all four candidates.
- Fisheye No.2 lens, circular top viewfinder, built-in flash and switches match the real layout.
- La Sardina is camera-body-only; the detachable flash was omitted. Its first oversized-lens candidate was rejected and corrected.
- ActionSampler retains four equal lenses, transparent shell, internal mechanics and restrained identification colors; the wrist cord was omitted.
- SuperSampler retains the tall body, four-lens vertical column, molded ribs, viewfinder and rip-cord loop; edition graphics were omitted.
- Logos and wording are localized into unreadable geometric marks; no full-camera blur was applied.
- Edge-connected checkerboards were removed and RGBA alpha verified.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26.

## Next candidates

After a fresh full-library duplicate check: Spinner 360, Horizon Perfekt, Horizon Kompakt, and LomoKino.
