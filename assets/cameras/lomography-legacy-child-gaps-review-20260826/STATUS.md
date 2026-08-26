# Status

## Batch

- Name: Lomography legacy child-variant gaps
- Date: 2026-08-26
- State: approved and uploaded, App integration pending
- Upload: completed in RollNote-assets commit `5a6e870`
- App integration: not performed

## Completed models

- Lomo LC-A 120
- Original Diana
- Diana Baby 110
- Holga 120GCFN

Full-library filename and inventory searches found no qualified image for these four variants. Original LOMO LC-A was excluded because the accepted LC-A+ review candidate was generated from the original LC-A hardware reference and already covers that physical body.

## Final assets

- `final/lca-120-rollnote-v1.png`
- `final/diana-original-rollnote-v1.png`
- `final/diana-baby-rollnote-v1.png`
- `final/holga-120gcfn-rollnote-v1.png`

All four files are 1536x1024, 8-bit RGBA PNGs with real transparent pixels.

## Review boards

- `lomography-legacy-child-gaps-review-board-a-v1.png`: Lomo LC-A 120 and Original Diana
- `lomography-legacy-child-gaps-review-board-b-v1.png`: Diana Baby 110 and Holga 120GCFN

## Quality control

- Two real structural references are retained for every model with exact source URLs.
- LC-A 120 references come from the official Lomography product gallery and replace invalid mixed 35mm/sample references rejected in the earlier family batch.
- Exact front view is used for all four candidates.
- LC-A 120 preserves its tall square proportions, center finder hump, broad pebbled panels, tall lens-cover housing, open square lens, top controls, side lugs, and right front lever. It is visibly distinct from the existing 35mm LC-A body.
- Original Diana preserves its flatter vintage body, muted turquoise ribbed top shell, raised square finder, black pebbled panels, silver-ringed lens, left winding knob, and simple front control. Modern Diana F+ flash hardware is omitted.
- Diana Baby 110 preserves its genuinely compact wide body, cyan top shell, center finder, black pebbled panels, single left control, smooth lens panel, and silver-rimmed 12 mm lens. Loose accessories and packaging are omitted.
- Holga 120GCFN preserves the tall 120 body, large left advance knob, top color-flash selector, built-in center flash, right finder, square lens board, glass lens, pebbled panels, and metal side clips. It is visibly distinct from the flashless 120N.
- Early RollNote styling is retained: hard black outer contours, crisp internal linework, monochrome-forward shading, modest rounding, moderate lens/body depth, and limited cyan or lens-glass recognition color.
- Brand names, model wording, logos, lens inscriptions, numbers, and instructional labels are replaced locally with crisp unreadable geometric marks. No whole-camera blur was used.
- Edge-connected generated checkerboards were removed. Dimensions, RGBA encoding, alpha, framing, and review-board model pairing were visually verified.
- `npm run build`: passed with Vite 8.0.14 on 2026-08-26 (1877 modules transformed).

## Next candidates

After another full-library duplicate check, a useful next group is Holga 135, LOMO Smena 8M, Lomography Lubitel 166+, and Fisheye Baby 110. Holga 120GN should be treated cautiously because its visible body is nearly identical to the accepted 120N candidate.
