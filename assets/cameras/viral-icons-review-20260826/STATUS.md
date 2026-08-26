# Viral Film Icons Review - 2026-08-26

Status: user-approved and uploaded in `RollNote-assets` commit `5a6e870`. The batch is not yet connected to the App.

## Candidates

| App parent | Camera | Selected candidate | Visual check |
| --- | --- | --- | --- |
| `cam-reto-pano` | RETO PANO 35mm | `final/reto-pano-rollnote-v1.png` | Wide smoky translucent shell, central 22mm lens, curved selector track, upper viewfinder/flash module and top shutter follow the official black-body references. |
| `cam-lomography-lca` | Lomography LC-A+ | `final/lomo-lca-plus-rollnote-v1.png` | Compact black body, raised central viewfinder/lens housing, twin pebbled panels, top controls and right-side lever follow the retailer references. |
| `cam-lomography-holga` | Holga 120N | `final/holga-120n-rollnote-v1.png` | Tall box body, large left advance knob, center-top finder block, upper-right viewfinder, square lens board, ribbed 60mm lens and metal side clips are retained. |
| `cam-lomography-diana` | Lomography Diana F+ | `final/diana-f-plus-rollnote-v1.png` | Turquoise upper shell, central finder, black textured lower body, large stepped lens and top controls match the reference; the detachable flash is intentionally omitted. |

## Review Boards

- `viral-icons-review-board-a-v1.png`: RETO PANO 35mm and Lomography LC-A+
- `viral-icons-review-board-b-v1.png`: Holga 120N and Lomography Diana F+

## QC

- All four candidates are 1536 x 1024 RGBA PNG files with real transparent pixels.
- All four use a straight-on front view and contain one isolated camera.
- Style target is the early RollNote hard-edge illustration language: crisp black contours, black/white/gray logic, restrained recognition color and moderate lens/body depth.
- Brand/model marks and lens lettering are replaced locally with unreadable geometric blocks. Camera geometry and controls remain sharp.
- Each model used two real references. References and source URLs are preserved in this directory.
- Diana F+ is represented as the camera body only; its detachable flash, strap and lens cap are excluded.
- No existing approved asset was regenerated. No App mapping or remote asset repository was changed.
- `npm run build` passed on 2026-08-26 (`vite v8.0.14`, 1877 modules transformed).

## Pending

Upload completed in `RollNote-assets` commit `5a6e870`. App integration remains pending; use the GitHub Pages asset base and preserve the prior `imageStub` and rollback values when connecting.

