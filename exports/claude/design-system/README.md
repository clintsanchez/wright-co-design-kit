Wright Co. is a land clearing and home-site prep crew serving Hammond, Tangipahoa Parish and the Northshore in Louisiana. It takes wooded land to build-ready in one order: **01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig**. The page should look like the ground itself and like a local crew's truck door: dark soil, rust and bone, heavy collegiate lettering, square edges.

**Status.** The name, the emblem, the colors sampled from it, the phone (360-957-5865), the email and wrightco.llc are the client's own. Color roles, typefaces, radii, component rules and voice are BlakSheep Creative proposals the owner, Cody Wright, has not yet approved. Keep every unapproved item visibly marked `CONFIRM BEFORE PUBLISHING` (a `warning` badge on dark).

## Content fundamentals

Write like Cody explaining the job over a tailgate: short sentences, the customer's own words, the work in the order it happens.

- **Walk the order.** First, then, then. "First we clear the trees and stumps. Then we cut in the driveway so trucks can get in. Then we build the pad."
- **Show it, don't claim it.** No adjectives about the company. Not "Hammond's premier, top-rated land clearing experts."
- **Straight about the hard parts.** Answer "how much?" with what drives the price: "Price comes down to five things: acreage, how thick the trees are, stumps, how far the fill hauls, and how high the pad needs to be."
- **Local, without the costume.** Name towns (Hammond, Ponchatoula, Independence, Amite) and ground (clay, low corners, pine and sweetgum). No gators, no "cher".
- Use "you" and "your land"; name Cody, not "our team". Contractions always. American English. Sentence case in source; CSS uppercases display type and buttons. No italics for emphasis; use weight 600 or 700. No emoji anywhere.
- Write "Wright Co." with the period. No "LLC" except inside the web address.
- The sequence always reads "01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig": never re-ordered, renamed or mixed with add-ons. The Homeplace Package always carries "Clear · Driveway · House Pad. One crew, one scope, build-ready."
- Never state: licensed, insured, bonded or any credential; a star rating, review count or review quote; a price, range or per-acre rate; a street address or hours; years in Hammond or Louisiana ("Clearing and excavating since 2022" is the only history line); a pad height, flood promise, permit handling or guarantee; any competitor's name.

## Color

Dark-first, one warm hue family. With eyes half shut a page reads as dark earth, bone type and one rust button.

- `bg-base` (Soil Black) is the page. Alternate dark sections `bg-base` / `bg-surface`; raised things sit on `bg-elevated`. Long reading (process, FAQ, estimate form) goes in `bg-light` sections. Roughly 70% Soil, 15% Bone, 10% `brand-secondary` and `brand-accent`, 5% rust and copper.
- **One thing in rust.** `brand-primary` fills the primary button and nothing else solid on that screen. Copper numerals and one rust rule may sit with it.
- `brand-primary-bright` (Copper) is for dark grounds: links, eyebrows, step numerals, the phone ring, focus rings. It only ever holds `text-on-light` text. Never a resting button fill.
- Text: `text-primary` and `text-muted` on Soil grounds; `text-on-light`, `text-muted-on-light` and `brand-secondary` on Bone.
- Status colors are UI states only and fail as text on Bone: on Bone, a field error is a 2px `error` border plus an `error` icon, the message in `text-on-light` at 600. There is no info color: a neutral notice is a `bg-elevated` panel with `text-primary` text and a `brand-accent` icon.
- Never add green, safety yellow, blue or any cool accent as a brand color. No gradients. No shadows. Color is never the only signal: links are underlined, errors carry text and an icon.

## Type

- `display`, `h1`, `h2`, `eyebrow` and step numerals: Graduate 400, uppercase, at most two lines and eight words. Graduate has one weight: always `font-weight: 400` and `font-synthesis: none`. Never for H3, buttons, nav, labels or paragraphs.
- Everything else: Source Sans 3 (`h3` 700, `lead`, `body` 400, `label` 600, `button` 700 uppercase +0.06em, `small`). Body is 18px; nothing on the web goes below 14px. Tabular figures for phone lines and tables.
- Both families load from Google Fonts (`family=Graduate&family=Source+Sans+3:wght@400;600;700`). Never request Graduate at 700. Without the brand fonts: Rockwell Bold headings, Arial body.
- Avoid Oswald or any condensed grotesk, grunge or script faces, light weights, all-caps paragraphs, and a third typeface.

## Space, shape and layout

- 8px base, six steps only: `space-1` to `space-6`. Section padding `space-4` on mobile, `space-5` on desktop, `space-6` for the hero and closing band only. Cards pad `space-3`.
- Angular: `radius-sm` for buttons, inputs and badges; `radius-md` for cards; `radius-lg` for media and photo slots. The chamfer (an 8 to 12px 45-degree cut) is the brand's alternative to a rounded corner: badges, sequence cards, the top-right of service cards. No pills, ever.
- Borders: 1px `border-subtle` on dark, 1px `border-subtle-light` on Bone; form fields 1px `text-muted-on-light`, focus 2px `brand-primary`. A rust rule (3 to 4px `brand-primary`) sits under each H2. Sections are separated by a change of ground, never a line.
- Content caps at `container`. Design at 360px first; tap targets 44px; buttons 52px tall. Each section opens the same way: optional eyebrow, H2 with a rust rule, optional lead, then one kind of content.
- Backgrounds beyond flat grounds: soil grain at 6% or less on dark only, and topographic contour lines in `brand-accent` at 8 to 10%, once per page at most.
- Motion: 150ms ease-out color changes only; nothing under `prefers-reduced-motion`. No bounce, parallax, scroll reveals, counters or auto carousels.

## Logo

There is one logo: the client's raster emblem (distressed bone varsity "WRIGHT CO" with rust bevels on a soil Louisiana silhouette, the phone in a banner). Every file is in the Logos asset group, with its grounds and sizes in that group's note.

- Composite the supplied files only. Never redraw, trace, retype, recolor, sharpen, crop the phone banner, or add "LLC", a tagline or a badge.
- Never set "WRIGHT CO" in Graduate or any font as a stand-in for the logo. Where a header wordmark is needed, use a labelled slot: "Wordmark (logo #3), not yet drawn. CONFIRM BEFORE PUBLISHING".
- The transparent emblem sits only on `bg-base`, `bg-surface`, `bg-elevated`, or a photo under a 60%+ Soil overlay, at 240px wide or more, with clear space one tenth of its width. On Bone, use the Soil square inside a square-cornered `bg-base` container. Once large per view.
- Still missing: a vector master, a no-phone emblem, a flat wordmark, a drawn small mark and one-color versions. Show them only as labelled slots.

## Buttons

Exactly two labels, as a pair, equal width, primary first: **Book a Free Lot Walk** (solid `brand-primary`) and **Call or Text 360-957-5865** (outlined, linked `tel:+13609575865`). One pair per view; a second Lot Walk on the same screen is a text link. See the Button component.

## Iconography

Proposed: Phosphor (Fill) or Tabler (filled); no set is chosen or bundled yet. Solid glyphs with square ends, or 2px+ strokes with square caps; no rounded or duotone sets. 24px beside text, 20px in a button, 32px on cards. `brand-accent` or `brand-primary-bright` on dark; `text-on-light` on Bone. Every icon has a text label. No machine, tree, shield or arched-badge device as identity.

## Photography

None exists. Every photo position is a labelled slot: a `bg-surface` or `bg-elevated` box at the final ratio (4:5, 1:1 or 16:9), a thin `brand-accent` border, `radius-lg`, labelled "Real job photo: [what]". Never stock, AI scenes, equipment renders or photos from the owner's Washington business. When real photos arrive: raw documentary, captioned with town and work in `small`. The Photos asset group holds only AI and stock images: reference or labelled placeholders, never published as Wright Co. work.

## Not synced

From `clintsanchez/wright-co-design-kit@561b18a`:

- **Type sizes** are the desktop maxima of the source's `clamp()` values; the mobile minimums are in each style's usage note. `--font-display-weight` (400) lives in the display styles rather than as a token.
- **Fonts**: no files in the repository (Graduate and Source Sans 3 are Google-hosted), so none were copied.
- **Logos**: the full `assets/logos/` set is in the Logos group (added on the page); `favicon.ico` sits there as a file.
- **Photos**: the Photos group (66 AI and stock images) was added on the page, not from the repository, which holds zero photos.
- **Components**: the repository has no component library. Button is hand-written from the CSS in `3 - Visual Identity.md` §10 as a static preview. Cards, sequence cards, badges, form fields, header and call bar are specified in prose only and were not built.
- **Icons**: none in the repository.
