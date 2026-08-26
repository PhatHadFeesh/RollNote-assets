# Rollback Stub

## Upload checkpoint

- User-approved finals and both review boards were uploaded in
  `RollNote-assets` commit `5a6e870`.
- App integration has not been performed; existing mappings and `imageStub`
  values remain unchanged.
- To roll back this upload, remove only this batch's root production PNGs
  and its two review boards from `RollNote-assets`.

This is a review-only batch. No App source or remote asset mapping has been
changed yet.

## Intended Future Mapping

- Parent: `cam-kodak-ektar-h35`
- Variant `Ektar H35`: `kodak-ektar-h35-rollnote-v1.png`
- Variant `Ektar H35N`: `kodak-ektar-h35n-rollnote-v1.png`
- Variant `M35`: `kodak-m35-rollnote-v1.png`
- Variant `M38`: `kodak-m38-rollnote-v1.png`

## Connection Rule

After user approval, upload selected files to `RollNote-assets` first and use
their remote GitHub Pages URLs in the App. Preserve the parent's existing
image state in `imageStub`, record the remote asset commit, and add a rollback
instruction that removes only these four variant mappings. Do not replace the
parent image or the `Ultra F9` mapping while connecting this batch.
