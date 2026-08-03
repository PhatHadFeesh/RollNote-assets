# Olympus FTL Review Assets

Generated on 2026-08-03 for RollNote.

This folder keeps recoverable review material for the Olympus FTL camera asset:

- `references/`: real-camera references and source page captures.
- `generated/`: chroma-key source generation.
- `transparent/`: local alpha cutout draft.
- `ftl-preview-v1.png`: side-by-side reference check.
- `rejected/non-body/`: fetched files that were not camera-body references.

Final app/remote asset:

- `/assets/cameras/olympus-ftl-rollnote-v1.png`

Reference sources used:

- Wikimedia Commons / Wikipedia Olympus FTL front image: `https://commons.wikimedia.org/wiki/File:Olympus_FTL_front.jpg`
- Wikipedia Olympus FTL model page: `https://en.wikipedia.org/wiki/Olympus_FTL`
- Biofos Olympus FTL page for production context and system references: `https://www.biofos.com/cornucop/ftl.html`
- Mike Eckman Olympus FTL page was checked for context, but fetched sample photos were moved to `rejected/non-body/` and not used as body references: `https://mikeeckman.com/2023/07/olympus-ftl-1971/`

Visual notes:

- Use a front-facing FTL body, not an OM-series body.
- Preserve the tall traditional SLR pentaprism, left-front `FTL` marking, prism-front `OLYMPUS` marking, silver top plate, black leatherette, and M42 Zuiko lens feel.

Rollback:

1. Remove `imageUrl` and `imageStub` from `cam-olympus-ftl` in `src/data.js`.
2. Remove `cam-olympus-ftl` from `CAMERA_VARIANT_ASSETS`.
3. Remove `OLYMPUS_FTL_REVIEW_PREVIEW_URL` if unused.
4. The generated source, reference, and transparent files in this folder can be reused to restore or regenerate the FTL asset.
