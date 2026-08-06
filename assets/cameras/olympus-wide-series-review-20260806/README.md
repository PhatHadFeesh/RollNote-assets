# Olympus Wide Series RollNote Assets

Date: 2026-08-06

## Final transparent assets

- `../olympus-wide-rollnote-v1.png`
- `../olympus-wide-e-rollnote-v1.png`
- `../olympus-wide-super-rollnote-v1.png`
- `../olympus-wide-ii-rollnote-v1.png`

## Review material

- `olympus-wide-series-reference-board.png`: local comparison board.
- `olympus-wide-series-preview-v1.png`: final RollNote-style preview board.
- `references/biofos-35-wide.gif`: Olympus 35 Wide reference.
- `references/biofos-35-wide-e.gif`: Olympus 35 Wide E reference.
- `references/biofos-35-wide-super.gif`: Olympus Wide Super reference.
- `references/flickr-wide-ii.jpg`: Olympus Wide II top-plate reference.
- `generated/*-green.png`: preserved chroma-key source images.
- `rejected/endoscopy-wide-ii-sample-photo-not-camera.jpg`: rejected because it is a sample photo, not a camera body reference.
- `rejected/olympus-wide-ii-reject-v1-overstated-controls-readable-text.png`: rejected for overstated top controls and readable/inaccurate text.
- `rejected/olympus-wide-ii-reject-v2-green-window.png`: rejected because the finder used green highlights that would be removed during chroma-key extraction.

## Notes

- Wide, Wide E, and Wide Super were matched directly to available front-facing references.
- Wide II public front-facing material was scarce in the local review set. The final asset uses the 35 Wide front layout plus documented Wide II top-plate changes: film advance lever, rewind knob with crank, middle bright-frame window, and left viewfinder window.
- Final transparent PNGs were cut from flat chroma-key sources with transparent corners and no opaque green residue.
- Runtime loading should use the remote asset base URL through `ios:sync:github-assets`, `android:sync:github-assets`, or `android:assemble:github-assets`; these PNGs should not be bundled into the app package.

## Rollback

Remove the `cam-olympus-wide-series` entry from `CAMERA_VARIANT_ASSETS`, remove `imageUrl` and `imageStub` from the `cam-olympus-wide-series` data entry, and revert/copy back the previous remote asset set if needed.
