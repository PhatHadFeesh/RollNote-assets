# Rollback Stub

## Upload checkpoint

- User-approved finals and both review boards were uploaded in
  `RollNote-assets` commit `5a6e870`.
- App integration has not been performed; existing mappings and `imageStub`
  values remain unchanged.
- To roll back this upload, remove only this batch's root production PNGs
  and its two review boards from `RollNote-assets`.

This batch is review-only.

- Approved finals and review boards were uploaded in commit `5a6e870`.
- Their GitHub Pages paths use the `/RollNote-assets/assets/cameras/` base.
- No App image mapping, equipment record, or `imageStub` was changed.
- To discard the batch, remove only
  `public/assets/cameras/soviet-rangefinder-late-gaps-review-20260826/`.
- The earlier Soviet rangefinder review directories are independent and must
  not be removed with this directory.
