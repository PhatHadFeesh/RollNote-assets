# Prompts

Tool: built-in image_gen; transparent_background=true. Serial calls, no CLI/API fallback. Reference images are exact-model photos; last reference is style only.

## instax SQUARE 2 v1
Inputs: refs/instax-square-2-1.png; refs/instax-square-2-2.png; ../common-fixed-lens-icons-v-review-20260923/final/petri-color-35-rollnote-v1.png.

```text
Use case: stylized-concept.
Asset type: RollNote camera library transparent cutout, exactly 1536x1024 landscape RGBA.
Generate ONE Fujifilm instax SQUARE 2 Misty White camera. Input 1 is the authoritative exact front-view product reference. Input 2 is the same exact model's side-view reference for lens depth. Input 3 is STYLE ONLY, an existing RollNote illustration; do not borrow its camera geometry.
Keep the first image's straight-on front composition and exact proportions: rounded square pale gray body, viewfinder recessed upper left, narrow vertical amber indicator to its right, horizontal flash with rounded rectangular surround at upper right, ribbed left grip and circular shutter button above it. Large concentric lens slightly right of center, white outer ring, black ribbed circular face; tiny two sensor windows at left, central lens, white circular selfie mirror at right, crescent-shaped filter slider lower right. Preserve every element and location; no extra buttons.
Style: precise hard black ink contours, clean grayscale shaded illustration, moderately rounded manufactured edges, solid three-dimensional lens depth, crisp narrow edge highlights and occlusion shading. Match input 3's illustrated material quality, not a photograph, flat icon, soft clay toy or sketchy pencil drawing. Grayscale dominates, only a small subdued amber indicator as in reference.
Replace ONLY brand/model inscriptions with a few clearly unreadable geometric blocks matching their original local positions. No legible lettering, logos, watermark or captions. Do not blur camera details.
One isolated camera, centered, fully visible with ample transparent margin, fills about 76 percent of width and 82 percent of height without distortion. True transparent background, no surface, no cast shadow outside silhouette, no checkerboard baked in, no colored backdrop. Preserve genuine alpha. No props, hands, print, strap, accessories, extra camera or separate lens.
```

Output path: /Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/exec-05ccaa63-693d-4d25-8d9b-92a8fdb05f7c.png. Persisted to generated/instax-square-2-v1.png.

## instax mini Evo Cinema v1
Inputs: refs/instax-mini-evo-cinema-1.png; refs/instax-mini-evo-cinema-2.png; same Petri style reference as above.

```text
Use case: stylized-concept.
Asset type: RollNote camera library, exactly 1536x1024 landscape RGBA transparent cutout.
Generate ONE Fujifilm instax mini Evo Cinema camera, in a strictly straight-on FRONT view like input image 1. Input 1 is the exact frontal model reference, input 2 shows its side controls and depth only. Input 3 is the RollNote STYLE ONLY reference, never borrow its geometry.
Preserve this camera's distinctive narrow tall vertical cine-camera body and bottom textured grip. Do not make it a wide ordinary mini Evo. Lens is near upper part of narrow front, with rectangular sensor/mirror/flash cluster above; two little horizontal slots near top. Keep central lens concentric rings and serrated rim, small curved shoulder surfaces, recessed rectangular front panel above lower grip, bottom grip seam/panel and thin bottom plate. Right edge may show only a sliver of actual side dials as in front reference. No invented side-view broad face, no attached external viewfinder, no separate accessories.
Style: precise hard black ink outlines and detailed grayscale illustration, moderate rounded edges and convincing 3D volume from restrained edge highlights and recess shadows. Same mature RollNote look as input 3, not photorealistic, not flat icon, no watercolor, no clay toy. Black/charcoal body must have readable grayscale separation. Keep true narrow proportions; centered on wide transparent canvas at about 84 percent canvas height, with broad margins left and right.
Brand names, model text, lens lettering replaced ONLY locally with a few unreadable rectangular geometric dashes/blocks; never blur the whole body, no readable words, numerals, logos, captions or watermark.
True transparent alpha outside single isolated camera, no background, no surface, no exterior cast shadow, no baked checkerboard. Do not crop, stretch, rotate onto its side, duplicate, add film print or hands.
```

Output path: /Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/exec-1fa10400-d961-40fd-9c0a-2253a7e2b9ca.png. Persisted to generated/instax-mini-evo-cinema-v1.png.

## Polaroid OneStep+ v1
Inputs: refs/polaroid-onestep-plus-1.jpg; refs/polaroid-onestep-plus-3.jpg; same Petri style reference.

```text
Use case: stylized-concept.
Asset type: RollNote library camera cutout, 1536x1024 landscape, 8-bit RGBA with true transparent alpha.
ONE Polaroid Originals OneStep+ black camera, not OneStep 2, not Now+. Input 1 is the exact authoritative FRONT photograph. Input 2 is an additional exact-model photograph. Input 3 is STYLE ONLY from RollNote, never use its geometry.
Strictly front view. Preserve black squared upper front panel and projecting wide lower film-ejection box; central recessed circular lens with fine concentric ribs; tall rectangular flash on viewer left; small square PLUS-function button and small round sensor just to its right; large square recessed viewfinder upper right with exposure slider directly below it; red circular shutter bottom left of upper panel; small round sensor lower right of lens; small red switch peeking above top. Correct broad print slot across lower front, central recessed latch above it. Preserve body and control proportions of reference 1 and moderate physical depth, do not substitute a white OneStep 2 shell.
Match RollNote style reference: crisp hard black contour linework, detailed restrained grayscale shading, slightly rounded manufactured edges, coherent moderate 3D volume, precise highlights and recess shadows, readable structure within dark body, not flat symbol, photo, sketch, soft clay or exaggerated glossy 3D. Color limited to real red shutter/tiny red switch and faint lens tint. Replace rainbow brand stripe with narrow neutral gray strips. Replace brand/model lettering and logos with unreadable geometric dashes in the SAME local positions. Keep the plain functional plus symbol on its button; it is a control, not a brand logo. No readable brand text or captions.
Single isolated camera centered, fully visible with generous margins, about 78 percent canvas width, correct aspect ratio. Genuine transparent background outside silhouette; no floor, no cast shadow outside object, no glow, no baked checkerboard, no hands, film prints, straps or other objects.
```

Output path: /Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/exec-8726f34a-d283-4ae0-afa1-12d6e00c93e2.png. Persisted to generated/polaroid-onestep-plus-v1.png.

## instax mini Evo Cinema local revision v2
Input: generated/instax-mini-evo-cinema-v1.png. V1 has non-reference red ticks; retained in rejected as a non-approved intermediate.

```text
Use case: precise-object-edit. Edit the attached RollNote instax mini Evo Cinema illustration only. Change ONLY the small RED geometric ticks on the circular lens ring to neutral LIGHT GRAY matching the other gray marks. Also neutralize any red tint if present on all colored ticks. Keep all other camera geometry, front view, narrow vertical silhouette, black hard-line illustration style, shading, texture, lens, grip, controls, local unreadable geometric debranding and composition exactly unchanged. Do not add text or change the camera to a different model. Preserve 1536x1024 RGBA dimensions and TRUE TRANSPARENT background alpha; no backdrop, no checkerboard, no exterior glow/shadow. Output the complete single camera, not a crop.
```

Output path: /Users/mac/.codex/generated_images/019e5ef7-673c-7001-b31d-67f87b1dd6a3/exec-a08ae7c2-f4b7-40a1-8af3-3b5a363b8349.png. Persisted to generated/instax-mini-evo-cinema-v2.png; accepted final is instax-mini-evo-cinema-rollnote-v1.png (first approved version).
