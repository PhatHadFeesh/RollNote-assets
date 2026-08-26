# Rollback Stub

## Upload checkpoint

- User-approved finals and both review boards were uploaded in
  `RollNote-assets` commit `5a6e870`.
- App integration has not been performed; existing mappings and `imageStub`
  values remain unchanged.
- To roll back this upload, remove only this batch's root production PNGs
  and its two review boards from `RollNote-assets`.

This is a review-only batch. No App source or remote asset mapping has been
changed.

## Intended Future Mapping

- Parent `cam-reto-pano`, variant `PANO 35mm`:
  `reto-pano-rollnote-v1.png`
- Parent `cam-lomography-lca`, variant `LC-A+`:
  `lomo-lca-plus-rollnote-v1.png`
- Parent `cam-lomography-holga`, variant `Holga 120N`:
  `holga-120n-rollnote-v1.png`
- Parent `cam-lomography-diana`, variant `Diana F+`:
  `diana-f-plus-rollnote-v1.png`

## Connection Rule

After user approval, upload only the selected files to `RollNote-assets` and
use their remote GitHub Pages URLs in the App. Before changing any mapping,
preserve each parent's current image state in `imageStub`, record the remote
asset commit, and add a rollback instruction that removes only these four
variant mappings. Do not replace parent images or modify sibling variants.
