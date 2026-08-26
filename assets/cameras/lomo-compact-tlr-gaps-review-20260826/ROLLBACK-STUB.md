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
- `imageStub` changes: none required at review stage

To discard the unapproved batch, remove only:

`public/assets/cameras/lomo-compact-tlr-gaps-review-20260826/`

No remote or App restoration is required.

After approval only, upload selected finals to `RollNote-assets`, use their
GitHub Pages URLs for variant-specific App mappings, preserve every previous
mapping in `imageStub`, and record the remote commit plus exact rollback
instructions before integration.
