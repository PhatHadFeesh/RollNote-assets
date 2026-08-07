# Olympus Quickmatic Review Stub

Date: 2026-08-07

This folder preserves the recoverable review trail for the RollNote-style Olympus Quickmatic group before the generated camera originals are connected through the remote asset repository.

## Connected Variants

- Quickmatic EE S 36mm f/2.8 -> `olympus-quickmatic-ees-f28-rollnote-v1.png`
- Quickmatic EE S 36mm f/3.5 -> `olympus-quickmatic-ees-f35-rollnote-v1.png`
- Quickmatic EE M -> `olympus-quickmatic-eem-rollnote-v1.png`
- Quickmatic 600 -> `olympus-quickmatic-600-rollnote-v1.png`

## Source References

- Quickmatic EE S f/3.5: Science Museum Group object page, `source-sciencemuseum-quickmatic-ees.html`, with local image `sciencemuseum-quickmatic-ees-f35.jpg`.
- Quickmatic EE S supplemental body reference: As Minhas Camaras blog page, `source-asminhascamaras-quickmatic-ees.html`, with local image `asminhascamaras-quickmatic-ees-f35-front.jpg`.
- Quickmatic EE M: James Ollinger camera collection page, `source-jollinger-olympus-eem.html`, with local image `jollinger-quickmatic-eem-front.jpg`.
- Quickmatic 600: Wikimedia Commons file page, `source-wikimedia-quickmatic-600.html`, with local image `wikimedia-quickmatic-600-front.jpg`.
- The Museum Victoria Quickmatic 600 page resolved to a Cloudflare challenge and was kept only as `source-museumsvictoria-quickmatic-600.html`, not used as a visual source.

The reference board is `olympus-quickmatic-reference-board.png`.

## Generated Sources

Green-screen originals are kept in `generated/`:

- `generated/olympus-quickmatic-ees-f28-rollnote-v1-green.png`
- `generated/olympus-quickmatic-ees-f35-rollnote-v1-green.png`
- `generated/olympus-quickmatic-eem-rollnote-v1-green.png`
- `generated/olympus-quickmatic-600-rollnote-v1-green.png`

Final transparent PNGs are stored one level up in `public/assets/cameras/` and mirrored to RollNote-assets before app connection. Chroma-key validation passed with transparent corners and `opaque_green=0` for all final PNGs. The group preview is `olympus-quickmatic-preview-v1.png`.

## Notes

The f/2.8 EE S variant is derived from the same EE S body references plus documented lens-spec differences because the local review set did not find a separate clean front-facing f/2.8 body photograph. The generated f/2.8 image keeps the same EES body but uses a subtly larger, deeper lens treatment than the f/3.5 version.

## Rollback

Remove this review folder and these four final PNGs from RollNote-assets, then remove the `cam-olympus-quickmatic` entry from `CAMERA_VARIANT_ASSETS` and clear `imageUrl` / `imageStub` from the corresponding `src/data.js` camera entry.
