# 8. Asset Manifest and Production Rules

Wright Co. Version 0.1, 2026-10-15. Prepared by BlakSheep Creative. What exists, what does not, and the rules for adding to it.

**Status.** Nothing in this kit has been approved by the owner, Cody Wright. The assets below are what the agency holds. The emblem is the client's own artwork, received as a raster. There are no photographs of Wright Co. work. Every rule here is a BlakSheep Creative proposal until he signs it off.

**Built from.** The brand style guide (version 2.0), the visual identity brief, the brand context, the voice guide, the site architecture and `tokens/css-tokens.css`.

## 1. Asset manifest

All paths are relative to the kit folder, `design-kit/`. Use these folders. Add no asset that is not listed in a folder's own README or manifest.

### Logos (`assets/logos/`)

The emblem: distressed bone-white varsity lettering "WRIGHT CO" with rust bevels, over a soil-filled Louisiana silhouette with cattails and marsh grass. The client's original is a raster of about 1536 × 1024 on a black ground with an outer glow, with the phone number in a banner. It is the client's artwork. Who made it, and whether a vector or layered original exists, is `CONFIRM BEFORE PUBLISHING`.

| Folder or file | What it holds | Purpose |
|---|---|---|
| `assets/logos/README.md` | The logo set's own guide | One row per file: what it contains, permitted grounds, minimum sizes, provenance. **The authority on which file goes where** |
| `assets/logos/source/` | The client's original emblem files, as received | Reference and master only. Not placed in layouts directly |
| `assets/logos/emblem/` | The emblem prepared for layouts | Hero, cover, closing slide, footer, print. Dark grounds only, 240 px wide or larger |
| `assets/logos/avatar/` | The square profile picture prepared from the emblem | Every profile picture, the same on every platform |
| `assets/logos/favicon/` | Browser and touch icons | Browser tabs, bookmarks, the home-screen icon |

Read the README before placing any file. It says which versions exist (for example, whether a phone-free emblem is among them) and at what sizes.

### Photography (`assets/photos/`)

**Zero photographs.** No Wright Co. job in Louisiana has been photographed yet.

| File | What it holds | Purpose |
|---|---|---|
| `assets/photos/PHOTO-MANIFEST.md` | The photo manifest. Today it lists no files | When photos arrive, one row per photo: source, who took it, permission, town, scope, dimensions, cautions |

Every layout that needs a picture uses a labelled photo slot (section 3). Photographs from the owner's Washington business are never added to this folder.

### Tokens

| File | Type | Use |
|---|---|---|
| `tokens/css-tokens.css` | CSS custom properties | The values of record for every hex, font stack, type size, line height, space, radius and container width. A copy of the website's token file. Where any other file disagrees with it, the token file wins |

The token file does not yet hold: a lead size (1.25rem), the eyebrow size and tracking (0.875rem, +0.08em), the button size (1rem), button-specific tokens, or a focus-ring token. File 3 gives those values from the style guide.

### Icons

| File or library | Type | Use |
|---|---|---|
| None bundled. Phosphor (Fill) or Tabler (filled) is proposed | Open-license filled glyphs, square ends, mitred corners | One set across everything. Record the set and its license when it is chosen. The list of icons needed is in file 3, section 11 |

### Fonts

Not bundled. **Graduate** (one weight, 400) and **Source Sans 3** (400, 600, 700) load from Google Fonts under the SIL Open Font License. Load Graduate as `family=Graduate` only, and set `font-weight: 400` and `font-synthesis: none`. For print and vinyl vendors, send Graduate with the job. Office fallbacks: Rockwell Bold, then Arial Black, for headings; Arial for body.

### What does not exist

Do not build, draw, trace or generate any of these inside a layout. Where one is needed, use a labelled slot marked `CONFIRM BEFORE PUBLISHING` and say what it is waiting for.

| Does not exist | Until it does |
|---|---|
| Any photograph of a Wright Co. job | A labelled photo slot. Type-led layouts with the sequence and soil texture |
| The before/after series of one lot | A labelled before/after slot pair |
| A photograph of Cody Wright | A labelled photo slot. Captions name him only once a real photo exists and he approves it |
| A vector emblem (the commissioned redraw) | The supplied raster files at 240 px or larger, on dark |
| The emblem without the phone banner, if `assets/logos/README.md` does not list one | The banner version under the rule in section 2, or a labelled logo slot |
| The horizontal wordmark (logo #3) | A labelled logo slot in headers, email signatures and estimates. Never "WRIGHT CO" set in type |
| The mark only (logo #4: state silhouette, single "W") | The files in `assets/logos/avatar/` and `assets/logos/favicon/` |
| One-color versions (Bone, Soil Black, Rust), embroidery files | Nothing. No one-color piece is produced until they exist |
| Pantone, vinyl or paint references; CMYK-proofed values | Build in RGB from the tokens. Give a printer the hex and a press proof to match. The CMYK in file 3 is a screen conversion |
| Reviews, ratings or testimonials | Nothing. No review block, no review card |
| Prices or cost ranges | Nothing. See file 6 |
| Hours | Nothing |
| A confirmed service radius | The place line only |
| Any video footage | Stills and type-led motion only. No video is generated |
| A Google Business Profile | Nothing to link or badge |
| A Facebook page fit to link (it carries "LLC" and the wrong website today) | No Facebook link in any piece until it is renamed and repointed |

## 2. Logo rules for production

1. **Never redraw, trace, re-letter, re-vectorize, recolor, upscale, clean up or AI-generate the emblem, its lettering, its silhouette, its cattails, a wordmark, a mark, an avatar or a favicon.** Not to "clean it up", not to make a square or one-color version, not to remove the phone banner.
2. Composite the supplied files only, unmodified, from `assets/logos/emblem/`, `assets/logos/avatar/` and `assets/logos/favicon/`, as `assets/logos/README.md` directs. Do not place files from `assets/logos/source/` directly.
3. The emblem sits on Soil Black, Soil Surface or Soil Elevated, or on a photograph under a 60 percent or stronger Soil overlay. On Bone or white, only inside a square-cornered Soil Black container.
4. Minimum 240 px wide on screen and 2 in in print. Below that, a labelled slot for the wordmark or mark until they exist.
5. Clear space: one tenth of the emblem's width on every side.
6. **The phone number never lives inside the logo in new work.** Use a phone-free emblem where the README lists one. Where the only file for a placement carries the banner, it may be used at 240 px or larger on dark, provided the number in it is 360-957-5865; set the phone in type as well where the layout allows. Do not crop, mask or paint the banner out.
7. Never add "LLC", a tagline, a phone number, "Est. 20XX", a badge or a frame to the lockup.
8. "WRIGHT CO" is never set in Graduate or any typeface as a substitute for the logo file, and the emblem's distressing is never imitated on running type.
9. In a mock-up of a truck door, yard sign, shirt or hat, show the supplied file flat on a plain panel, labelled as a mock-up. Do not render it onto a generated truck, shirt or scene, and do not let an image model draw any lettering.
10. The tagline is never part of the logo artwork.

## 3. Image rules

1. **Real photographs only.** Anything that shows land, a lot, a driveway, a pad, a pond, a machine, a truck, a crew member, Cody or a customer uses a real photograph of a real Louisiana Wright Co. job from `assets/photos/`. None exists yet, so use a labelled photo slot.
2. **Show the ground, not the gear.** The lot and the result fill the frame. A machine is never the subject alone.
3. **Never use a photograph from the owner's Washington business,** captioned "past work" or not.
4. **One preset on everything:** warm and slightly desaturated, greens pulled down 15 to 20 percent, shadows lifted a touch, red clay and soil kept true. No other filter, no heavy HDR.
5. **No compositing, object removal, generative fill, sky replacement, expansion or upscaling.**
6. **Caption every job photo with the town and the work:** "Independence · 3 ac cleared · 300 ft drive · pad" (format example only). Never an invented number. Never a client's name without permission.
7. **Crop out house numbers, plates and faces** of anyone who hasn't given permission. Crop; do not blur.
8. **Never show another company's equipment or logo** as the subject.
9. **Text on a photograph only under a 60 to 75 percent Soil overlay.**
10. **The before/after series is shot from one fixed spot** (a stake or fence post), same framing every time.
11. **If a landowner asks for a photo to come down, it comes down the same day.**
12. Alt text says what is in the frame: "A cleared lot outside Independence with the driveway cut in and the house pad built." No keyword stuffing.

### Photo slot

A photo slot is a flat Soil Surface rectangle with a 1 px Clay hairline at 16 percent and an 8 px radius, a filled camera icon in Clay, and a label in Source Sans 3 that names the missing picture and what it takes to get it: "Before: wooded lot, from the fixed spot. `CONFIRM BEFORE PUBLISHING`: photograph needed from the first Louisiana job." On a Bone section: Bone Alt fill, Soil hairline at 10 percent, the icon in Soil Black. It is a kit component, clearly unfinished, and it never ships in a public piece. A public page with no photo is type-led instead.

Standard slots to use:

| Slot label | Where |
|---|---|
| "Before: wooded lot, from the fixed spot" / "After: pad built, same spot" | Hero (once real), before/after posts |
| "01 Clear: stumps coming out" | Land clearing page |
| "02 Driveway: driveway cut in, culvert at the road" | Driveway page |
| "03 Pad: finished pad with the builder's stakes" | House pad page |
| "Pond holding water" | Ponds page |
| "Cody walking a lot with a landowner (with permission)" | About page, Lot Walk page |

### The `CONFIRM BEFORE PUBLISHING` badge

A small label for any unfilled or unapproved slot: Source Sans 3 700 at 14 px, uppercase, 0.06em tracking, Warning `#E8A33D` text on Soil Elevated (7.49 to 1) with a 1 px Warning border and a 2 px radius. Warning text fails on Bone, so on a Bone section the badge sits on its own Soil Elevated chip. It is removed only when the item is confirmed.

## 4. AI image generation rules

**Generated images are not permitted for job imagery, people, places or logos.** That covers:

1. A lot, a field, woods, a driveway, a culvert, a house pad, a pond, a foundation dig or a cleared site, in any style: photographic, illustrated or cartoon.
2. A machine, truck, trailer or piece of equipment.
3. Cody, a crew member, a landowner, a builder or any person.
4. A house, a Hammond landmark, a parish scene or any recognizable place.
5. The emblem, the lettering, the silhouette, the cattails, or any text rendered on a generated object.
6. A mock-up of a truck, sign, shirt or hat.
7. An extension, outpaint, upscale, relight, clean-up or background swap of any supplied file.
8. A map with a pin on an address or a radius ring.

**The only permitted non-photographic graphics are abstract elements built from the tokens,** in code or as vector shapes: flat fields of a token color; the numbered sequence (strip, cards, list); rust rules; stitched-patch frames; chamfered shapes; the soil grain (noise at 6 percent opacity or less, dark sections only); topographic contour lines (Clay at 8 to 10 percent); an icon-based sequence diagram built from the chosen icon set; a simple static map of the parishes with no address pin. They carry no imagery of land, machines or people.

The reason is the brand's own position: it wins by showing real lots, not by claiming. A generated lot would be a fabricated job.

There is no approved prompt for a generated photograph, because none may be generated. Where a picture is missing, the answer is the shot list (file 3, section 12) and a labelled photo slot in the meantime.

## 5. Platform application rules

Sizes are working values. Verify each against the platform's current guidance at production time and record the date. Keep dimensions as editable values.

### Rules for every platform

- **One job, one photo, one next step,** once real photos exist. Until then, type-led cards: the sequence, The Dirt Order tips, straight answers.
- **Avatar:** the same file on every platform, from `assets/logos/avatar/`. Test it in a circle at 32, 64, 128 and 256 px and report honestly where it fails. When mark #4 is delivered, it replaces this.
- **Cover:** the emblem (no phone, where one exists) on Soil with soil grain. Later, the before/after of one real lot.
- **Logo in a graphic:** the emblem only where it can be 240 px or larger and still sit clear of the safe margins: covers, closing slides. Elsewhere, no logo on the graphic; the account name and avatar carry the brand. When the wordmark exists, it sits small at bottom right.
- **Safe margins:** 80 px on all sides of a 1080 px canvas. On 1080 × 1920, keep text out of the top 250 px and the bottom 340 px (Default).
- **Type:** Graduate for the headline, uppercase, two lines and eight words at most. Source Sans 3 for support lines. Smallest text 36 px. No more than two type sizes plus a label.
- **Grounds:** Soil Black, Soil Surface, Bone. One ground plus at most one panel color. No gradients, shadows or glows.
- **One thing in rust:** a rust rule, the before/after divider or a Copper numeral. Not all three.
- **Calls to action:** "Book a Free Lot Walk" and "Call or Text 360-957-5865", written in the caption, and where a graphic needs one, as a single line of text. No button drawn on an image.
- **Captions:** what + where + what's next + call to action. Zero to two emoji in a Facebook caption at most; none in a graphic.
- **Alt text** on every image post. Nothing essential (the phone number, a date) lives only in the image.
- **Banned in every template:** see section 6. In short: no "LLC"; no licensed, insured or bonded; no years in Hammond or "established"; no ratings or review counts; nothing from the Washington business; no street address; no prices; no competitor's phrasing; no pad heights; no stock or AI job imagery; no green.

### Platforms this client uses

| Platform | Account today | Sizes (working values) | Rules for this platform |
|---|---|---|---|
| **Facebook** | A page exists, titled with "LLC", linking to the wrong website, with a placeholder street address | Feed 1080 × 1350 and 1080 × 1080. Story and reel cover 1080 × 1920. Link preview 1200 × 630. Cover 1640 × 924, subject kept in the middle strip | The priority channel. The rename to "Wright Co. \| Hammond LA", the link to wrightco.llc and the removal of the address are `CONFIRM BEFORE PUBLISHING` (the owner's permission). Post templates: (a) before/after split with a 4 px Rust divider and a town caption bar (waits on photos); (b) "Step 01 / 02 / 03 / 04" cards; (c) plain-talk tip cards, Bone on Soil. Reply in the thread, then move to text. Pin a "Just closed on land? Book a free lot walk." post |
| **Google Business Profile** | None. To be created | Post 1200 × 900. Cover 1080 × 608. Logo square, from `assets/logos/avatar/` | A service-area business with no address. Services match the website pages. Posts are short: one job, one photo, the phone. No hashtags. Real job photos only. Ask every finished customer for a review, with no incentive |
| **Instagram** | No account on file | Feed 1080 × 1350 and 1080 × 1080. Story and reel 1080 × 1920. Carousel 1080 × 1350 | Build nothing beyond the shared masters until an account exists; label any frame "no account on file". If opened: step-card carousels, the last slide on Soil with the emblem and the phone |
| **YouTube** | No account on file | Thumbnail 1280 × 720. Banner 2560 × 1440, important content inside the center 1546 × 423 | The Dirt Order clips are planned ("Dirt Order #3: How high should my pad be?"). Real footage only; none exists. No generated or stock footage |

### Other applications

- **Website open graph images:** 1200 × 630. Soil ground, the emblem (no phone, where one exists) at 240 px or larger at left, the tagline or page title in Graduate at right. Everything inside a 40 px margin.
- **Blog graphics:** a real photograph at column width with a caption beneath, or the sequence graphic. No text on a photo without the Soil overlay.
- **Email:** header with the wordmark (a labelled slot until it exists) on Soil Black, body on Bone, Source Sans 3 or Arial. Signature: "Cody Wright · Wright Co. · 360-957-5865 · wrightco.llc", with the phone as a `tel:` link. No "LLC", no license line.
- **Estimates and invoices:** Bone page, wordmark top-left (slot until it exists), a Rust rule, numbered scope sections that mirror 01 to 04, a separate "On your side" block (911 address, culvert permit, survey), a "What can change it" block, Source Sans 3 throughout, a Rust totals line. The most serious register: no humor, no adjectives. The legal-name line is left blank.
- **Business cards:** Soil front with the emblem (no phone); Bone back with Cody Wright, the phone, the email, the domain and the place line in Source Sans 3, one Rust rule. Square corners, uncoated stock.
- **Presentations and one-sheets:** Soil title slide, Bone content slides. Graduate headings at 32 to 40 pt (Rockwell Bold in Office), Source Sans 3 body (Arial) at 18 pt minimum. One rust element per slide.
- **Yard and job-site sign (18 × 24 in coroplast):** Soil ground, the emblem (no phone) at top, a Graduate line ("LOT CLEARING IN PROGRESS" or "BUILD-READY LOTS"), the phone in 3 in Source Sans 3 700, the domain. Square corners. Placed only with the landowner's written permission.
- **Truck doors:** the emblem (no phone), full color on dark trucks; "WRIGHTCO.LLC · 360-957-5865" in Source Sans 3 700 beneath, then "Land Clearing · Driveways · House Pads". No "LLC" after the name, no license or insurance line, no DOT number that doesn't belong to the Louisiana operation. One-color versions wait on the logo system.
- **Tailgate:** the wordmark (once drawn) and the phone, letters 3 in or taller.
- **Apparel:** waits on the one-color mark and on the owner confirming the gear line. Never the logo on hi-vis yellow as the brand look.
- **Print collateral generally:** 0.125 in bleed and a 0.25 in safe margin as working values. Build in RGB from the tokens and mark every piece "Color to be matched from a press proof". Nothing is printed, and no vehicle is lettered, until the owner signs off; mark each piece "Not yet approved by the owner. Do not send to production until he signs off."

## 6. Quality control checklist

Run on every page, template, graphic, post and export. One "no" stops it.

**Provenance and status**

- [ ] Nothing describes the kit as approved by the owner. Derived items are marked as proposals.
- [ ] Every unconfirmed item carries a visible `CONFIRM BEFORE PUBLISHING` marker and is not filled with a guess.
- [ ] No invented brand element: no new logo, mark, monogram, mascot, illustration, pattern or color.
- [ ] No generic contractor-template styling. The piece looks like dark soil, rust and bone, heavy and square.

**Name, place and history**

- [ ] The name is "Wright Co.", with the period. No "LLC" anywhere, in any form ("wrightco.llc" as a URL is the only exception).
- [ ] No street address. The place line reads exactly "Serving Hammond, Tangipahoa Parish & the Northshore" (or "a Hammond-area crew").
- [ ] The only history claim is "clearing and excavating since 2022", with no place attached. No years in Hammond or Louisiana, no "established", no "Est.", no "decades".
- [ ] Nothing from Wright Excavation LLC: no testimonial, review, photo, logo, link, rating or mention.
- [ ] The owner is "Cody Wright" or "Cody". Never "founder". No story detail beyond file 6's approved list.

**Logo**

- [ ] The correct supplied file from `assets/logos/emblem/`, `avatar/` or `favicon/` is composited, unmodified, proportions preserved, as the README directs.
- [ ] The emblem is on Soil, on a photo under a 60 percent or stronger Soil overlay, or inside a square-cornered Soil container.
- [ ] At least 240 px wide (2 in in print), with clear space of one tenth its width.
- [ ] No redrawn, re-lettered, recolored, traced, upscaled or generated logo, wordmark, mark, avatar or favicon anywhere, mock-ups included. The phone banner has not been cropped or painted out.
- [ ] "WRIGHT CO" is not set in type as a stand-in for the logo. Missing logo versions are labelled slots.
- [ ] No "LLC", tagline, phone, "Est." or badge inside the lockup.

**Color and type**

- [ ] Only the token colors. Cattail Rust is `#A15C27`, Soil Black `#120C06`, Bone `#F9F7F4`.
- [ ] No green, safety yellow, blue or cool accent as a brand color. Status green appears only as a form success state.
- [ ] One thing in rust per screen. No gradients.
- [ ] No Copper text under 24 px on Bone. No white or Bone text on Copper. No Clay text on Bone. No Earth Brown text on Soil. No status-color text on Bone.
- [ ] Every text and background pair meets WCAG AA; every icon, field border and focus ring meets 3 to 1. Checked on the actual background.
- [ ] Display, H1, H2, eyebrows, numerals and badges are Graduate at weight 400 with `font-synthesis: none`, uppercase, eight words and two lines at most. Everything else is Source Sans 3. No third typeface, no Oswald.
- [ ] Spacing uses 8, 16, 32, 64, 96 or 128 px. Radius is 2, 4 or 8 px, or a chamfer. No pill shapes, no shadows, no glows.
- [ ] Every interactive element has a visible focus ring and is at least 44 × 44 px; buttons are 52 px tall.

**Buttons**

- [ ] The primary reads exactly "Book a Free Lot Walk": solid Cattail Rust, Bone label, 2 px radius.
- [ ] The secondary reads exactly "Call or Text 360-957-5865" (or "Call or Text" in a narrow header): outlined, a 2 px Copper ring on dark or Soil Black ring on Bone, linked `tel:+13609575865`. It is a button, not a bare link.
- [ ] The two are equal width, primary first, capped at 520 px for the pair.
- [ ] Any form actually submits.

**Images**

- [ ] Every photograph is a real Louisiana Wright Co. job from `assets/photos/`. Today that means none: every picture is a labelled photo slot, and no slot ships in a public piece.
- [ ] No stock photo. No AI-generated or illustrated lot, machine, crew, landowner, house or place.
- [ ] No Washington photo, captioned or not.
- [ ] Captions name the town and the work, with no invented number and no client name without permission.
- [ ] Only permitted abstract graphics (section 4): token fields, the sequence, rust rules, patches, chamfers, soil grain, contour lines.

**Claims**

- [ ] No licensed, insured, bonded, license number or credential.
- [ ] No star rating, review count, "5-star", "top-rated", review seal or counter. No review quote at all until a real, verified Louisiana review exists.
- [ ] No price, range, per-acre rate, "from", discount, "affordable" or comparison. Pricing reads "no prices; quotes via the Free Lot Walk or an estimate".
- [ ] No "#1", "premier", "best", "trusted", "quality" as a claim, "solutions", "full-service" or "no job too big or too small".
- [ ] No "standing pine", "slab", "every phase", "one contractor", "raw land to finished build", and no bare "start to finish".
- [ ] No competitor named or described.
- [ ] No pad height, elevation, flood promise, "permits handled", guaranteed date or "settles over winter".
- [ ] No promise still marked `CONFIRM BEFORE PUBLISHING` in file 6 (firm price, callback time, culvert install, hauling, what's in the package, the Lot Walk terms) appears without its marker.
- [ ] The Homeplace Package carries its descriptor. The Dirt Order carries its subtitle.
- [ ] At most one "Wright" pun in the whole system, and none until the owner confirms it.

**Copy**

- [ ] Copy matches the voice in file 4: plain, sequenced, straight, a little grit, no adjectives about ourselves.
- [ ] The sequence reads "01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig" exactly.
- [ ] Contact details are current: 360-957-5865 · wrightco504@gmail.com · wrightco.llc · "Serving Hammond, Tangipahoa Parish & the Northshore". No address, no hours.
- [ ] No emoji on the website, in graphics, headings or buttons. At most one exclamation mark, and none in a heading or button.
- [ ] No Cajun costume, no swagger, no false urgency.

**Platform**

- [ ] Mobile crop checked at 360 px. Social safe areas checked. Circular avatar crop checked.
- [ ] Smallest text in a 1080 px graphic is 36 px.
- [ ] One message per graphic. No more than two type sizes plus a label.
- [ ] Alt text written. Nothing essential lives only in the image.
- [ ] No link to the Facebook page until it is renamed and repointed.

**Privacy**

- [ ] Only public business details appear: the business phone, wrightco504@gmail.com, wrightco.llc and the place line. No home or street address, no other contact details for the owner, no account identifiers, no credentials, no agency notes, no record-check detail.

## 7. Maintenance

Review this kit:

- When the owner answers any open item. Remove the matching `CONFIRM BEFORE PUBLISHING` markers and no others, and update file 6 first.
- **When the commissioned logo system arrives** (phone-free emblem, transparent emblem, wordmark, mark, one-color versions, vector masters): add the files to `assets/logos/`, update its README and file 3 section 1, and replace every logo slot.
- When the first real Louisiana job is photographed: add each photo to `assets/photos/PHOTO-MANIFEST.md` with its town, scope, permission and cautions, and replace the matching photo slots. Start the before/after series from a fixed spot.
- When the Google Business Profile is verified and the first real reviews arrive: add the approved-quote rules to file 5, and only then any review card or rating line, dated.
- When the Facebook page is renamed and repointed: allow links to it.
- When the owner confirms the Free Lot Walk terms, the Homeplace Package scope, the culvert and hauling questions, the callback standard or the radius: update files 5 and 6, then this checklist.
- When the owner approves cost ranges: file 6 changes first. Until then, nothing.
- When the registration, licensing and insurance questions are resolved: a credential may be added as a secondary trust layer under the build-ready promise, never as the pitch. Not before.
- When a local Louisiana phone number is added: every piece, the emblem banner question and all listings change together.
- When `website/css-tokens.css` changes: replace `tokens/css-tokens.css` and re-check every value quoted in file 3.
- When a landowner asks for a photo to come down: remove it the same day and delete its rows here and in the photo manifest.
- After any change of services, ownership or name.
- At least once a year.

### Change log

| Date | Change | Author |
|---|---|---|
| 2026-10-15 | Version 0.1. Initial input kit, built from the brand package, the style guide version 2.0, the site architecture and the offer plan. Not approved by the owner | BlakSheep Creative |
