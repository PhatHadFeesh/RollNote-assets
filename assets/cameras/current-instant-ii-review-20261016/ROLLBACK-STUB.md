# Rollback

Batch: current-instant-ii-review-20261016.

Exact mappings to add to CAMERA_ARTWORK_CATCHUP:
- cam-instax-square-analog / SQUARE 2 -> instax-square-2-rollnote-v1.png. New child; preserve family default and SQ1/SQ6/SQ40 assets.
- cam-instax-mini-evo / mini Evo Cinema -> instax-mini-evo-cinema-rollnote-v1.png. New hybrid-instant child using instax mini film; preserve ordinary mini Evo and finish options.
- cam-polaroid-modern-itype / OneStep+ -> polaroid-onestep-plus-rollnote-v1.png. Prior exact asset: /assets/cameras/polaroid-onestep2-rollnote-v1.png, status generated.

Existing withCameraArtworkCatchup stores previousAsset, previousImageUrl and the original family imageStub. Remove only these three reviewed entries to restore earlier resolution. Remove this batch's added child aliases/options by removing those entries; do not delete prior family records or assets. Previous default remote version: 0f5c052.

Preserve all refs, generated, rejected and final files, and published files for existing links. No unrelated git changes or user data may be reverted. New builds must be under freshly-created /tmp directories.
