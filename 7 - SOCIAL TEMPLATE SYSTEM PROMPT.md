# Claude Design Prompt: Wright Co. Social and Digital Content Template System

Version 0.1 · 2026-10-15 · Prepared by BlakSheep Creative

You are acting as a senior brand designer, design systems architect, social media designer, information designer, accessibility specialist and production copywriter.

Extend the master brand design kit already built in this project into a complete, reusable, editable social and digital content template system for **Wright Co.**, a land clearing and home-site prep crew serving Hammond, Tangipahoa Parish and the Northshore in Louisiana. Build a system: tokens, components, variants, named layers, safe zones and recomposition between sizes. Do not produce a set of one-off sample posts.

Do not pause for general discovery. Produce the complete first version. Where a fact is unknown or waits on the owner, place a visible, editable field labelled exactly `CONFIRM BEFORE PUBLISHING` and say what is needed. Never invent a fact, a figure, a review, a customer, a job, a town, a date or a photograph.

**Run this second.** The master brand design kit (`1 - MASTER PROMPT.md`) must already exist in this project. This system inherits its tokens and components and adds nothing to the brand.

**Read first:** `0 - READ ME FIRST.md`, files `2` to `6`, `8 - Asset Manifest and Production Rules.md`, `assets/logos/README.md`, `assets/photos/PHOTO-MANIFEST.md`, `tokens/css-tokens.css`. This prompt is self-contained if any of those is missing. Where this prompt and `assets/logos/README.md` disagree about a logo file, the README wins. The claims lists at the end of `6 - Brand Context and Prices.md` override everything.

**Format to match:** the social, video and data content section of the reference kit format, `assets/references/reference-kit-format_REFERENCE-ONLY.pdf`, if it has been attached. It is another client's finished kit, used for structure and depth only. Take nothing else from it: no colour, typeface, wording, photograph, motif, figure or fact. The two Markdown files ending `_REFERENCE-ONLY.md` are generic agency templates; this prompt already accounts for every section of the universal social template (the agency's record of how is `assets/references/social-prompt-universal-section-map.md`, which is not an instruction).

## Status and provenance

**Nothing here has been reviewed or approved by the owner, Cody Wright.** The position, the voice, the colour roles, the typefaces and every line of sample copy are BlakSheep Creative drafts. The tagline "You bought the land. We'll get it ready to build." and the three offer names (The Homeplace Package, The Free Lot Walk, The Dirt Order) are BlakSheep Creative decisions, usable now, with his approval pending. Label the finished library on its cover and in its documentation footer: "Draft by BlakSheep Creative, version 0.1, 2026-10-15. Not reviewed or approved by the owner." Do not describe the output as the client's approved templates.

Settled facts that are not drafts: the name "Wright Co."; the phone 360-957-5865; the business email wrightco504@gmail.com; the web address wrightco.llc; the place line "Serving Hammond, Tangipahoa Parish & the Northshore"; the history line "Clearing and excavating since 2022"; free estimates; the colours sampled from the emblem; and the emblem itself, the client's own raster art.

**Where the library starts from.** There are **zero photographs** of Wright Co. work. There are no reviews, no rating and no prices. The Facebook page exists but still shows "LLC" in its name, links to the wrong website and shows a placeholder address, so no post links to it and no template shows it (W-05). There is no Google Business Profile yet and no Instagram or YouTube account. This library is built so that type-led posts can go out now, and so that every photo post is ready the day the first real Louisiana job is photographed, without any of it being untrue to look finished.

---

# 1. Dependency and token flow

Every value in this system comes from the master kit. State this flow on the first plate of the output:

```
MASTER BRAND KIT        tokens/css-tokens.css   (--brand-*, --bg-*, --text-*, --border-*, --success, --warning, --error, --font-*, --text-*, --leading-*, --space-*, --radius-*, --container)
        ↓               tokens/components.css   (button, focus, rule, icon, slot and confirm-badge aliases, from the master run)
        ↓
SOCIAL CONTENT SYSTEM   tokens/social.css       (formats, safe zones, social type scale, data palette; aliases only)
        ↓
CONTENT FAMILY          step card, plain-talk tip, Free Lot Walk, seasonal, now booking and service area, Dirt Order teaser, statement, straight answer, before/after slot, job photo slot, operations notice
        ↓
PLATFORM FORMAT         one canvas component driven by the Platform Specifications table
        ↓
FINAL ASSET             a composed, editable template
```

Rules for the token layer:

1. `tokens/social.css` introduces no raw colour and no font. Every social token is an alias of a master token or a size for a named canvas. Examples: `--social-ground-dark: var(--bg-base)`, `--social-ground-surface: var(--bg-surface)`, `--social-panel: var(--bg-elevated)`, `--social-ground-light: var(--bg-light)`, `--social-headline-color: var(--text-primary)`, `--social-numeral: var(--brand-primary-bright)`, `--social-rule: var(--brand-primary)`, `--data-1: var(--text-primary)`.
2. Master tokens in use, by their real names: `--brand-primary` (Cattail Rust `#A15C27`), `--brand-primary-bright` (Copper `#C8783A`), `--brand-secondary` (Earth Brown `#6F482A`), `--brand-accent` (Clay `#D4B8A0`), `--bg-base` (Soil Black `#120C06`), `--bg-surface` (`#20150C`), `--bg-elevated` (`#2E1D10`), `--bg-light` (Bone `#F9F7F4`), `--bg-light-alt` (Bone Alt `#ECE1D8`), `--text-primary` (Bone), `--text-muted` (Dust `#BFA89B`), `--text-on-light` (Soil Black), `--text-muted-on-light` (Dust Dark `#5C5048`), `--border-subtle`, `--border-subtle-light`, `--success` (`#22A06B`), `--warning` (`#E8A33D`), `--error` (`#D9534F`), `--font-display` (Graduate), `--font-display-weight` (400), `--font-body` (Source Sans 3), `--space-1` to `--space-6` (8, 16, 32, 64, 96, 128 px), `--radius-sm`, `--radius-md`, `--radius-lg` (2, 4, 8 px).
3. Canvas sizes and safe zones live in one place, the Platform Specifications table (section 7), and reach templates as `--format-<name>-w`, `--format-<name>-h` and `--safe-*` tokens. No template holds a typed-in dimension.
4. A change to `tokens/css-tokens.css` must flow through every template. Do not paste a hex value into a component.
5. Do not redesign the brand. No new colour, font, logo treatment, gradient, pattern, texture, illustration style, icon style or photographic style. **Brand adaptation, resolved:** this brand is dark-first, bold, heavy and square, industrial and local, a service business with no photographs yet. The architecture stays universal; the expression is soil, rust and bone.

---

# 2. Brand facts to inherit

| | |
|---|---|
| Name | **Wright Co.**, with the period, in all running text. The emblem artwork reads "WRIGHT CO"; the artwork is not changed. Never "LLC" in any form, never "WrightCo" |
| What it is | A land clearing and home-site prep crew. Category line: "Land clearing, driveways and house pads" |
| The sequence | **01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig**. Displayed "01 CLEAR · 02 DRIVEWAY · 03 PAD · 04 FOUNDATION DIG". Same words, same order, every time. Add-ons (ponds and drainage) never join it |
| Offers | **The Homeplace Package**, always with "Clear · Driveway · House Pad. One crew, one scope, build-ready." **The Free Lot Walk**, the button "Book a Free Lot Walk". **The Dirt Order**, always with "Building on Raw Land in Tangipahoa, Step by Step." |
| Owner | Cody Wright. "Cody" in social. Never "founder". His first-person voice on Facebook is `CONFIRM BEFORE PUBLISHING` (W-19); until then posts speak as "we" and sign off "Call or text Cody" |
| Phone | 360-957-5865, linked `tel:+13609575865`, always in this form |
| Email | wrightco504@gmail.com (expanded footer only) |
| Website | wrightco.llc |
| Place line | "Serving Hammond, Tangipahoa Parish & the Northshore". Hammond and Ponchatoula may be named. Every other town waits on the radius (W-07), except in a caption for a real job there |
| Address, hours | None. Never on a graphic |
| History | "Clearing and excavating since 2022", no place attached |
| Prices | None. Cost questions are answered with what drives the price |
| Reviews, rating | None. Nothing quoted, counted or starred |
| Photographs | None. Every photo position is a labelled slot |
| Tagline | "You bought the land. We'll get it ready to build." Short form "Ready to build." Alternate "From the first tree to the house pad." Builder-only "One crew. Woods to build-ready." |
| Voice | The neighbor with the equipment who walks your land with you: plain-spoken, straight about the hard parts, quietly sure he can get it ready to build. Short sentences, the order of the work, no adjectives about ourselves, a little dry grit on Facebook |

**Platforms on record (2026-10-15).** Facebook: a page exists, not fit to link until renamed and repointed (W-05). Google Business Profile: none, to be created as a service-area business with no address. Instagram, YouTube: no account on file. Every handle field in the footer component is empty and switched off by default; the web address is the default.

---

# 3. Four rules above all others

Present these as four rule cards at the head of the output, as the reference kit format does.

**Recompose, never resize.** One message is rebuilt for each ratio. A 4:5 step card stacks the giant numeral over the step name over the line; the 4:3 Google post sets the numeral beside them; the 9:16 story sets them between the safe-zone bands. A portrait card cut down to a landscape shape does not count as a landscape template.

**Real or a labelled slot.** No photograph exists. Every photo position is a `PhotoSlot` whose label begins "Real job photo:" and names the shot. No stock, no AI-generated scene, no illustrated lot, no equipment render, no blurred placeholder, ever. A post that would need a photo either waits for one or runs type-led.

**Every number carries a source and a date, and almost none may appear.** No price, acreage, lot count, job count, years figure, rating, review count, pad height or duration appears in a publishable template. The only figures allowed are the step numerals 01 to 04, the year in "since 2022", the phone number, and parish process facts with their source linked and dated. Every other figure in a specimen is flagged as sample data.

**One thing in rust, on soil.** Soil Black or Soil Surface carries the canvas; Bone is for long reading; Cattail Rust or Copper marks one thing. Every post names only what Wright Co. does, makes no promise the owner has not confirmed, and says nothing about any other company.

---

# 4. Claims: what may never appear

This section is part of the components, not a note beside them. A social post is an advertisement published under the business's name. The full register is section 11 of the master brief and the prohibited list in file 6; it binds every caption, alt text, hashtag and graphic.

## 4.1 The prohibited-claims register, for social

| Never | Use instead |
|---|---|
| "LLC" in any form; "WrightCo"; "Wright Company" | "Wright Co." |
| Licensed, insured, bonded, any licence number, credential, certification or a badge implying one | Nothing |
| Years in Hammond or Louisiana, "local since", "established", "Est. 2022", "founded", "decades of experience" | "Clearing and excavating since 2022" |
| Star ratings, review counts, "5-star", "top-rated", review seals, any review quote | Nothing, until real Louisiana reviews exist |
| Anything from the owner's separate business in another state: photos, reviews, jobs, logo, link | Nothing |
| Any price, range, per-acre rate, "from", discount, promo code, "winter pricing", "affordable", "no hidden fees", "save", "deal" | "Here's what moves the price." |
| "#1", "premier", "best", "trusted", "top-rated", "quality" as a claim, "solutions", "full-service", "no job too big or too small" | A specific fact |
| "Standing pine", "slab", "every phase", "one contractor", "raw land to finished build", a bare "start to finish" | "build-ready", "house pad", "one crew" |
| Any competitor named or described; "unlike", "the other guys", "most contractors" | Say what Wright Co. does |
| Pad heights, elevations, "high and dry", flood promises; "we handle your permits" | "Your surveyor and the parish set the height. We build to it." · "The application is yours to file." |
| "Guaranteed", "pad ready by spring", **"your pad settles over winter"**, "settled by spring", "rain or shine" | "If rain moves it, we'll tell you." |
| "Same-day", a callback time, "firm price", "no surprises", "texts welcome" | "Straight answers, in plain words. Call or text Cody." |
| A street address, "based in Hammond", a map pin, a radius ring | The place line |
| Countdowns, "limited time", "only 2 spots left", "book before prices go up" | Real facts only |
| Concrete, fencing, decking, tree care, commercial or subdivision work | "We stop where your builder starts." |
| Stock photos, AI-generated or illustrated lots, machines, crews, people, houses or places; equipment renders; mock-ups on generated trucks or shirts | A labelled `PhotoSlot` or a type-led card |
| A redrawn, retyped or generated logo; "WRIGHT CO" set in Graduate as a logo | The supplied emblem file |
| Cajun or bayou costume; "Louisiana born and raised" | Plain words. The emblem carries Louisiana |
| More than one "Wright" pun; any before the owner confirms "the Wright way" (W-21) | Nothing |
| A link to the Facebook page in any piece (W-05) | Nothing |

## 4.2 What the company's current channels say, and what changes

The live website and Facebook page carry wording that is retired. None of it is reused, in any form, and the templates are built so each is hard to repeat:

- "Built on Hard Work. Driven by Quality." as a headline.
- "Work Done the Wright Way" as a heading.
- "We cover all your excavation needs!" and the asterisk list of services on Facebook, including services not confirmed for Louisiana (W-16).
- "Proudly based in Hammond, Louisiana" and the placeholder street address on the Facebook page.
- "Excavation & Trucking" as a title; "Trucking" as a category.
- "Wright Co. LLC" as the page name.
- Photos and reviews whose state and customer are unknown (W-22). None is used until confirmed as Louisiana work with permission.

## 4.3 The three-part test for every post

Before a template is marked complete, its sample copy passes all three:

1. It makes no claim outside file 6's approved list, and no promise the owner has not confirmed. If it does, the promise sits in a `CONFIRM BEFORE PUBLISHING` field.
2. It shows no photograph that is not a real Louisiana Wright Co. job; today that means it shows none.
3. It says nothing about any other company.

---

# 5. Visual layer

**The idea.** The canvas should look like the ground itself and like a local crew's truck door: dark soil, rust and bone, heavy collegiate lettering, square edges. With eyes half shut, a post reads as dark earth, one bone headline and one rust or copper mark. Once real photos exist, a real photograph with a plain caption beats a designed card; until then, the sequence and plain talk carry the feed.

## 5.1 Logo and mark

The only logo is the supplied emblem: a detailed raster illustration with the phone number baked into its banner. Composite the supplied files; never redraw, trace, re-letter, retype, recolour, outline, crop into, sharpen, upscale or AI-generate any part of it. Paths are relative to `assets/logos/`.

| Use | File | Rule |
|---|---|---|
| Emblem on a dark canvas | `emblem/wright-co-emblem-transparent-1200w.png` (or `-native-1263w.png`) | Soil Black, Soil Surface or Soil Elevated only. At least 240 px wide; on a 1080 px canvas use 480 px or more, because feeds are seen at about a third of size. Clear space one tenth of its width |
| Emblem on a light canvas | `emblem/wright-co-emblem-on-soil-square-1200.png` inside a square-cornered Soil Black container | Never the transparent file directly on Bone or white: its shadow reads as a grey smudge |
| Link preview and cover base | `emblem/wright-co-emblem-on-soil-landscape-1200x628.png` (and `-2400x1257.png`) | Used whole |
| Avatar | `avatar/wright-co-avatar-emblem-on-soil-1024.png` (master), `-512`, `-400`, `-320`, `-180` | Section 12.1 |
| Favicon | `favicon/` | Interim. Never on a social canvas |
| Not for use | `source/` (both files); `emblem/wright-co-emblem-transparent-2400w-upscaled.png` for anything but a layout that demands 2400 px | |

**Because the emblem needs 480 px on a 1080 px canvas, it appears only on covers, the opening and closing slides of carousels, end cards and the Free Lot Walk card.** Step, tip and statement cards carry no logo: the page name and avatar sit beside every post, and the footer carries "wrightco.llc". **The emblem appears once per canvas, never twice, and never with a second mark.** No corner mark exists (the drawn small mark is logo #4, not yet made); do not build one from the emblem or the favicon crop. Where a small mark would go, leave it out.

**Missing logo versions** (no-phone emblem, flat wordmark, small mark, one-colour versions, vector master) are labelled `LogoSlot`s in the library documentation only; no publishable template depends on them.

## 5.2 Colour on a social canvas

- **Grounds:** Soil Black (default), Soil Surface, and Bone for reading-heavy cards. Soil Elevated is a panel inside a canvas, never a full ground. One ground plus at most one panel colour per canvas.
- Headlines: Bone on dark; Soil Black on Bone. Body: Bone or Dust on dark; Soil Black on Bone. Captions and sources: Dust on dark (8.59 to 1); Dust Dark on Bone (7.28 to 1).
- Copper: giant numerals, eyebrows and labels on dark (5.74 to 1). On Bone, Copper only as a numeral of 24 px or larger (3.17 to 1); never body text.
- Cattail Rust: the 4 px rule or the before/after divider. **No button is drawn on an image**, so Rust is never a button fill on social.
- Feed graphics are read at about a third of their pixel size: body text pairs reach 7 to 1 (Bone, Dust and Clay on the Soil grounds all do; Soil Black and Dust Dark on Bone do).
- Never: Earth Brown text on Soil (2.44), Clay on Bone (1.76), Bone on Copper (3.39), Warning text on Bone (2.02). No gradients, shadows, glows, duotones or photo tints other than the Soil overlay at 60 to 75 percent. No green, yellow or blue.

## 5.3 Social type scale

**Graduate, weight 400 only, with `font-synthesis: none`, uppercase,** for headlines, numerals and labels. **Source Sans 3** at 400, 600 and 700 for support lines, body, sources and footers. No third family. Source text in sentence case; CSS uppercases Graduate. "WRIGHT CO" is never set in Graduate as a logo.

Working sizes on a 1080 px wide canvas. Publish them as tokens (`social.square.headline`, `social.portrait.headline`, `social.story.headline`, `social.landscape.headline`, `social.banner.headline`, `social.thumbnail.headline` and so on) and derive other canvases by proportion.

| Token | Size | Face | Role |
|---|---|---|---|
| `--social-numeral` | 200 to 240 px | Graduate 400, Copper | The step numeral, "01" to "04" |
| `--social-display` | 96 px | Graduate 400 | One short line on a statement card |
| `--social-headline` | 72 to 88 px | Graduate 400 | Headline, eight words and two lines at most, line height 1.1 |
| `--social-headline-story` | 88 px | Graduate 400 | Story and reel cover headline |
| `--social-headline-thumb` | 104 px on 1280 x 720 | Graduate 400 | Thumbnail headline, five words at most |
| `--social-subhead` | 40 to 44 px | Source Sans 3 400 | One support sentence, line height 1.4 |
| `--social-body` | 36 px | Source Sans 3 400 | Smallest running text allowed |
| `--social-label` | 28 to 30 px | Graduate 400, +0.08em | Eyebrow, series label, step strip. The only style below 36 px with the source |
| `--social-source` | 30 px | Source Sans 3 400 | Citation and date line; footer |
| `--social-cta-line` | 36 px | Source Sans 3 700 | "Book a Free Lot Walk · Call or Text 360-957-5865" as one line of text |

No more than two type sizes plus a label on one canvas. No exclamation mark in a headline. No emoji in artwork. No italics.

## 5.4 Spacing and grid

Use the master scale and nothing between: 8, 16, 32, 64, 96, 128 px. Canvas padding `--social-pad` is 80 px on feed canvases (64 + 16), 64 px on landscape canvases 720 px tall or less and on banners. Stack gaps are 32 and 16 px. Document a grid for square, portrait, landscape, story, banner, thumbnail and infographic: margin, columns (4 for portrait and story, 6 for square, 12 for landscape and banners), gutter 16 px, an 8 px baseline, and left alignment. Nothing is rotated or overlapped; nothing is centred except a single short line on a closing slide. Radius: 4 px on panels, 8 px on photo slots and framed photos, square on anything edge to edge and on the emblem's Soil container. Chamfered corners (8 to 12 px, 45°) on stitched badges and step panels. No pills.

## 5.5 Grounds and decoration

**Grounds (five):** `soil` (Soil Black, with soil grain at 6 percent or less), `surface` (Soil Surface, with grain), `bone` (Bone, no grain), `photo` (a real photograph under a 60 to 75 percent Soil overlay where type sits on it; today only a `PhotoSlot`), `split` (a hard horizontal stop: a photo slot above, Soil or Bone below; never a gradient).

**Decoration (three gestures):**

| Gesture | What it is | Limits |
|---|---|---|
| `GiantNumeral` | A step numeral in Copper Graduate at 200 to 240 px, top left | Only on step cards and the sequence carousel. Never a number that is not a step |
| `RustRule` | A 4 px Cattail Rust rule under the headline, or as the before/after divider | Straight, one weight, one per canvas |
| `ContourLines` | Topographic contour lines in Clay at 8 to 10 percent opacity, cropped by the canvas edge | Abstract lines, not a map of a real place. Dark grounds only. Never behind body text at higher opacity |

**One gesture per canvas.** A numeral or a rule or contour lines, never two. Soil grain is a ground texture, not a gesture. The stitched-patch badge is a label component (offer names, "DIRT ORDER #3"), not a gesture. Show this as a callout, with six composed canvases that put each gesture to work.

## 5.6 Optional brand elements

Build component slots only for what exists.

| Exists: build a slot or component | Does not exist: do not manufacture |
|---|---|
| The supplied emblem, with its state silhouette, cattails and marsh grass, inside the art | A mascot, character, gator, crawfish or Cajun motif |
| The numbered sequence | An illustration style; drawn lots, machines or crews |
| The stitched-patch badge and the chamfer | A small mark, monogram or "WC" |
| Soil grain and contour lines | Patterns, other textures, gradients |
| Real job photographs, machines and crew, **once they exist** (photo slots today) | Equipment renders, vehicle mock-ups, uniform mock-ups |
| Cody as the named person in copy | A founder-as-brand photo system: no photograph of Cody exists (slot only, with permission) |
| A filled icon set (Phosphor Fill or Tabler filled, one set) | A second icon style; outline or duotone icons |

---

# 6. Photography and image containers

**Zero photographs.** `assets/photos/PHOTO-MANIFEST.md` lists none and the folder holds no images. Photographs from the owner's other business are never used. Facebook photos are not used until each is confirmed as Louisiana work with permission (W-22).

**The `PhotoSlot` component** (inherited from the master kit): a flat Soil Surface rectangle (Soil Elevated on a Surface canvas; Bone Alt on Bone) at the final crop ratio, 8 px radius (square when full bleed), a 1 px Clay hairline at 16 percent, a filled camera icon in Clay, and a label in Source Sans 3 at 36 px that **always begins "Real job photo:"**, names the shot, gives the ratio, then the `CONFIRM BEFORE PUBLISHING` badge and "Photograph needed from the first Louisiana job." It is visibly unfinished and **never ships in a published post.**

**Standard social slots:**

| Slot label | Ratio | Family |
|---|---|---|
| "Real job photo: before, wooded lot, from the fixed spot" | 4:5, 1:1, 16:9 | Before/after |
| "Real job photo: after, pad built, same spot" | 4:5, 1:1, 16:9 | Before/after |
| "Real job photo: 01 Clear, stumps coming out" | 4:5 | Step 01 photo variant, job photo |
| "Real job photo: 02 Driveway, driveway cut in, culvert at the road" | 4:5 | Step 02 photo variant |
| "Real job photo: 03 Pad, finished pad with the builder's stakes" | 4:5 | Step 03 photo variant |
| "Real job photo: Cody walking a lot with a landowner (with permission)" | 4:5 | Free Lot Walk photo variant |
| "Real job photo: the lot, wide, after clearing, from the road" | 16:9 | Covers, thumbnails |
| "Real job vertical video: brush going down, 10 to 30 seconds" | 9:16 | Reel cover |

**Treatment rules for when photos arrive:** real Louisiana Wright Co. jobs only, logged in the manifest; show the ground, not the gear (a machine is never the subject alone; another company's equipment or lettering is cropped out); one grade on everything (warm, slightly desaturated, greens down 15 to 20 percent, shadows lifted a touch, red clay true); crop and straighten only, no compositing, object removal, generative fill, expansion or upscaling; caption every job photo with the town and the work, never an invented number or a client's name without permission; faces, house numbers and plates cropped out unless cleared; text on a photo only under a 60 to 75 percent Soil overlay; the before/after series from one fixed spot; a photo comes down the same day a landowner asks.

**Image containers.** Build one component with variants: `full-bleed`, `framed` (8 px radius), `split`, `before-after` (two equal frames, 4 px Rust divider, caption bar), `service` (a job photo with a caption bar naming the town and the work). Every variant holds a `PhotoSlot` today and a real photo later; every variant has an alt-text field. **Not built:** rounded image (no rounded shapes), cutout subject (nothing to cut out, and a cutout of a machine reads as a render), background image behind text without the overlay, screenshot, browser frame, device frame, product image, portrait (no photograph of Cody exists; a portrait slot exists only as the Lot Walk slot above).

---

# 7. Master formats and the Platform Specifications table

## 7.1 Master format families

Show these as ratio tiles and as a table.

| Family | Size | Ratio | Used here by |
|---|---|---|---|
| Portrait feed | 1080 x 1350 | 4:5 | Facebook first; Instagram once an account exists; carousels |
| Square | 1080 x 1080 | 1:1 | Facebook, Instagram, avatars |
| Google post | 1200 x 900 | 4:3 | Google Business Profile updates, once the profile exists |
| Full-screen portrait | 1080 x 1920 | 9:16 | Stories, reel covers |
| Social landscape | 1200 x 630 | 1.91:1 | Link previews, open graph |
| Video thumbnail | 1280 x 720 | 16:9 | YouTube, once an account exists |
| Standard widescreen | 1920 x 1080 | 16:9 | Video end card, slides |
| Wide banner | 1500 x 500 | 3:1 | Architecture only: no platform in use |
| Tall content | 1000 x 1500 | 2:3 | Architecture only: no platform in use |
| Ultra-wide header | 1584 x 396 | 4:1 | Architecture only: no platform in use |

## 7.2 Platforms in priority order

1. **Facebook.** The priority channel. Design every family for it first, at 1080 x 1350. Posts go out from the existing page; the page is not linked from any piece until it is renamed and repointed (W-05).
2. **Google Business Profile.** To be created as a service-area business with no address. Build the 1200 x 900 post, the cover and the logo image now, and test every post at small card size. Status "to be created".
3. **Instagram.** No account on file. Instagram uses the shared 1080 x 1350, 1080 x 1080 and 1080 x 1920 masters only; label any Instagram-specific frame "no account on file". Build nothing else for it.
4. **YouTube.** No account on file. The Dirt Order clips are planned. Build the thumbnail, banner and end card masters only, labelled "no account on file".
5. **Not in use:** LinkedIn, X, TikTok, Pinterest, Threads, Bluesky, Snapchat, Reddit, Mastodon. Keep their rows in the table so the architecture is complete. Build no specimen for them.

## 7.3 The central table

Keep one `Platform Specifications` page. Every row has: platform, asset, width, height, ratio, safe zone, crop behaviour, status (in use, to be created, no account on file, not in use), notes, date checked. These are working values dated 2026-10-15; verify each against current platform guidance at production and re-date the row.

| Platform | Asset | Size | Ratio | Safe zone | Crop behaviour | Status |
|---|---|---|---|---|---|---|
| Facebook | Feed portrait / square | 1080 x 1350 / 1080 x 1080 | 4:5 / 1:1 | 80 px margin | Grid crops toward 1:1; keep the subject centred | In use |
| Facebook | Feed landscape | 1200 x 630 | 1.91:1 | 60 px margin | None | In use, rarely |
| Facebook | Story / reel cover | 1080 x 1920 | 9:16 | Clear of top 250 px and bottom 340 px | Platform chrome covers both | In use |
| Facebook | Page cover | 1640 x 924 | 16:9 | Middle 1640 x 624 | Phones show all of it; desktop crops to the middle strip (displayed near 851 x 315). The universal template lists 851 x 315; the larger master is used and this row flagged | In use |
| Facebook | Link preview | 1200 x 630 | 1.91:1 | 60 px margin | None | In use; no link to the page itself |
| Facebook | Profile image | 1024 master, 320 shown | 1:1 | Central 70 percent | Circular crop | In use |
| Facebook | Group cover, event cover | 1640 x 856 / 1920 x 1005 | | Centre | | Not in use; no groups or events on record |
| Google Business Profile | Update post | 1200 x 900 | 4:3 | 60 px margin | Shown small; type must survive a small card | To be created |
| Google Business Profile | Cover image | 1080 x 608 | 16:9 | Centre | A real photo, or the landscape emblem file, no extra text | To be created |
| Google Business Profile | Logo | 512 x 512 supplied | 1:1 | Central 70 percent | Square and circular crops | To be created |
| Google Business Profile | Square / landscape graphic | 1080 x 1080 / 1200 x 900 | | 60 px margin | | To be created |
| Instagram | Feed portrait / square / landscape | 1080 x 1350 / 1080 x 1080 / 1080 x 566 | 4:5 / 1:1 / 1.91:1 | 80 px margin | Grid preview crops; keep the subject centred | No account on file |
| Instagram | Story / reel cover | 1080 x 1920 | 9:16 | Clear of top 250 px and bottom 340 px | Grid shows the centre of a reel cover | No account on file |
| Instagram | Carousel | 1080 x 1350 | 4:5 | 80 px margin | All slides share one ratio | No account on file |
| Instagram | Profile image | 1024 master (320 x 320 shown) | 1:1 | Central 70 percent | Circular crop | No account on file |
| YouTube | Video thumbnail | 1280 x 720 | 16:9 | 60 px margin; lower right clear | Duration badge sits lower right | No account on file |
| YouTube | Channel banner | 2560 x 1440 | 16:9 | Centre 1546 x 423 | Only the centre shows on phones | No account on file |
| YouTube | Profile image | 800 x 800 | 1:1 | Central 70 percent | Circular crop | No account on file |
| YouTube | Community square / portrait / landscape | Shared masters | | 80 px margin | | No account on file |
| YouTube | Podcast playlist thumbnail | 1280 x 1280 | 1:1 | | | Not in use |
| YouTube | Video end card | 1920 x 1080 | 16:9 | 80 px margin | | No account on file |
| LinkedIn | Landscape / square / portrait / carousel / link preview | 1200 x 627 / 1200 x 1200 / 720 x 900 / 1080 x 1080 / 1200 x 627 | various | 60 px margin | None | Not in use |
| LinkedIn | Personal banner / company cover / logo | 1584 x 396 / 1128 x 191 / 400 x 400 | 4:1 / 5.9:1 / 1:1 | Centre / central 70 percent | Very shallow | Not in use |
| X | Landscape / portrait / square / header / profile | 1280 x 720 / 720 x 1280 / 1080 x 1080 / 1500 x 500 / 400 x 400 | various | Centre 640 px on the header | Avatar overlaps the header's lower left | Not in use |
| TikTok | Vertical post, cover, story / landscape ad / square ad / profile | 1080 x 1920 / 1920 x 1080 / 1080 x 1080 / 200 x 200 | various | Centre 1080 x 1420 | Caption and controls cover the bottom | Not in use |
| Pinterest | Standard / square pin / landscape cover / profile | 1000 x 1500 / 1000 x 1000 / 800 x 450 / 280 x 280 | various | 60 px margin | Taller pins are cut in feed | Not in use |
| Snapchat | Story, ad / profile / banner | 1080 x 1920 | 9:16 | Centre 1080 x 1420 | Chrome covers top and bottom | Not in use |
| Threads, Bluesky, Mastodon, Reddit | Square, portrait, landscape, link preview, profile | Shared masters | various | 60 px margin | None | Not in use |
| Bluesky, Mastodon | Banner / header | 1500 x 500 | 3:1 | Centre 640 px | Responsive height | Not in use |
| Reddit | Community banner / icon | 1920 x 384 / 256 x 256 | 5:1 / 1:1 | Centre 900 px / central 70 percent | Crops hard on phones | Not in use |

Add an "Adding a platform" callout: (1) add the canvas to the format list; (2) add its `--format-<name>-w` and `-h` tokens; (3) add a row to this table with its safe zone and crop behaviour; (4) map the existing content families into the new ratio by recomposing. Supporting a new platform means new rows and tokens, with no existing template edited.

---

# 8. Components

Build each once, with variants instead of duplicates. Names carry no client name.

- `Canvas` (format, ground, decoration gesture, safe-zone overlay toggle)
- `Eyebrow` (Graduate label: "SERVING HAMMOND, TANGIPAHOA PARISH & THE NORTHSHORE", "THE DIRT ORDER", "STRAIGHT ANSWER", "THE FREE LOT WALK", "NOW BOOKING" (badged))
- `Headline`, `Subhead`, `Body`
- `GiantNumeral` ("01" to "04" only)
- `SequenceStrip` ("01 CLEAR · 02 DRIVEWAY · 03 PAD · 04 FOUNDATION DIG"; variant with one step highlighted in Bone and the rest in Dust)
- `StitchedBadge` (offer names; "DIRT ORDER #n" series label)
- `RustRule`
- `PhotoSlot` and `BeforeAfterSlot` (section 6; required label beginning "Real job photo:"; alt-text field)
- `Photo frame` (the image container variants of section 6)
- `Overlay plate` (Soil Black at 60 to 75 percent, straight-edged, for type over a real photo; never a gradient scrim)
- `Step` (numeral, icon, step name, one line)
- `Checklist item` (filled check icon plus text; never colour alone)
- `FAQ` (question, answer)
- `Notice` (Soil Elevated panel, Clay icon, Bone text; operations notices)
- `Call to action line` ("Book a Free Lot Walk · Call or Text 360-957-5865" as text; variants: both, Lot Walk only, phone only). **No drawn button on any social graphic.** A drawn equal-width button pair exists only on the carousel's last slide if the master kit's `CtaPair` is placed as a non-interactive illustration of the website, labelled as such; default off
- `Footer` (compact: wrightco.llc · standard: 360-957-5865 · wrightco.llc · expanded: the place line, phone, web address, email. Optional page number and source. Shows only supplied information: no address, no hours, no handle by default, no copyright line, no Facebook link)
- `Citation` (section 11)
- `Carousel page number` ("2 / 5") and `Swipe indicator` (an arrow in Copper, optional)
- `Chart frame`, `Legend`, `KPI tile` (section 11)
- `Sample data` flag ("Sample data. Not a published figure.")
- `ConfirmBadge`: `CONFIRM BEFORE PUBLISHING` in Source Sans 3 700, uppercase, Warning `#E8A33D` text on Soil Elevated with a 1 px Warning border and 2 px radius, with an alert icon and the words; on a Bone canvas it sits on its own Soil Elevated chip. Visible in every specimen that needs it.
- `LogoEmblem` (encodes the 480 px minimum on a 1080 px canvas, the clear space and the permitted grounds; switches to the Soil-square file on Bone)
- `ReviewQuote` (section 10: an empty future component only)

Template states to build: dark (Soil Black, Soil Surface), light (Bone, for reading-heavy cards), photo (a `PhotoSlot` today), text only, minimal (one line), text heavy (tips and FAQ), data (sample-flagged only). **Not built:** brand character (none exists), product and editorial states (no products, no editorial photography), service-photo state beyond the slot.

---

# 9. Content families and sample content

Build each family at portrait (1080 x 1350), square (1080 x 1080), Google post (1200 x 900) and story (1080 x 1920) unless noted, recomposed for each. Every template has named editable fields. Sample copy is a default, never baked into a component. **No Lorem Ipsum: every sample is publishable as written, or it carries a `CONFIRM BEFORE PUBLISHING` field.** All sample copy is BlakSheep Creative draft, in the voice of file 4: short sentences, the order of the work, "we" and "you", contractions, no adjectives about ourselves.

Families kept from the universal list: statement, tips, checklist, FAQ, process, announcement (reduced), before and after (as slots), problem and solution (as the honest version, below). Families added for this client: step cards, plain-talk tips (The Dirt Order), the Free Lot Walk, the seasonal message, now booking and service area, the Dirt Order guide teaser, the operations notice.

## 9.1 Step cards: "Step 01 / 02 / 03 / 04"

- **Layout:** Soil Black with grain. `GiantNumeral` top left in Copper. The step name in Graduate as the headline. One line in Source Sans 3 at 44 px. No rule: the numeral is the canvas's one gesture. `SequenceStrip` as the footer label with the current step highlighted. Compact footer "wrightco.llc".
- **Copy (exact steps, fixed lines):**
  - "01 CLEAR" · "Trees and stumps out." · optional second line "Stumps pulled, not just ground down."
  - "02 DRIVEWAY" · "Cut in so trucks can get to your home site."
  - "03 PAD" · "Your house pad, built up to the height on your survey." · optional "Your surveyor and the parish set the height. We build to it."
  - "04 FOUNDATION DIG" · "Dug the way your builder specifies, then handed off."
- **Caption default:** "First we clear it. Then we cut in the driveway. Then we build the pad. One crew, in order. Book a Free Lot Walk or call or text Cody at 360-957-5865."
- **Formats:** the four as single posts; a five-slide carousel (cover "ONE CREW. YOUR LAND. IN ORDER." with the emblem at 480 px, then 01 to 04); a 1200 x 900 Google post per step (numeral left, words right); a story per step.
- **Photo variant:** the step's `PhotoSlot` fills the top 58 percent, a Soil band beneath carries the numeral at 120 px and the step name. Ships only with a real photo.
- **Never:** re-ordered or renamed steps ("Drive", "Land Clearing", "Step 1"); ponds or hauling mixed in; a duration, acreage or price; the culvert install as Wright Co.'s job (W-08).

## 9.2 Plain-talk tip cards (The Dirt Order series)

- **Layout:** Soil Surface ground (or Bone for the longer ones). `StitchedBadge` "DIRT ORDER #n" top left. A question as the headline. One or two sentences beneath. A `Citation` line wherever a parish fact appears. Compact footer.
- **Samples:**
  - #1 "What comes first?" · "In Tangipahoa it's your 911 address, then the culvert permit, then us: clear, driveway, pad."
  - #2 "Why does the culvert come first?" · "In Tangipahoa, the parish won't start the culvert process without a 911 address, and installation can take up to 30 days after notice." · `Citation`: "Source: Tangipahoa Parish, [published process, date last checked]" with the date field `CONFIRM BEFORE PUBLISHING` (re-verify quarterly)
  - #3 "How high should my pad be?" · "Your surveyor and the parish set it. We build to it."
  - #4 "Do I need a permit to clear?" · "It depends on how much you clear. We'll tell you what applies to your lot. The application is yours to file." (any acreage threshold is a badged field from the parish's current published application)
  - #5 "What moves the price?" · "Acreage, how thick the trees are, stumps, how far the fill hauls, and how high the pad needs to be." · line "We'll walk it and put it in writing."
  - #6 "Why don't you run on wet ground?" · "It ruts your lot and makes a worse pad. When it's too wet, we wait."
  - #7 "Mulching or clearing?" · "Mulching is fine for trails, pasture and views. A house pad needs the stumps and roots out."
- **Tips variants (universal "Tips: 3, 5, 7, 10"):** a 3-tip and a 5-tip carousel built from these. No 10-tip version: there are not ten sourced tips.
- **Never:** an elevation, a flood-zone claim, "we handle your permits", a parish fact without its source and date, a guarantee of what the parish will do.

## 9.3 The Free Lot Walk

- **Layout:** Soil Black, contour lines as the gesture. `StitchedBadge` "THE FREE LOT WALK". Headline "BOOK A FREE LOT WALK". Support "Tell us where your land is and Cody will get back to you." `Call to action line` in Source Sans 3 700. The emblem at 480 px in the lower right (this is the one step-free card that carries it). Standard footer.
- **Variant A ("just closed"):** headline "JUST CLOSED ON LAND?" · support "Here's what happens first. Book a free lot walk and we'll look at yours."
- **Badged variant (W-07):** "Cody walks your land with you and maps clearing → driveway → pad on one sheet. No charge, no pressure." This full descriptor sits in a `CONFIRM BEFORE PUBLISHING` field and is off by default. So are "We'll flag your driveway and pad line" (the Flag Walk) and any distance.
- **Photo variant:** "Real job photo: Cody walking a lot with a landowner (with permission)" slot above, Soil band below.
- **Pin it:** a 1080 x 1350 version for the Facebook pinned post: "Just closed on land? Book a free lot walk."
- **Never:** "free" anywhere except "The Free Lot Walk" and "free estimates"; a price; "limited spots"; a countdown.

## 9.4 Seasonal: "Get your lot ready this winter. Build in spring."

A message, not a price offer. It runs on real facts only.

- **Layout:** Soil Black with grain, `RustRule` under the headline. Headline "GET YOUR LOT READY THIS WINTER. BUILD IN SPRING." (two lines). Support, the honest version: "The slow parts are the 911 address, the culvert permit and the culvert install. Start the paperwork and the clearing now, and the pad is ready when your builder is." Second panel or carousel slide: the culvert fact with its `Citation` (as 9.2 #2). `Call to action line`.
- **Carousel (5 slides):** (1) the headline (2) "Bought land this year? The slow part isn't the dirt work." (3) "911 address → culvert permit → culvert install." with the sourced culvert line (4) "Then we clear it, cut in the driveway and build your pad, while the ground lets us work." (5) "Walk it this winter, build in spring." and the CTA line.
- **Badged fields, off by default:** "October and November are usually the driest months around Hammond." (`CONFIRM BEFORE PUBLISHING`: verify against the NOAA station normals) · "We're booking winter lots now." (`CONFIRM BEFORE PUBLISHING`: only when true at the time of posting) · "a winter start plan" from the lot walk (W-07).
- **Weather line** that may run: "When it's too wet, we don't run equipment. It ruts your lot and makes a worse pad." "We'll text you when we're rained out and when we're back" is badged (W-10).
- **Never:** a price, a discount, "winter pricing", an early-bird anything, a bonus, a deadline, a countdown, "pad ready by spring", "guaranteed", **"your pad settles over winter"**, "let it settle", "winter is easy", "dry season" as a promise.

## 9.5 Now booking and service area

- **Service area card.** Soil Surface. Eyebrow "WHERE WE WORK". Headline "SERVING HAMMOND, TANGIPAHOA PARISH & THE NORTHSHORE". Support "Hammond, Ponchatoula and around. Not sure about your spot? Call or text and ask." An optional plain-text line of further Tangipahoa towns (Independence, Amite, Loranger, Tickfaw, Natalbany, Albany, Kentwood, Robert) as a badged field (W-07). **No map pin, no radius ring, no address, no "based in".** A simple parish-outline graphic is not used on social (it reads as a coverage promise).
- **Now booking card.** Soil Black. The headline "NOW BOOKING LOT WALKS" is itself a `CONFIRM BEFORE PUBLISHING` field (true at the time of posting), with the place line beneath and the CTA line. The safe default headline, usable any time: "BOUGHT LAND AROUND HAMMOND? LET'S WALK IT."
- **Never:** a town outside Tangipahoa named as served without W-07; "only X spots"; a date window.

## 9.6 The Dirt Order guide teasers

- **Layout:** Bone ground (reading), Soil Black text, `StitchedBadge` "THE DIRT ORDER" on its Soil chip, the subtitle always beneath: "Building on Raw Land in Tangipahoa, Step by Step." The first three steps as a numbered list ("Your 911 address" · "The culvert permit" · "Clearing"). Text line "Read The Dirt Order at wrightco.llc" (the guide's URL is a field, empty until the guide is published). Byline "Wright Co." (Cody's byline waits on W-19).
- **Link preview (1200 x 630):** the guide title in Graduate, the subtitle, the compact footer. No support sentence.
- **Carousel teaser:** cover (title + subtitle), three slides of steps, last slide "The full guide: wrightco.llc" and the CTA line.
- **Never:** the guide described as certifying permits, elevations or flood compliance; a published URL before the guide exists.

## 9.7 Before and after (photo slots only)

- **Layout:** `BeforeAfterSlot`: two equal frames, a 4 px Cattail Rust divider (the canvas's one gesture), a caption bar on Soil Black: "[Town] · [the work]" as two empty fields. Portrait stacks the two frames; square and Google post set them side by side; story stacks them between the safe bands.
- **Copy, when real:** "Same lot, [time apart]. 01 Clear → 02 Driveway → 03 Pad. Ready for the builder." The time apart, the town and the work are fields filled only from the real job record.
- **Status:** the whole family is `CONFIRM BEFORE PUBLISHING` and **never ships as slots.** It waits on the first Louisiana job shot from one fixed spot.
- **Never:** a stock, AI, illustrated or out-of-state photo; an invented town, date, acreage or duration; two different lots presented as one.

## 9.8 Job photo (on the job)

- **Layout:** one `Photo frame` at full bleed, untouched, with an optional caption bar on Soil Black. No other text on the image.
- **Caption format:** what + where + what's next + call to action. Format example only, posted only when true: "Six acres outside Independence. Stumps out and driveway cut in. Pad's next week. Bought land and don't know where to start? Call or text Cody, 360-957-5865."
- **Status:** a slot until real photos exist. Never ships as a slot.

## 9.9 Straight answers (FAQ and problem and solution, the honest version)

- **Layout:** single card and a three to five slide carousel, one question per slide. Soil Surface, eyebrow "STRAIGHT ANSWER".
- **Samples:** "Do you do the whole thing or just clearing?" · "Either. Most folks want the whole dirt side: clear, driveway, pad, in that order." · "Do you set the pad height?" · "No. Your surveyor and the parish do. We build to it." · "How much does it cost to clear an acre?" · "It comes down to how thick the trees are, the stumps, the debris, access and wet ground. We'll walk it and put it in writing." · "Do you do tree trimming?" · "That's tree work, not dirt work, so we're not the right crew." · "Is the lot walk really free?" · "Yes. The first look at your land is free." (in person every time is W-07)
- **Problem and solution:** the buyer's real problem, then the plain answer, never a competitor as the problem: "Builder says the site work's on you?" → "We do the dirt side: clear, driveway, pad." The FAQ cover slide is "STRAIGHT ANSWERS" in Graduate.
- **Never:** a figure for a cost question; a myth column (a "myth" tends to describe other companies).

## 9.10 Statement

- **Layout:** Soil Black, eyebrow, display line, one support sentence, `RustRule`. The tagline card carries the emblem at 480 px instead of the rule.
- **Samples:** "YOU BOUGHT THE LAND. WE'LL GET IT READY TO BUILD." · "FROM THE FIRST TREE TO THE HOUSE PAD." · "STUMPS OUT. DRIVEWAY IN. PAD UP." · "WE STOP WHERE YOUR BUILDER STARTS." with "No concrete, fencing, decking or tree care." · "WE'RE NEW TO THE HAMMOND AREA." with "So we're showing our work one lot at a time." · Offer statement: `StitchedBadge` "THE HOMEPLACE PACKAGE" with "Clear · Driveway · House Pad. One crew, one scope, build-ready." and "Ask what's included for your lot." (scope W-08).
- **Builder variant (builder posts only):** "ONE CREW. WOODS TO BUILD-READY." with the builder line "Text us the address and the survey." badged (W-12).

## 9.11 Operations notice (weather and schedule)

- **Layout:** a `Notice` panel on Soil Surface: Clay icon, one or two sentences in Bone.
- **Samples (posted only when true, fields empty by default):** "Rained out today. Clay needs a couple of dry days before we pad. Back at it [day]." · "Holiday: we're off [day, date]. Back [day]." Every variable field is `CONFIRM BEFORE PUBLISHING`.
- **Never:** an excuse, a guarantee, hours (none are on file).

## 9.12 Announcement (reduced)

- **Variants built:** "The Dirt Order is live" (empty until the guide is published); "Our Google Business Profile is up" (empty until it is); a new service (an empty slot that waits on W-11 or W-16); a holiday note (as 9.11). Every variable field badged.
- **Not built:** new employee (no crew detail on record, W-24), partnership, award, certification (none, and credentials are prohibited), milestone (a years or job-count milestone is prohibited), event (none on record).

## 9.13 Families from the universal list that are dropped or reduced

| Family | Decision | Reason |
|---|---|---|
| Statistic | Reduced | No business figure is publishable. The "statistic" is the parish process fact with its citation (9.2 #2) |
| Quote | Dropped | No customer quote exists, and research persona quotes are never published |
| Testimonial; review; rating | Reduced to one empty future template | Section 10. No review, rating or count exists |
| Problem | Merged | Into 9.9 |
| Problem, agitation, solution | Dropped | The brand does not agitate; buyers are already stressed |
| Comparison (A vs B, old vs new, good vs bad, feature) | Dropped | A comparison tends to describe other companies. The one fair comparison, mulching vs clearing, is a tip (9.2 #7) |
| Before vs after | Kept as slots | 9.7; waits on photos |
| Myth versus fact | Merged | Into 9.9 |
| Case study (cover, challenge, strategy, solution, result, metrics, testimonial) | Dropped | No Louisiana job exists yet. When one does, it is the job photo and before/after families with a caption, never metrics |
| Client results; KPI dashboard | Reduced | KPI tiles exist as components with sample data only (section 11) |
| Reports; audits | Dropped | Not a business that publishes reports |
| Offers; promotions | Reduced | No price, discount or bonus exists. The Free Lot Walk (9.3) is the only offer post; an empty `Offer` slot exists, flagged `CONFIRM BEFORE PUBLISHING` |
| Event | Merged | Into Announcement; none on record |
| Hiring | Dropped | Nothing on file; crew size is unconfirmed (W-24) |
| Community | Dropped | No community programme on record. A community note may run as an operations notice only when real |
| Blog promotion | Reduced | To The Dirt Order teaser and the link preview (9.6) |
| Podcast, webinar promotion | Dropped | The business runs neither |
| Thought leadership; industry commentary | Dropped | Nothing may be said about other companies or the industry |
| Branded memes | Dropped | Dry humour lives in captions, not meme graphics |
| Timeline; process | Kept | As the step cards (9.1) and the seasonal carousel (9.4) |
| Storm cleanup | Dropped | No campaign; a reactive post after a real event only, as an operations notice |
| Meet the crew; equipment showcase | Dropped | Nothing supplied; a machine is never the subject alone |

---

# 10. Review and testimonial templates

**No review, testimonial or rating exists.** Facebook shows a handful of unverified reviews whose state and customers are unknown (W-22); none is quoted, counted or shown. Research persona names and "quotes" are illustrations and are never published.

Build **one** component, `ReviewQuote`, as an **empty future template**, clearly marked:

- Its canvas carries a permanent banner across the top: "FUTURE TEMPLATE. NOT FOR USE UNTIL A REAL, VERIFIED LOUISIANA REVIEW EXISTS. `CONFIRM BEFORE PUBLISHING`".
- Four required fields, all empty: `quote` (verbatim, never edited; empty state reads "Paste a verbatim quote from a verified Louisiana review"), `reviewer` (first name and last initial, with permission), `source` (locked text "Google review"; never Google's logo), `date` (month and year). If any field is empty the canvas shows the banner and the badge in place of the quote.
- Stitched-patch frame on Soil Surface, quote in Source Sans 3 400 at 44 to 52 px, Bone. **No stars, no rating, no count, no reviewer photo, no avatar.**
- **No sample text of any kind** inside it, not even an obviously fake one. Specimens show the empty state only.
- No "leave us a review" graphic and no review-incentive post exist. A review is asked for in person or by text after a finished job, with no incentive.

---

# 11. Data, charts and citations

This client publishes almost no numbers. Build the chart system so the architecture is complete, and make the limits impossible to miss.

1. **No business figure is publishable today.** No price, acreage, lot count, job count, rating, review count, pad height, duration or years figure.
2. **The only real figures are parish process facts**, each with its source linked and dated (the culvert line in 9.2 #2), and the year in "since 2022".
3. **Every other figure in a specimen is sample data** and carries the `Sample data` flag on the canvas: "Sample data. Not a published figure." Use neutral labels ("Series A", "Q1") so a sample cannot be mistaken for a business fact. No specimen shows a price, acreage, rainfall or count, even as sample data.
4. No statistic about the business, the industry, the weather or any competitor may be published without a source the agency has checked. Rainfall normals stay out until verified against the NOAA station record. Show this as a callout above the data posts.
5. No chart is delivered on its own. Each is placed in a real platform canvas with a headline, a source line, the footer and one decoration gesture.

**Chart components, each inside `Chart frame`:** vertical, horizontal, grouped, stacked and 100 percent stacked bar; line, multi-series line, area; pie and donut; scatter and bubble; funnel and waterfall; gauge, progress bar and progress ring; sparkline; heat map; ranking; timeline; comparison matrix. Each supports title, subtitle, axis, grid, labels, values, legend, annotation, highlight, source, date and footnote. Build the component set; render specimens only for: a horizontal bar, a donut, a progress bar, a timeline (the sequence 01 to 04 as a process timeline, no dates) and a comparison matrix of the four steps (step, what happens, who sets it: "you", "the parish", "your surveyor", "us"), the last two with real, non-numeric content.

**KPI tiles:** one, two, three and four metric layouts and a dashboard grid, as components only, every value "00" with the `Sample data` flag. The component is industry-neutral. No client-results dashboard is built.

**Data palette, derived only from the approved colours.** Show it as swatches with token names.

| Token | On dark (default) | On Bone | Contrast | Note |
|---|---|---|---|---|
| `--data-1` | Bone | Soil Black | 18.17 | Primary series; `--data-highlight` adds a 4 px Copper outline |
| `--data-2` | Copper | Earth Brown | 5.74 / 7.45 | Second series, diagonal hatch |
| `--data-3` | Clay | Dust Dark | 10.33 / 7.28 | Third series, dots |
| `--data-4` | Dust | Cattail Rust | 8.59 / 4.82 | Fourth series, cross-hatch |
| `--data-positive` | Success, with a check glyph and a label | Success as a mark only, Soil Black label | | Dark grounds for text |
| `--data-negative` | Error, with a glyph and a label | Error as a mark only, Soil Black label | | |
| `--data-neutral` | Dust | Dust Dark | | Axis labels |
| `--data-track` | Soil Elevated | Bone Alt | | Tracks, never data |
| `--data-grid` | `--border-subtle` | `--border-subtle-light` | | Grid lines |

The series sit close together (Clay against Dust is 1.2 to 1; Copper against Clay 1.8 to 1). So adjacent series are separated by a 2 px gap in the ground colour, labelled directly, and distinguished by pattern, line style or marker shape as well as colour. No hue outside this table enters a chart. No gradient fills.

**Citation component.** Two forms: `Source: Organization, Year` and `Source: Organization · Report · Year`. For this client the working form is `Source: Tangipahoa Parish, [document], checked [date]`, with the date field `CONFIRM BEFORE PUBLISHING` until re-verified. Dust on dark, Dust Dark on Bone, 30 px on a 1080 px canvas, always inside the safe zone. Never fabricate a source or a statistic. A figure with an empty source field does not render.

---

# 12. Avatars, banners, covers, video

## 12.1 Avatar system

- **Master:** the supplied `assets/logos/avatar/wright-co-avatar-emblem-on-soil-1024.png`: the emblem small inside a Soil Black square, sized so the circle crop never clips the art. Composite it unaltered. Do not draw it.
- **Sizes, also supplied:** `-512.png` (Google Business Profile), `-400.png`, `-320.png` (Facebook, Instagram), `-180.png` (touch icon).
- Show the master in a square and in the circular crop, and the previews the universal system asks for at 256, 128, 64 and 32 px, built by downscaling the supplied 1024 and 512 files, never by redrawing. **Report honestly:** at 180 px and below the phone number does not read; at 64 px and below only the bone lettering band registers; at 32 px it is a light band on dark. Print that note on the plate.
- **Not built:** a symbol, monogram, brand mark, character head or founder portrait avatar. None exists; the drawn small mark (logo #4) is a `LogoSlot`. The favicon crop is never an avatar.
- The same avatar on every platform.

## 12.2 Banners and covers

Each shows the full canvas, the desktop safe zone, the mobile safe zone, the logo area, the one-line area and the image area, with the crop zones drawn.

| Asset | Size | Build |
|---|---|---|
| Facebook page cover | 1640 x 924 | Soil Black with grain and contour lines. The transparent emblem centred inside the middle 1640 x 624 at 480 px or more, with clear space. Variant: the tagline in Graduate at 48 px beneath. Later variant: the before/after of one real lot (slot) |
| Google Business Profile cover | 1080 x 608 | `emblem/wright-co-emblem-on-soil-landscape-1200x628.png`, cropped to 16:9 within the art's clear space, or a real photo once one exists. No added text |
| YouTube channel banner | 2560 x 1440 | Soil Black; the emblem and "The Dirt Order" with its subtitle inside the centre 1546 x 423. Labelled "no account on file" |
| X, LinkedIn, Bluesky, Pinterest, community, event, podcast, webinar banners | per table | Not built. Mapped in the table by recomposing the Facebook cover |

The avatar and page name supply the brand. A cover carries one line at most, and no rating, seal, address, town list or phone (the phone is already in the emblem's banner).

## 12.3 Story and reel covers

On the 1080 x 1920 master. Draw the safe zones as a switchable overlay: top 250 px (user information) and bottom 340 px (captions, controls, navigation) clear; the headline in the centre band; the footer lifted above the bottom zone; a reel cover keeps its subject in the centre 1:1. Build: a step cover ("01 CLEAR" numeral), a tip cover ("DIRT ORDER #3"), a Free Lot Walk cover, and a video cover holding the "Real job vertical video" slot under an overlay plate. Facebook reels and stories are in use; Instagram, TikTok and Shorts covers are the same master, labelled by status.

## 12.4 YouTube thumbnails

One dominant idea, five words at most, legible at 210 px wide, lower right clear for the duration badge. Labelled "no account on file".

- **Build:** text focused ("HOW HIGH SHOULD MY PAD BE?" on Soil Black with a Copper "#3" badge); how-to ("WHAT COMES FIRST ON RAW LAND"); before and after (two `PhotoSlot`s with the Rust divider; waits on photos); service ("LAND CLEARING, STUMPS OUT" with a slot).
- **Do not build:** human focused (no photograph of Cody), product focused (no products), screenshot focused, data focused (no figures), reaction, commentary, news, review, client result, list, brand character.

---

# 13. Carousel, infographic and repurposing

**Carousel.** Slide 1 hook, slide 2 context, middle slides content, penultimate summary, final slide the call to action line on Soil Black with the emblem at 480 px. Persistent compact footer, page numbers ("2 / 5"), an optional Copper swipe arrow, one consistent content area, one ratio for all slides (1080 x 1350). Build: the sequence (9.1), the Dirt Order tips (9.2), the seasonal message (9.4), the Dirt Order teaser (9.6), straight answers (9.9), a "how to" ("What to have ready for your lot walk": your survey or plat, your builder's spec, your 911 address if you have one). Not built: case study, statistics, myth versus fact, industry commentary, data.

**Infographic.** Modular sections: header, introduction, numbered step, icon step, timeline (the sequence, undated), checklist, warning (a `Notice`), recommendation, source (`Citation`), call to action, footer. Hero stat, statistic, chart, quote and comparison modules are left out (no figures, no quotes, no comparisons). Build one tall specimen on 1080 x 1920 and one on 1080 x 1350: "Building on raw land in Tangipahoa: what comes first", with 911 address → culvert permit → 01 Clear → 02 Driveway → 03 Pad → 04 Foundation Dig, the culvert fact with its citation, the pad-height line and the CTA line. For anything longer than one screen, use a carousel. The 1000 x 1500 tall format is mapped but not built (no Pinterest).

**Repurposing one concept.** Begin with the sentence to be said, then choose canvases. Document it with the line "You bought the land. We'll get it ready to build.":

1. Write the line and its one support sentence ("We clear the trees and stumps, cut in your driveway and build your house pad. One crew, in order.").
2. **Facebook portrait 1080 x 1350:** eyebrow (the place line), the line, the support, the emblem at 480 px.
3. **Square:** the line low on the canvas, the sequence strip above it, compact footer.
4. **Google post 1200 x 900:** the line left, the sequence strip right. Tested at small card size.
5. **Story:** the line inside the centre band, the footer lifted clear of the bottom zone.
6. **Link preview:** the line as a headline beside the emblem, compact footer, no support sentence.
7. **Thumbnail:** "READY TO BUILD." beside a slot.
8. **Carousel:** the line is slide 1, the steps are slides 2 to 5, the CTA is slide 6.
9. **Cover:** the line beneath the emblem on the Facebook cover variant.
10. Instagram, YouTube community, LinkedIn, X and Pinterest versions are mapped in the coverage table, not built, by status.

Preserve the message, the brand and the hierarchy. Change the composition, the amount of text, the crop, the scale and the safe zones. Show the plate "one message, every format" as the argument for the first rule in section 3.

---

# 14. Calls to action, captions and hashtags

**Calls to action. These and no others.**

| | Wording | On a graphic | Goes to |
|---|---|---|---|
| Primary | **Book a Free Lot Walk** | One line of text, Source Sans 3 700. No drawn button | The Free Lot Walk page on wrightco.llc |
| Secondary | **Call or Text 360-957-5865** | One line of text, or paired with the primary as "Book a Free Lot Walk · Call or Text 360-957-5865" | `tel:+13609575865` |
| Text link | **Read The Dirt Order** | One line | The guide, once published |
| In a sentence | "Call or text Cody at 360-957-5865, or book a free lot walk." | Captions | |

Where a button pair is shown at all (the website illustration on a carousel's last slide, off by default), the two are equal width, primary first, and the phone is a button, not a bare line. **Excluded from the universal CTA list:** "Learn More", "Get Started", "Request Quote", "Book Now", "Call Now", "View Service", "Read More", "Download", "Save", "Share", "Follow", "Contact Us". Also never "Get a Quote", "Get a Free Estimate" as a button, "Get Your Lot Build-Ready", "Limited Time" or any "Wright" pun.

**Captions.** One job, one photo, one next step once photos exist; until then, one idea and one next step. What + where + what's next + call to action. Two to four sentences on Facebook; short on Google, no hashtags. "We" for the company, "you" for the reader; "I" only once W-19 clears and Cody is writing. Contractions always. Sentences under 10 words where possible. At most one exclamation mark, none in a headline. Zero to two emoji in a Facebook caption at most; none in artwork or on Google. No dashes in a caption that is also used as a text message. Nothing essential (the phone, a date) appears only in the image. Captions obey section 4 exactly as artwork does. Reply to comments in the thread with a straight answer, then move to text; never a price in public.

**Hashtags.** None in artwork. None on Google Business Profile posts. On Facebook (and Instagram, once an account exists), two or three at most, from this list only (BlakSheep Creative proposal):

`#HammondLA` · `#TangipahoaParish` · `#Northshore` · `#LandClearing` · `#HousePad` · `#BuildingOnRawLand`

**Banned tags:** any competitor's name; `#Licensed`, `#Insured`, `#Bonded`; `#BestOf`, `#Top`, `#Premier`; any town or parish tag outside the place line before W-07; `#Trucking`; `#Excavation` as the lead tag; price, discount or deal tags; any "Wright" pun tag; tags about another state.

**Bio line for every profile:** "Land clearing, driveways & house pads around Hammond, LA. You bought the land, we'll get it ready to build. Free Lot Walk · 360-957-5865"

---

# 15. Accessibility

- Text meets WCAG 2.1 AA at minimum; body text on feed graphics reaches 7 to 1. Use only the pairs in the master kit's contrast table.
- Smallest running text 36 px on a 1080 px canvas; the label and source styles at 28 to 30 px are the only exception.
- Graduate is never used for running text and never below 28 px on a 1080 px canvas.
- Test every Google post at small card size, every thumbnail at 210 px wide, and the avatar at 32 px; report what fails.
- Colour is never the only signal in a chart, a checklist, the sequence strip (the current step also changes weight or carries an underline) or a status badge.
- Every template has an alt text field and a caption field. Alt text says what is in the frame; for a type-led card it repeats the words on the card.
- Nothing inside a platform's chrome zones.

---

# 16. Organisation, naming, editability, documentation

**Editability.** Components, variants, variables, tokens, auto layout, named text layers, named image layers, named groups and reusable styles. Nothing is flattened. Sample copy lives in fields, not in component definitions.

**Naming.** Semantic, with no client name: `Social / Feed / Portrait / Step` · `Social / Feed / Square / Tip` · `Social / Feed / Portrait / Lot Walk` · `Social / Feed / Portrait / Seasonal` · `Social / Feed / Square / Service Area` · `Social / Google Post / Step` · `Social / Story / Step` · `Social / Carousel / Cover` · `Social / Carousel / Content` · `Social / Feed / Portrait / Before After Slot` · `Social / Future / Review Quote` · `Video / Thumbnail / How To` · `Video / Vertical / Cover` · `Banner / Facebook` · `Banner / YouTube` · `Data / Bar / Horizontal` · `Data / KPI / Two Metric` · `Infographic / Steps` · `Component / Citation` · `Component / Call to action line` · `Component / Photo Slot`.

**Library order.** (1) Foundations and token flow (2) Active client brand (3) Components (4) Avatars (5) Feed posts (6) Google posts (7) Stories (8) Vertical video (9) Carousels (10) Banners and covers (11) YouTube (12) Data visualisation, charts and KPIs (13) Infographics (14) Reviews: the one future template (15) Educational: steps, Dirt Order tips, straight answers, checklist (16) Seasonal, Free Lot Walk, service area, announcements, operations notices (17) Platform Specifications (18) Documentation. Testimonials, case studies and promotions are omitted for the reasons in 9.13.

**Plates to deliver, in the reference kit format's order:**

1. Section opener and the token flow, with a table of which concern lives in which file.
2. The four rule cards.
3. Master format families as ratio tiles, then the table.
4. The Platform Specifications table with status, and the "Adding a platform" callout.
5. Social type scale and spacing tokens.
6. The data palette swatches.
7. Content families available; charts available; repurposing one concept.
8. The template library rendered by ratio: portrait, square, Google post, landscape and link preview.
9. Story, video cover and carousel, with the safe-zone specimen.
10. YouTube thumbnails.
11. Banners and covers with crop zones.
12. The avatar system, with the honest size report.
13. The tall infographic with its module list.
14. One message, every format.
15. The decoration layer: the five grounds, the three gestures, the "one gesture per canvas" callout, and six composed canvases.
16. Data posts: charts inside real canvases, by ratio, with the sample data callout.
17. The photo-slot plate: every standard slot, and the rule that slots never ship.
18. Switching this architecture to another client.
19. A coverage table: family by format, marking what is complete as type on soil, what is a slot, what waits on the owner, and what is mapped but not built.

**Documentation to include.** Which design system is active; how tokens flow; logo use (composite only, 480 px on a 1080 canvas, dark grounds, the Soil container on Bone); type (Graduate 400 with `font-synthesis: none`, Source Sans 3); colour; grid and spacing; photo-slot treatment and the rules for when photos arrive; the chart system and its limits; the citation component; platform safe zones; template naming; how to create a new template; how to update a platform dimension; how to add a content family; how to add a platform; how to switch client.

**Switching to another client.** (1) Load the new client's design system and replace `tokens/css-tokens.css`. (2) Replace `assets/` and the paths in the logo, avatar and footer components. (3) Replace typography tokens. (4) Replace imagery rules and re-derive `--data-*` in `tokens/social.css`. (5) Replace or remove the client-specific components: the giant numeral and sequence strip, the stitched badge, the contour lines, the photo-slot label rule, the claims register, the CTA line wording. (6) Keep the canvas, the type roles, the chart frame, the chart set and the family architecture. (7) Review every composition for brand fit and adjust. Recolouring this client's posts does not make another client's system.

**Future content types.** A new platform or asset type needs only its canvas specification, safe zones, crop rules and the mapping of existing families into its ratio. The brand and content components stay as they are.

---

# 17. Quality control

Before any template is marked complete, verify:

**System**
- Correct dimensions, from the Platform Specifications table, with the row's date checked.
- Every colour, size, radius and space resolves to a token. No typed-in hex value.
- Recomposed for its ratio, not resized or cropped from another.
- Nothing inside a safe zone's excluded area. Nothing flattened. Layers named.
- Graduate at 400 with `font-synthesis: none`; Source Sans 3 for everything else; no third family; no running text under 36 px on a 1080 px canvas.
- One ground, at most one panel colour, one decoration gesture. No gradient, shadow or glow. Radius 2, 4 or 8 px or a chamfer; no pill.

**Brand**
- The library is labelled a BlakSheep Creative draft, version 0.1, not approved by the owner.
- The logo is a supplied emblem file, composited, unaltered, at 480 px or wider on a 1080 px canvas, on a Soil ground or inside a square-cornered Soil container on Bone, once per canvas. Nothing from `assets/logos/source/`. No monogram, no corner mark, no "WRIGHT CO" in type.
- "Wright Co." with the period. No "LLC". "Cody", never "founder".
- No photograph anywhere. Every photo position is a `PhotoSlot` whose label begins "Real job photo:", and no template that depends on a slot is marked ready to post.

**Claims**
- Nothing outside file 6's approved list; every promise the owner has not made sits in a `CONFIRM BEFORE PUBLISHING` field.
- No licence, insurance, bond or credential. No years in the area. No rating, star, count or review quote. The review template is empty and bannered.
- No price, discount, bonus or price word. Cost questions are answered with what drives the price.
- No pad height, flood promise, permit handling, guarantee, "pad ready by spring" or "settles over winter".
- No address, map pin or radius ring. Only the place line, Hammond and Ponchatoula, plus badged towns.
- No competitor named or described; none of the banned phrases.
- The sequence reads "01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig" exactly. The offers carry their descriptors.
- Calls to action read "Book a Free Lot Walk" and "Call or Text 360-957-5865" (plus "Read The Dirt Order"), as text lines; no drawn button on a graphic.
- Hashtags: none in artwork, none on Google, at most three from the approved list on Facebook.
- Every `CONFIRM BEFORE PUBLISHING` field is visible and editable.

**Last check, and the most important.** No asset, colour, font, phrase, figure, motif or layout detail from any other client appears anywhere: not from the reference kit format file, not from any other kit in this workspace, not from a previous project, and nothing from the owner's other business. Search the finished library for any colour that is not in `tokens/css-tokens.css`, any font that is not Graduate or Source Sans 3, and any name that is not this company's. Do not hard code BlakSheep Creative into a component; it appears only in the provenance label.

---

# 18. Final report

Finish with three things, in this order.

1. **Inventory.** Every template and every component built, by its semantic name, with the formats each exists in, and actual counts.
2. **Coverage table.** Family by format. Mark each cell as one of: complete as type on soil; slot (waits on a real photo); badged (waits on the owner); mapped but no specimen; not built. Beside the table, list every family and system that was reduced or dropped, with the reason from section 9.13, 10 or 11.
3. **One list of every `CONFIRM BEFORE PUBLISHING` field**, grouped by W number where it has one (W-03, W-05, W-07, W-08, W-10, W-11, W-12, W-16, W-19, W-21, W-22, W-24, W-25, W-26), with what is needed to clear it and which templates unlock when it clears.

Do not report anything as built that was not built. Do not report a slot as a finished template. Do not describe any part of the library as approved.
