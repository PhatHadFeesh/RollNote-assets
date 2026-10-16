# Quality review

2026-10-16. Built-in image_gen used serially; no CLI fallback or alpha postprocessing. Three v1 originals accepted after visual comparison. No rejected generations.

| File | Dimensions / mode | Alpha range | Fully transparent pixels | Alpha >=250 pixels |
| --- | --- | --- | --- | --- |
| instax-mini-8-plus-rollnote-v1.png | 1536x1024 / RGBA | 0-254 | 601015 | 953326 |
| polaroid-impulse-af-rollnote-v1.png | 1536x1024 / RGBA | 0-254 | 901331 | 650104 |
| polaroid-onestep2-viewfinder-rollnote-v1.png | 1536x1024 / RGBA | 0-254 | 681661 | 868832 |

PNG IHDR: 8-bit RGBA, color type 6. Corners alpha <=1; generated native alpha retained (maximum 254 rather than 255). Near-transparent antialias pixels outside silhouettes are retained, not silently clipped. Checkerboard composite inspection confirms no visible rectangular backdrop or halo. The dark glow visible in tool raw previews is not a composited background.

- mini 8+: front view; integral selfie mirror, left finder/shutter, flash/sensor pair, power button and rounded body retained. White/gray representative, not a color-variant duplication. Hard outline and lens relief match RollNote style.
- Impulse AF: straight front; raised flash/open lens, gold sonar behind horizontal grille, stacked right optical windows, red trim and film exit retained. Differs from non-AF inventory art.
- OneStep 2 Viewfinder: front view; enlarged finder housing, concentric lens, flash/timer/sensors, red shutter, yellow exposure slider and film exit retained. No OneStep+ Bluetooth control added.
- Branding/model words replaced only locally by unreadable geometric marks; functional power/exposure pictograms retained. This is a visual treatment, not a legal determination of clearance.
- All three boards pair only matching models. Mini references show two finishes; Impulse references show open/closed flash states. Sources are in SOURCES.md.
- Moderate stylized depth rather than literal engineering reconstruction; user can review contour strength and perspective using boards. No separate lens assets produced.
