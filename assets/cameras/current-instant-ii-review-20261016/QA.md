# Artwork QA - 2026-10-16

All three accepted originals: 1536x1024, PNG RGBA, 8-bit, original generated alpha preserved without postprocessed background removal. Board images: 2200x1600. Visual inspection completed against both exact-model references on each board.

| Model | Alpha range | Fully transparent pixels | Corners | Result |
| --- | --- | --- | --- | --- |
| instax SQUARE 2 | 0..254 | 39.78% | 0,0,0,0 | pass |
| instax mini Evo Cinema | 0..254 | 80.67% | 1,0,0,0 | pass with negligible alpha residue note |
| Polaroid OneStep+ | 0..254 | 39.79% | 0,0,0,0 | pass |

- No image has edge pixels with alpha greater than 16/255. The Evo corner alpha 1/255 is a negligible generator residue; broad surrounding areas are alpha 0. No visible halo on checkerboard comparison boards. No baked background or checkerboard in originals.
- SQUARE 2: square pale body, upper-left finder, flash, shutter/grip, two lens sensors, circular selfie mirror and lower-right filter lever retained. Hard contours and moderate lens depth.
- Evo Cinema: vertical narrow front, upper sensor/mirror/flash cluster, lens, grip and right-edge controls retained. V1's non-reference red lens ticks were rejected; v2 changes them to gray. Accepted as first approved final v1. Its front-only silhouette is deliberately narrow, not a horizontal ordinary mini Evo.
- OneStep+: black front, function-plus button, red shutter, flash, viewfinder, exposure slider, lens, film latch and exit retained. Neutral gray strips replace rainbow branding. It is no longer represented by a OneStep 2 illustration.
- Grayscale with minimal real identification accents; no readable brand/model names. Functional plus/minus controls remain. No whole-object blur.
- Subjective line weight, simplified markings and fine surface shading remain available for user review through the three individual comparison boards. Local debranding is not a legal clearance guarantee.

No separate lens assets generated. No unrelated user images replaced.
