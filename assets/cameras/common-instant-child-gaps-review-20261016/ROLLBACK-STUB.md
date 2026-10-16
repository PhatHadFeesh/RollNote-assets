# Rollback

Batch: common-instant-child-gaps-review-20261016.

- cam-instax-mini-8-9 / mini 8+ -> instax-mini-8-plus-rollnote-v1.png. Previous exact asset: /assets/cameras/instax-mini-8-rollnote-v1.png. Preserve mini 8 and mini 9 siblings.
- cam-polaroid-impulse / Impulse AF -> polaroid-impulse-af-rollnote-v1.png. Previous exact asset: /assets/cameras/polaroid-impulse-rollnote-v1.png. Preserve Impulse and Impulse Portrait.
- cam-polaroid-modern-itype / OneStep 2 Viewfinder -> polaroid-onestep2-viewfinder-rollnote-v1.png. New generation child. Preserve OneStep 2 and OneStep+.

withCameraArtworkCatchup stores previousAsset, previousImageUrl and original family imageStub. Remove only these three reviewed entries to restore original mapping and remove newly added exact aliases/options. Previous default remote asset version: a6babea. Do not delete previous family records/assets or any published URLs.

Preserve refs, generated, final and rejected history. Do not revert unrelated dirty files or user data. All tests/builds use fresh /tmp directories; no existing dist writes.
