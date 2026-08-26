# Rollback Stub

## Upload checkpoint

- User-approved finals and both review boards were uploaded in
  `RollNote-assets` commit `5a6e870`.
- App integration has not been performed; existing mappings and `imageStub`
  values remain unchanged.
- To roll back this upload, remove only this batch's root production PNGs
  and its two review boards from `RollNote-assets`.

This batch contains review-only assets.

- Production camera mappings changed: none
- Existing production images replaced: none
- `RollNote-assets` uploads: none
- Remote asset URLs added: none
- App inventory integration: none

To discard the unapproved batch, remove only:

`public/assets/cameras/lomography-panoramic-motion-review-20260826/`

No remote or app restoration is required. Rejected source or candidate files remain in `rejected/` until the user completes review.
