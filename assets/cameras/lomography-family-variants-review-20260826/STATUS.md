# Status

## Batch

- Name: Lomography family variants
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Completed models

- Lomography LC-Wide
- Lomography Diana Mini
- Holga 135BC
- Lomography Sprocket Rocket

LC-A 120 was intentionally removed after source review found mixed 35mm LC-A+ and sample-photo references. Sprocket Rocket replaced it after a clean full-library duplicate check.

## Final assets

- `final/lomo-lc-wide-rollnote-v1.png`
- `final/diana-mini-rollnote-v1.png`
- `final/holga-135bc-rollnote-v1.png`
- `final/sprocket-rocket-rollnote-v1.png`

All four final files are 1536x1024 RGBA PNGs with true alpha.

## Review boards

- `lomography-family-variants-review-board-a-v1.png`
- `lomography-family-variants-review-board-b-v1.png`

## Quality control

- Two real references retained for every model.
- Front view used for every candidate.
- Camera silhouette, lens, viewfinder, controls, and panel layout checked against references.
- Early RollNote hard-outline, monochrome-forward style retained; Diana Mini keeps cyan and LC-Wide keeps muted red identification accents.
- Logos and model wording are localized into unreadable geometric marks; no whole-camera blur was applied.
- Edge-connected generated checkerboards were removed, assets normalized to transparent 1536x1024, and alpha verified.
- Diana Mini v1 was rejected for excess width and an invented front window; corrected v2 became final.
- Sprocket Rocket v1 was rejected for an oversized lens; corrected v2 became final.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26.

## Next candidates

After another full-library duplicate check: Lomography Fisheye No.2, La Sardina, ActionSampler, and SuperSampler.
