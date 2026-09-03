# Camera Image Generation Priority

Updated: 2026-08-23

## Primary rule

Future batches prioritize highly searched, widely recognized, and frequently featured cameras before obscure catalog completion.

Brand order and release chronology are secondary. A famous individual model may be generated before the rest of its parent series.

## Mandatory duplicate gate

Before any generation call:

1. Search the local camera assets, review folders, remote URL mappings, aliases, regional names, and child-model names.
2. Reuse an existing qualified image when one already represents the exact child model.
3. Do not regenerate merely because a popular model appears near the top of a new ranking.
4. Regenerate only when the existing image is demonstrably wrong, below the approved style standard, or explicitly rejected by the user.

## Ranking signals

Rank missing models using current evidence rather than intuition alone:

- Search demand and trend visibility: 40%
- Social-media and creator visibility: 25%
- Resale-market listing and discussion frequency: 15%
- Visual recognizability and collector reputation: 10%
- RollNote library coverage gap: 10%

Use Google Trends or equivalent search evidence when available, then cross-check creator coverage and active marketplace presence. Record the evidence date because popularity changes.

## Provisional high-visibility gap pool

Verify current popularity before fixing the order:

- Yashica T5 / T5D
- Ricoh GR1s / GR1v
- Konica Big Mini BM-201 / BM-301 and notable child variants
- Lomo LC-A / LC-A+
- Other high-visibility compact or instant models discovered during the live check

The pool is not permission to skip exact child-model research. Each visually distinct child model receives its own asset.

## Production standard

- Use real-camera references and preserve identifying geometry and controls.
- Prefer a straight front view unless the mechanism requires another view.
- Match the early RollNote hard-line style: crisp outlines, bounded tones, restrained depth, and mechanically readable detail.
- Keep exact branded markings only in real-camera references and rollback/review sources. Before an asset is eligible for App integration, create a non-destructive trademark-softened variant with localized blur over brand wordmarks, model badges, and branded lens text.
- Preserve generic technical markings such as focal length and aperture where practical. Do not let logo blur soften body edges, controls, finder windows, lens glass, or the overall illustration.
- Treat trademark softening as a risk-reduction presentation choice, not as proof of legal clearance.
- Deliver transparent 1536 x 1024 RGBA PNG assets.
- Keep generated sources, review boards, status notes, and rollback stubs.
- Upload to RollNote-assets and connect through a remote URL only after visual approval.
