# Rollback Stub

## Upload checkpoint

- User-approved finals and both review boards were uploaded in
  `RollNote-assets` commit `5a6e870`.
- App integration has not been performed; existing mappings and `imageStub`
  values remain unchanged.
- To roll back this upload, remove only this batch's root production PNGs
  and its two review boards from `RollNote-assets`.

The approved production PNGs were copied to the remote production camera
namespace in `RollNote-assets` commit `5a6e870`. Application data is still
unchanged.

## Current state

- Production asset mappings changed: none
- Remote asset URLs added: none
- App inventory records added: none
- Existing production images replaced: none

## Rollback

To discard this batch before approval, remove only:

`public/assets/cameras/lomography-family-variants-review-20260826/`

No app mapping, remote repository, or prior camera file requires restoration.

Rejected candidates and rejected LC-A 120 references are intentionally retained in `rejected/` until the user finishes review.
