# Quality Review

- All four final images: 1536 x 1024, 8-bit RGBA PNG. Previews: 320 x 213 RGBA. Boards: 2200 x 1600 RGBA.
- Alpha range is 0..254, preserved from the generator. Fully transparent pixels: T3 59.58%, EF3 47.96%, 636 60.15%, LiPlay+ 67.89%. These are real alpha cutouts, not opaque black or checkerboard backgrounds.
- T3 top-left corner has alpha 1/255; all other sampled corners are 0. This is negligible generator residue, not a painted background. No opaque edge matte or visible halo was observed on checkerboards. Originals retained byte-for-byte rather than destructive thresholding.
- Polaroid raised-flash open gaps tested at (560,335) and (950,335): both alpha 0.
- Front-view proportions and distinguishing elements reviewed against the two references for every camera. Grayscale hard outlines, controlled depth and local unreadable brand marks are consistent across this batch. Integral lenses retained; no separate lens product generated.
- T3: regional T Scope reference, wide grip, three-window upper bank, lower sliding lens cover.
- EF3: white-gray front, circular lens/meter, distinct front timer and pop-up slider, rectangular finder and flash.
- 636: raised flash, open struts, front close-up controls, deep film ejection housing; no Sun 660 sonar added.
- LiPlay+: upright slim body, left grip/shutter and stepped square lens surround, distinguished from ordinary LiPlay.
- AI illustration is not a dimensionally certified engineering drawing. User visual review remains appropriate for fine control shapes and subjective style.
- Local debranding is a visual treatment, not a guarantee of intellectual-property clearance.

## SHA-256

- yashica-t3-rollnote-v1.png: 094894fd691adbba7ad539e0df6459f39bfefacdae433a54127ef617dc0efaa6
- konica-c35-ef3-rollnote-v1.png: 6b040f90405651d853226062c9cca34e7bc49763ca45c8a05b74cd7d8808daaf
- polaroid-636-closeup-rollnote-v1.png: e569c57a30ec3aeb511ae467a3ff0c4b592f7f7e2d120a33245bb7003a44bfb4
- instax-mini-liplay-plus-rollnote-v1.png: 615117f64508d691754658c87620b74b597bbd92d3624b8de09cab404df8c4ef
