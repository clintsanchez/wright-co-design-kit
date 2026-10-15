# Wright Co logo set (2026-10-15)

Version 0.1. Prepared by BlakSheep Creative. Nothing here has been approved by the owner, Cody Wright.

## Provenance

- **There is one logo: the supplied emblem.** Distressed bone varsity "WRIGHT CO" with rust bevels, on a dark soil Louisiana silhouette with grass and cattails, and "360-957-5865" on a banner under the lettering. It is the client's own raster art. No vector, layered or original-artist file has been supplied.
- **`source/` holds the originals, unchanged.**
  - `wright-co-llc-logo_on-transparent_1536x1024.png` is a byte-identical copy of `brand/assets/wright-co-llc-logo.png`. It is 1536 × 1024 RGBA and **already a clean transparent cut-out**: alpha is 0 outside the art, and the dark outer glow/drop shadow is part of the art's alpha. On a black page it looks like a "black vignette", but there is no black background in the file. The art itself occupies about 1263 × 971 px.
  - `wright-co-logo-white-bg_wrightco-llc-site_1536x1024.jpg` is `https://wrightco.llc/logo.jpg`, downloaded 2026-10-15. It is the same art flattened onto white, as a JPEG. Reference only; the PNG is the better source in every case.
- **Every other file is built from the PNG by `brand/tools/build_logo_variants.py`** (run `python3 -I brand/tools/build_logo_variants.py` from the repo root). The script only trims, resamples (Lanczos) and centres the supplied pixels on a canvas. Nothing is redrawn, retouched, recoloured or generated.
- **The phone number is baked into the art.** 360-957-5865 is confirmed as the public number (Clint Sanchez, BlakSheep Creative, 2026-10-14). It is a 360 (Washington) area code on a Louisiana business; that is correct and is not to be "fixed". If the public number ever changes, every file here is wrong and needs the no-phone emblem (see Missing).

## Files

Minimum size is the displayed width of the emblem itself. Below 240 px the phone digits and the distressing stop reading.

### `emblem/`

| File | What it is | Size | Ground | Minimum size |
|---|---|---|---|---|
| `wright-co-emblem-transparent-native-1263w.png` | **The master.** Source art trimmed to its bounding box, transparent | 1263 × 971, RGBA | Soil Black `#120C06`, Soil surfaces `#20150C` / `#2E1D10`, or a dark photo under a 60%+ Soil overlay | 240 px |
| `wright-co-emblem-transparent-1200w.png` | Same, downscaled | 1200 × 923, RGBA | As above | 240 px |
| `wright-co-emblem-transparent-2400w-upscaled.png` | Same, **upscaled ~1.9×** from the 1263 px art. No detail is added; it is soft at 100%. Use only where a layout demands a 2400 px file; never for large-format print | 2400 × 1845, RGBA | As above | 240 px |
| `wright-co-emblem-on-soil-square-2400.png` / `-1200.png` | Emblem centred on an opaque Soil Black square, clear space 1/10 of emblem width each side | 2400², 1200², RGB | Its own Soil ground | 300 px square |
| `wright-co-emblem-on-soil-landscape-2400x1257.png` / `-1200x628.png` | Emblem centred on an opaque Soil Black 1.91:1 canvas (link preview / OG / cover base) | 2400 × 1257, 1200 × 628, RGB | Its own Soil ground | 600 px wide |

The transparent files were checked composited on solid red at 2× zoom: edges, cattails and the coastline are clean, with no white or black halo. The soft dark shadow round the art is part of the supplied art and stays. **On white, Bone `#F9F7F4` or any light ground the shadow reads as a grey smudge.** On light pages, place the Soil square file inside a square-cornered Soil container instead (per `brand/identity.md` §02).

No recolour of a "vignette" to Soil Black was needed or done: the source is transparent, so the Soil files are a straight composite.

### `avatar/`

| File | Size | Use |
|---|---|---|
| `wright-co-avatar-emblem-on-soil-1024.png` | 1024 × 1024 | Master avatar; upload where a platform takes a large file |
| `wright-co-avatar-emblem-on-soil-512.png` | 512 × 512 | Google Business Profile, general |
| `wright-co-avatar-emblem-on-soil-400.png` | 400 × 400 | X / LinkedIn |
| `wright-co-avatar-emblem-on-soil-320.png` | 320 × 320 | Facebook / Instagram |
| `wright-co-avatar-emblem-on-soil-180.png` | 180 × 180 | Apple touch icon, small slots |

The emblem's whole bounding-box diagonal sits inside 88% of the inscribed circle, so a circular crop never clips the art (checked visually with a circle mask). The emblem is small inside the circle by design. **At 180 px and below the phone number does not read**, and at feed-avatar sizes (about 40 px) only the bone lettering band will register. Interim only: the drawn mark (Missing, item 5) replaces it.

### `favicon/` — INTERIM, needs a drawn mark

| File | Size |
|---|---|
| `favicon-W-crop-master.png` | 380 × 380, the crop before downscaling |
| `favicon-64.png`, `favicon-48.png`, `favicon-32.png`, `favicon-16.png` | as named |
| `favicon.ico` | 16, 32, 48 and 64 in one file |

The "W" of WRIGHT cropped straight from the supplied art and padded onto Soil Black. Checked visually at 1× and 4× nearest-neighbour:

- **64 and 48 px:** reads as a bone W on dark. Acceptable.
- **32 px:** reads as a W, but the texture turns to noise and the rust bevel is lost.
- **16 px: illegible.** A light smear on dark; the W is not identifiable.
- The crop has hard edges where it cuts through the grass above the W and the banner rule at its lower right. Visible at 64 px.

**Status: interim — needs a drawn mark.** Ship it only until a designer draws the flat mark (Missing, item 5).

## Non-negotiables

- **Composite the supplied files only.** Never redraw, trace, auto-vectorise, re-letter, retype, recolour, retouch or AI-generate the logo or any part of it: the lettering, the state, the grass, the cattails, the banner or the phone number. That includes "cleaning up" the distressing, removing the phone with generative fill, and setting "WRIGHT CO" in Graduate or any font as a stand-in for the logo.
- Never stretch, skew, rotate, outline or add a glow, shadow, bevel or texture. Never crop into the art except for the interim favicon above.
- Never add "LLC", a tagline, a second phone number, a URL or "Est. 20XX" to the artwork.
- Dark grounds only: Soil Black and the Soil surfaces, or a dark photo under a 60%+ Soil overlay. On light grounds, use the Soil square inside a square-cornered Soil container.
- Clear space: one-tenth of the emblem's width on every side.
- Minimum 240 px wide on screen, 2 in in print. Print larger than about 4 in wide needs the vector master (Missing, item 1); the 1263 px art prints about 4.2 in at 300 dpi.
- Do not use the 2400w upscale for print or as a source for any further work.

## Missing (needs a designer or the original artist)

1. **Vector (SVG / AI / EPS / PDF) master.** None exists. Do not auto-trace the raster; the grain and grass turn to noise. Ask Cody who made the logo and whether layered or vector files exist.
2. **No-phone emblem.** The planned new primary (`brand/identity.md` §02, item 1). Not possible by compositing; the banner and digits sit on top of the art.
3. **Flat horizontal wordmark.** "WRIGHT CO" redrawn flat in the emblem's varsity letterforms for headers, email signatures and invoices. Until it exists, headers use the emblem at 240 px or more, or no logo.
4. **One-colour versions** (Bone, Soil Black, Rust) for embroidery, one-ink print, vinyl, stamps and engraving.
5. **Drawn small mark.** The simplified Louisiana silhouette with a single bone "W", for favicon, avatar, hat front and app icon. Replaces the interim favicon and the small avatars.

Spec for all five: `brand/identity.md` §02. Full kit rules: `../../8 - Asset Manifest and Production Rules.md`.
