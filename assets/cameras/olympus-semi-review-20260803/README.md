# Semi Olympus Review Assets

Generated on 2026-08-03 for RollNote.

This folder keeps recoverable review material for the Semi Olympus camera group:

- `references/`: real-camera references and source page captures.
- `generated/`: chroma-key source generations.
- `transparent/`: local alpha cutout drafts.
- `semi-reference-board.png`: reference-only board used to compare available sources.
- `semi-preview-v1.png`: reference check for the generated cutouts.

Final app/remote assets:

- `/assets/cameras/olympus-semi-i-rollnote-v1.png`
- `/assets/cameras/olympus-semi-ii-rollnote-v1.png`
- `/assets/cameras/olympus-semi-standard-rollnote-v1.png`

Reference sources used:

- OM Digital product history, Semi-Olympus I: `https://www.om-digitalsolutions.com/en/product-history/semi-olympus_1/`
- Biofos folding-camera collection notes and Semi I / Semi II reference images: `https://www.biofos.com/coll/subcoll/folder.html`
- Leitz Auction Olympus Standard Prototype reference images: `https://www.leitz-auction.com/en/Olympus-Standard-Prototype/AI-31-35213`

Visual notes:

- `Semi-Olympus I` is treated as the narrow vertical 120 folding camera with the front bed opened and a side sports finder.
- `Semi-Olympus II` is treated as a wider horizontal 120 folding camera with a pop-up finder and opened bellows.
- `Semi-Olympus Standard` is visually distinct: an early rangefinder-style prototype, not a folding camera.

Rollback:

1. Remove `imageUrl` and `imageStub` from `cam-olympus-semi` in `src/data.js`.
2. Remove `cam-olympus-semi` from `CAMERA_VARIANT_ASSETS`.
3. Remove `OLYMPUS_SEMI_REVIEW_PREVIEW_URL` if unused.
4. The generated source, reference, and transparent files in this folder can be reused to restore or regenerate any variant.
