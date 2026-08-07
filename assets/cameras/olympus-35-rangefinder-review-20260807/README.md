# Olympus 35 SP / RC / RD Review Stub

Date: 2026-08-07

This folder preserves the recoverable review trail for the RollNote-style Olympus 35 rangefinder group before the generated camera originals are connected through the remote asset repository.

## Connected Variants

- 35 SP -> `olympus-35-sp-rollnote-v1.png`
- 35 SPn -> `olympus-35-spn-rollnote-v1.png`
- 35 UC -> `olympus-35-uc-rollnote-v1.png`
- 35 RC -> `olympus-35-rc-rollnote-v1.png`
- 35 RD -> `olympus-35-rd-rollnote-v1.png`
- 35 DC -> `olympus-35-dc-rollnote-v1.png`
- 35 EC -> `olympus-35-ec-rollnote-v1.png`
- 35 EC2 -> `olympus-35-ec2-rollnote-v1.png`
- 35 ECR -> `olympus-35-ecr-rollnote-v1.png`
- 35 ED -> reused existing `olympus-35-ed-rollnote-v1.png`

## Source References

- 35 SP / 35 RC: 35mmc reference page, `source-35mmc-35-sp-35-rc.html`, with local front references `35mmc-35-sp-front.jpg`, `35mmc-35-rc-front.jpg`, and `35mmc-sp-rc-twins-front.jpg`.
- 35 SPn: 35mmc reference page, `source-35mmc-35-spn.html`, with local front reference `35mmc-35-spn-front.jpg`.
- 35 UC: Classic Cameras reference page, `source-classiccameras-35-uc.html`, with local front reference `classiccameras-35-uc-front.jpg`.
- 35 RD: Broken Camera reference page, `source-brokencamera-35-rd.html`, with local front reference `brokencamera-35-rd-front.jpeg`.
- 35 DC: 35mmc and Broken Camera references, `source-35mmc-35-sp-dc.html` and `source-brokencamera-35-dc.html`, with local front reference `brokencamera-35-dc-front.jpeg`.
- 35 EC / EC2: 35mmc and Broken Camera references, `source-35mmc-35-ec-ec2.html` and `source-brokencamera-35-ec.html`, with local front references `brokencamera-35-ec-front.jpeg` and `35mmc-35-ec-ec2-front.jpg`.
- 35 ECR: Randomphoto reference page, `source-randomphoto-35-ecr.html`, with local references `randomphoto-35-ecr-camera-013.jpg` and `randomphoto-35-ecr-camera-014.jpg`.
- The Ken Rockwell SP page download resolved to a Cloudflare challenge and was kept only as `source-kenrockwell-35-sp.html`, not used as a visual source.

The reference board is `olympus-35-rangefinder-reference-board.png`.

## Generated Sources

Green-screen originals are kept in `generated/`:

- `generated/olympus-35-sp-rollnote-v1-green.png`
- `generated/olympus-35-spn-rollnote-v1-green.png`
- `generated/olympus-35-uc-rollnote-v1-green.png`
- `generated/olympus-35-rc-rollnote-v1-green.png`
- `generated/olympus-35-rd-rollnote-v1-green.png`
- `generated/olympus-35-dc-rollnote-v1-green.png`
- `generated/olympus-35-ec-rollnote-v1-green.png`
- `generated/olympus-35-ec2-rollnote-v1-green.png`
- `generated/olympus-35-ecr-rollnote-v1-green.png`

Final transparent PNGs are stored one level up in `public/assets/cameras/` and mirrored to RollNote-assets before app connection. Chroma-key validation passed with transparent corners and `opaque_green=0` for all connected final PNGs. The group preview is `olympus-35-rangefinder-preview-v1.png`.

## Notes

The 35 ED image was already produced and connected in the previous Auto Eye / 35 LE group, so this group reuses that file to avoid regenerating an already available matching asset. The UI entry still exposes 35 ED in the 35 SP / RC / RD family because users may naturally search for it there.

## Rollback

Remove this review folder and the nine new final PNGs from RollNote-assets, then remove the `cam-olympus-35-rangefinder` entry from `CAMERA_VARIANT_ASSETS` and clear `imageUrl` / `imageStub` from the corresponding `src/data.js` camera entry. Keep `olympus-35-ed-rollnote-v1.png` if the previous Auto Eye / 35 LE group remains connected.
