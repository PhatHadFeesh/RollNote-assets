# Olympus 35 S / SII RollNote Assets

Date: 2026-08-06

## Final transparent assets

- `../olympus-35-s-rollnote-v1.png`
- `../olympus-35-s-f35-rollnote-v1.png`
- `../olympus-35-sii-rollnote-v1.png`
- `../olympus-35-sii-f18-rollnote-v1.png`
- `../olympus-35-sii-f28-rollnote-v1.png`

## Review material

- `olympus-35-s-series-reference-board.png`: local comparison board for the real references.
- `olympus-35-s-series-preview-v1.png`: final RollNote-style preview board.
- `references/source-biofos-35.html`: Biofos Olympus 35 lineage page.
- `references/biofos-35s-18-external-delay.gif`: 35S 1.8 reference.
- `references/biofos-35s-gold-s.gif`: 35S Gold S reference; the page listed `35goldS.gif`, but the accessible server path was `35golds.gif`.
- `references/biofos-35s-28.gif`: 35S / Tower 35S 2.8 reference.
- `references/biofos-35s-20.gif`: 35S 2.0 reference.
- `references/source-pheugo-35sii.html`, `references/pheugo-35sii-full.jpg`, `references/pheugo-35sii-top1.jpg`: 35-SII body and top-plate references.
- `references/source-cameracollector-35s.html`, `references/cameracollector-35s.jpg`, `references/cameracollector-35sii.jpg`, `references/cameracollector-35s-vs-35sii.jpg`: 35-S and 35-SII comparison references.
- `references/source-flickr-35sii.html`, `references/flickr-35sii-variation.jpg`: S-II variation reference.
- `generated/*-green.png`: preserved chroma-key source images.

## Notes

- The 35 S, 35 SII, 35 SII 1.8, and 35 SII 2.8 assets were matched to visible 35-S / 35-SII body differences: upper front window layout, lens size, gold S-style badge presence, and top-plate control proportions.
- The 35 S-3.5 asset is intentionally treated as a smaller-lens early 35 S variant because direct, clear public f/3.5 front references were sparse in the local review set. It is documented as an inference and should be replaced if a better direct reference is found.
- Final transparent PNGs were cut from flat chroma-key sources with transparent corners and no opaque green residue.
- Runtime loading should use the remote asset base URL through `ios:sync:github-assets`, `android:sync:github-assets`, or `android:assemble:github-assets`; these PNGs should not be bundled into the app package.

## Rollback

Remove the `cam-olympus-35-s-series` entry from `CAMERA_VARIANT_ASSETS`, remove `imageUrl` and `imageStub` from the `cam-olympus-35-s-series` data entry, and revert/copy back the previous remote asset set if needed.
