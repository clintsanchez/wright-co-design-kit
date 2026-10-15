# Wright Co.: Design Kit

Input folder for Claude Design (claude.ai/design). Prepared by BlakSheep Creative, 2026-10-15, version 0.1.

Wright Co. is a land clearing and home-site prep crew serving Hammond, Tangipahoa Parish and the Northshore in Louisiana, 360-957-5865, wrightco.llc. It takes wooded land to build-ready, in one order: 01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig.

**Nothing here is approved by the owner, Cody Wright, and he has seen none of it.** The name, the emblem, the colours sampled from it, the phone, the business email and the web address are the client's own. The tagline, the three offer names (The Homeplace Package, The Free Lot Walk, The Dirt Order) and the button pair are BlakSheep Creative decisions, usable now. The position, values, voice, colour roles, typefaces and every template are BlakSheep Creative proposals awaiting his sign-off. The emblem is his raster art; every logo file here is trimmed, resampled and centred from it, never redrawn. There are zero photographs. Start with `0 - READ ME FIRST.md`.

## Run order

1. **`1 - MASTER PROMPT.md`**: the master brand design kit, with three website page mockups (home, land clearing, The Homeplace Package). Run this first.
2. **`7 - SOCIAL TEMPLATE SYSTEM PROMPT.md`**: the social template system. Run it second, in the same Claude Design project, so it inherits the design system from step 1.

## Import steps for Claude Design

Claude Design has no API. A person does this by hand.

1. Open claude.ai/design and start a new project named **"Wright Co"**.
2. Give it this folder. Either upload the `design-kit` folder (or a ZIP of it), or use "Create here" and point it at a GitHub repository that holds it (see "Sharing": no repository has been created yet). If the whole client repository is used, tell Claude Design to work from `design-kit/` only.
3. Upload `assets/references/reference-kit-format_REFERENCE-ONLY.pdf` by hand. It is not in version control.
4. Create one design system for this client, so everything generated afterwards uses the same tokens.
5. Paste the launcher for the first run (below), or the full text of `1 - MASTER PROMPT.md`. It is self-contained and names the files to read.
6. Check the first run (next section) before going further.
7. Review the result against the quality checklist in `8 - Asset Manifest and Production Rules.md`.
8. Paste the second launcher, or the full text of `7 - SOCIAL TEMPLATE SYSTEM PROMPT.md`, in the same project.
9. Regenerate weak sections one at a time with a short prompt that names the section. A single "redo everything" prompt tends to go generic on the later sections.
10. Save exports to an `exports/` folder beside this file. A re-sync from a repository is one-way and does not rewrite pages already on the canvas.

The files in this folder are the source of truth. Claude Design is a viewer and a generator. Make changes here first, then re-sync or re-upload.

**If Claude Design is pointed at the whole client repository:** tell it to read `design-kit/` only. The rest of the repository holds working files, research that names competitors, and records that are not for any layout.

## What to check after the first run

| Check | Pass | If it fails |
|---|---|---|
| The emblem | Every logo on the canvas is one of the supplied files in `assets/logos/emblem/`, `avatar/` or `favicon/`, composited unchanged, 240 px wide or more, once per view | If it has been redrawn, traced, re-lettered, sharpened, recoloured, cleaned up, had its phone banner removed, or been given a tagline or "LLC", stop and tell Claude Design to composite the supplied file |
| The name in type | "WRIGHT CO" is never set in Graduate or any font as a stand-in for the logo. The header uses a labelled wordmark slot or the emblem at 240 px | Replace it with the slot or the supplied file |
| Grounds | The transparent emblem sits only on Soil Black, Soil Surface or Soil Elevated. On Bone or white it is the Soil square inside a square-cornered Soil container | Swap in `wright-co-emblem-on-soil-square-1200.png` in a Soil container |
| Missing logo versions | The vector master, no-phone emblem, flat wordmark, small mark and one-colour versions appear only as labelled slots | Delete anything drawn and restore the slot |
| Favicon and avatar | The supplied files, with the favicon labelled interim and its 16 px illegibility reported honestly | Restore the supplied files and the honest note |
| Photos | No photograph anywhere. Every photo position is a labelled slot whose label starts "Real job photo:" | Replace any stock, AI scene, illustrated lot, equipment render or blurred placeholder with a labelled slot |
| Colour | Dark-first soil palette from `tokens/css-tokens.css` only. One thing in rust per screen. No green, yellow or blue, no gradient, no shadow | Point Claude Design at the token file |
| Type | Graduate at weight 400 only with `font-synthesis: none`, uppercase, for display, H1, H2, eyebrows and numerals. Source Sans 3 for everything else. No faux bold | Correct the face and weight |
| Shape | Radius 2, 4 or 8 px, or a chamfer. No pills, no rounded buttons | Correct the radius |
| Buttons | "Book a Free Lot Walk" (solid Cattail Rust) and "Call or Text 360-957-5865" (outlined), equal width, primary first. The phone is a button, never a bare link | Correct the wording and the widths |
| The sequence | "01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig" everywhere, never re-ordered or renamed | Correct it |
| Offers | The Homeplace Package always with "Clear · Driveway · House Pad. One crew, one scope, build-ready."; The Dirt Order always with its subtitle | Restore the descriptor |
| Claims | No banned claim anywhere: see the prohibited list at the end of `6 - Brand Context and Prices.md`. No price, licence, rating, review, address, hours, "LLC", years-in-place or competitor phrasing | Delete the line. Do not soften it |
| Page mockups | Home, land clearing and The Homeplace Package follow the outlines in section 10 of the master prompt, at 360 px and 1440 px, and read correctly with the photo slots removed | Regenerate the page from its outline |
| Open items | Every unapproved item still shows `CONFIRM BEFORE PUBLISHING` | Restore the marker |

## Launcher messages

The two prompt files are long (about 150 KB and 75 KB). With this folder attached to the Claude Design project, paste the short launcher and let it read the file. If a launcher produces a thin result, paste the full prompt file instead.

**First run, master brand design kit:**

```text
Read `1 - MASTER PROMPT.md` in the attached folder in full and carry it out exactly. It is self-contained. Also read `0 - READ ME FIRST.md`, files `2` to `6`, `8 - Asset Manifest and Production Rules.md`, `assets/logos/README.md`, `assets/photos/PHOTO-MANIFEST.md` and `tokens/css-tokens.css`. If `reference-kit-format_REFERENCE-ONLY.pdf` is attached, use it for structure and depth only; it is another client's kit and none of its brand, facts, colours, type or wording applies. The two Markdown files in `assets/references/` ending REFERENCE-ONLY are generic agency templates, and the section map there is an agency record; the master prompt already covers them. Composite the supplied emblem, avatar and favicon files; never redraw, trace, retype or generate any part of the emblem, and never place the transparent emblem directly on a light ground. There are no photographs: every photo position is a labelled slot reading "Real job photo: [what]", with no stock, no AI scenes and no equipment renders. Do not pause for discovery; mark anything unresolved CONFIRM BEFORE PUBLISHING.
```

**Second run, same project, social template system:**

```text
Read `7 - SOCIAL TEMPLATE SYSTEM PROMPT.md` in the attached folder in full and carry it out exactly. It inherits the design system you just built. The supplied emblem and avatar files are the only brand marks; composite them unchanged, on Soil grounds only. There are no photographs: every photo position is a labelled slot reading "Real job photo: [what]". No review or testimonial content, no prices, no buttons drawn on graphics. Do not pause for discovery; mark anything unresolved CONFIRM BEFORE PUBLISHING.
```

## What is here

| Path | Contents |
|---|---|
| `0 - READ ME FIRST.md` | Status, brand facts, run order, priority order, open decisions |
| `1 - MASTER PROMPT.md` | Claude Design prompt: master brand design kit and three website page mockups |
| `2 - Brand Guidelines.md` | The binding limits, positioning, mission, vision, values, personality, audience, promise, differentiators, do and do not |
| `3 - Visual Identity.md` | Logo system and rules, colour, contrast, type, layout, components, photography |
| `4 - Brand Voice.md` | Voice, tone, writing rules, vocabulary, examples, SMS and phone scripts |
| `5 - Messaging.md` | Positioning, pitches, pillars with proof, trust signals, objections, calls to action, campaign themes |
| `6 - Brand Context and Prices.md` | Business facts, service area, services, offers, pricing rule, operational facts, competitors, the claims lists |
| `7 - SOCIAL TEMPLATE SYSTEM PROMPT.md` | Claude Design prompt: social templates |
| `8 - Asset Manifest and Production Rules.md` | Asset list, logo and image rules, AI image rules, platform rules, quality checklist, maintenance |
| `assets/logos/README.md` | The logo set's own guide: provenance, every file, grounds, sizes, the five missing versions |
| `assets/logos/emblem/wright-co-emblem-transparent-native-1263w.png` | **The master.** The supplied art trimmed to its bounding box, transparent, 1263 × 971. Soil grounds only, 240 px wide or more |
| `assets/logos/emblem/wright-co-emblem-transparent-1200w.png` | The same, 1200 × 923 |
| `assets/logos/emblem/wright-co-emblem-transparent-2400w-upscaled.png` | The same, upscaled to 2400 × 1845. Soft; never for print or further work |
| `assets/logos/emblem/wright-co-emblem-on-soil-square-2400.png`, `-1200.png` | The emblem on an opaque Soil Black square. For light pages, inside a Soil container |
| `assets/logos/emblem/wright-co-emblem-on-soil-landscape-2400x1257.png`, `-1200x628.png` | The emblem on an opaque Soil Black 1.91:1 canvas. Link preview, open graph, cover base |
| `assets/logos/avatar/wright-co-avatar-emblem-on-soil-1024.png`, `-512.png`, `-400.png`, `-320.png`, `-180.png` | The avatar, sized for a circle crop. The phone stops reading at 180 px and below |
| `assets/logos/favicon/favicon-W-crop-master.png`, `favicon-64.png`, `favicon-48.png`, `favicon-32.png`, `favicon-16.png`, `favicon.ico` | **Interim.** The "W" cropped from the art. Illegible at 16 px; replaced when a small mark is drawn |
| `assets/logos/source/wright-co-llc-logo_on-transparent_1536x1024.png` | The client's original, untouched. Reference only |
| `assets/logos/source/wright-co-logo-white-bg_wrightco-llc-site_1536x1024.jpg` | The same art flattened on white, from the live website. Reference only; never used |
| `assets/photos/PHOTO-MANIFEST.md` | Zero photos. The slot rule and the shot list for the owner |
| `assets/references/reference-kit-format_REFERENCE-ONLY.pdf` | Another client's finished kit, for structure and depth only. Git-ignored; uploaded by hand. See "Sharing" |
| `assets/references/master-brand-kit-template_REFERENCE-ONLY.md` | The agency's generic master brand kit template. File 1 covers every section of it (its section 1.5) and overrides it |
| `assets/references/universal-social-template-system_REFERENCE-ONLY.md` | The agency's generic social template prompt. File 7 accounts for all 43 sections and overrides it |
| `assets/references/social-prompt-universal-section-map.md` | Agency record of how file 7 maps to the universal social prompt. Not an instruction |
| `assets/references/.gitignore` | Keeps the reference PDF out of version control |
| `tokens/css-tokens.css` | Token values of record (a copy of `website/css-tokens.css`) |
| `source-manifest.json` | Kit files, their sources, bytes and sha256, date |

## Non-negotiables

- The emblem is never redrawn, traced, auto-vectorised, re-lettered, retyped, recoloured, retouched, sharpened, upscaled further or AI-generated, in whole or in part. Only the supplied files are composited. Nothing is added to the artwork: no tagline, no "LLC", no "Est.", no badge. The phone banner is never cropped, masked or painted out.
- The transparent emblem sits on Soil Black, Soil Surface, Soil Elevated, or a dark photo under a 60 percent or stronger Soil overlay. Never directly on white or Bone; there, the Soil square goes inside a square-cornered Soil container. Minimum 240 px wide on screen, 2 in in print; clear space one tenth of its width.
- "WRIGHT CO" is never set in Graduate or any font as the logo. The missing logo versions are labelled slots.
- The favicon is interim and is labelled so.
- Zero photographs: every photo position is a labelled slot "Real job photo: [what]". No stock, no AI-generated lots, machines, crews, people or places, no equipment renders, no Washington photos.
- Dark-first soil palette from `tokens/css-tokens.css` only. One thing in rust. No green, safety yellow or blue; no gradients; no shadows.
- Graduate at 400 only, with `font-synthesis: none`; Source Sans 3 for everything else.
- Radius 2 / 4 / 8 px or a chamfer. No pills, no rounded buttons.
- Buttons read exactly "Book a Free Lot Walk" and "Call or Text 360-957-5865", at equal width, primary first.
- The sequence reads "01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig" everywhere. The Homeplace Package and The Dirt Order always carry their descriptors.
- "Wright Co." with the period. No "LLC" anywhere except inside the web address.
- No licensed, insured, bonded or any credential. No star rating, review count or review quote. No price, range, per-acre rate or discount. No street address, hours or map pin. No years in Hammond or Louisiana; "Clearing and excavating since 2022" is the only history line.
- No pad height, flood promise, "we handle your permits", guarantee or "settles over winter".
- No competitor's name or phrasing, and nothing from the owner's separate business in another state.
- No link to the Facebook page until it is renamed and repointed.
- Anything unconfirmed stays visible as `CONFIRM BEFORE PUBLISHING`.

## Still missing

- The owner's approval of everything in this kit.
- A vector master of the emblem, and who made the original.
- The no-phone emblem, the flat horizontal wordmark, the drawn small mark and one-colour versions (briefs in `assets/logos/README.md`).
- Any photograph of a Wright Co. job in Louisiana; the before/after series from one fixed spot.
- The Free Lot Walk terms, the Homeplace Package scope, culvert and hauling answers, a callback standard, the service radius, hours and any cost ranges.
- A Google Business Profile; a Facebook page fit to link.
- Font files (Graduate and Source Sans 3 load from Google Fonts) and an icon set chosen and recorded.
- Print colour references (Pantone, vinyl or paint). Only hex values and screen conversions exist.
- Verification of the parish culvert source and the NOAA rainfall normals before either is quoted.

## Sharing

**Nothing has been created for sharing yet, and the choice is Clint's.** Two options have been used for earlier clients:

1. **A separate kit-only repository**, proposed name `clintsanchez/wright-co-design-kit`, holding just this folder, so Claude Design can read it through "Create here". **It does not exist yet.** Whether it is public or private, and whether it is created at all, is Clint's decision; a public repository exposes everything in it while it is public.
2. **The whole client repository made public for the import**, as was done for one recent client, with Claude Design told to read `design-kit/` only, then set back to private once the import is done. This exposes the rest of the repository (research, records and working files) for that window.

Uploading the `design-kit` folder (or a ZIP of it) by hand avoids needing any repository to be public.

The folder holds public business details only (the name, the phone, the business email, the web address, the place line), the agency's draft proposals, the client's emblem and files derived from it. It holds no photographs, no street address and no account identifiers.

**The reference kit PDF is not in version control.** `assets/references/reference-kit-format_REFERENCE-ONLY.pdf` is another client's confidential brand kit, used only to show the structure, depth and format expected. It is excluded by `assets/references/.gitignore` and is uploaded to Claude Design by hand. Do not bundle it, the two generic templates or the section map into anything sent to the client.
