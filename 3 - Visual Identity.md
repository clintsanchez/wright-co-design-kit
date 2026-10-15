# 3. Visual Identity

Wright Co. Version 0.1, 2026-10-15. Prepared by BlakSheep Creative. Values of record: `tokens/css-tokens.css`.

**Status.** Nothing in this file has been approved by the owner, Cody Wright. He has seen none of it. The emblem and the colors sampled from it are the company's own and stay. The color roles, the typefaces (Graduate and Source Sans 3), the 2 / 4 / 8 radius, the component rules, the graphic devices and every layout rule are BlakSheep Creative decisions, usable now, with the owner's sign-off pending. Where this file states a value the sources do not, it says "Default".

**Built from.** The brand style guide (version 2.0), the visual identity brief, the messaging framework, the site architecture and `tokens/css-tokens.css`. Where a value appears in more than one of those, the token file wins.

**The idea.** The page should look like the ground itself, and like a local crew's truck door rather than a franchise website: dark soil, rust and bone, heavy collegiate lettering, square edges. Soil Black carries the page. Bone carries the long reading. Cattail Rust marks the one thing to press. With eyes half shut, a page reads as dark earth with bone type and one rust button.

| Principle | In practice |
|---|---|
| Show the ground, not the gear | Lead with the land and the result. No bare machine as a hero. With no real photo yet, type, the numbered sequence and soil texture carry the hero |
| Heavy and square | Graduate capitals, 2 px buttons, 4 px or chamfered cards, rust rules. Nothing rounded, light or airy |
| One thing in rust | Rust is for action. Three rust things on a screen means two are wrong |
| Grit lives in the logo and the photos | The emblem is illustrated and distressed. Type, UI and layout stay clean and readable in one look |

---

## 1. Logo system

### What the logo is

**The primary logo is the illustrated emblem.** Distressed bone-white varsity lettering "WRIGHT CO" with rust bevels, over a soil-filled Louisiana silhouette with cattails and marsh grass. The client's original is a raster of about 1536 × 1024 on a black ground with an outer glow, and it carries the phone number in a banner.

The artwork reads "WRIGHT CO" without the period. The written name is "Wright Co." (file 2). The artwork is not changed to match.

It is the most distinctive mark in the local market, and the job is not to redesign it. It is to build a system around it.

### Files and where they live

All logo files are in `assets/logos/`. `assets/logos/README.md` lists every file, what it contains, its grounds and its sizes, and it is the authority on which file to place where. This file sets the rules those files obey.

| Folder | What it holds | Use |
|---|---|---|
| `assets/logos/source/` | The client's original emblem files, as received | Reference only. The masters the other folders were prepared from. Not placed in layouts directly |
| `assets/logos/emblem/` | The emblem, prepared for layouts | Hero, cover, closing slide, footer, print. On dark grounds only, 240 px wide or larger |
| `assets/logos/avatar/` | The square profile picture prepared from the emblem | Every profile picture, the same on every platform |
| `assets/logos/favicon/` | The browser and touch icons | Browser tabs, bookmarks, home-screen icon |

### The logo system still to be drawn

The emblem works large and on dark. It does not work small, in one color, or in a header. The style guide commissions a vector logo system from a designer (a human vector redraw, not an auto-trace). **None of it exists in this kit until it is delivered.** Claude Design does not draw, trace or generate any of it; where one is needed, it uses a labelled logo slot marked `CONFIRM BEFORE PUBLISHING`.

| # | Version | Construction | Use | Minimum |
|---|---|---|---|---|
| 1 | Emblem, no phone (the new primary) | Full illustration, phone banner removed | Website hero, social cover, truck doors, yard signs, shirt backs | 240 px / 2 in wide |
| 2 | Emblem, transparent | Black vignette and outer glow removed | Over dark photos, Soil sections, merch | 240 px / 2 in |
| 3 | Horizontal wordmark | "WRIGHT CO" flat in the emblem's varsity letterforms: Bone fill, one solid Rust offset outline, no distressing below 200 px. Optional small state silhouette at left | Site header, email signature, estimates, invoices | 140 px / 1.25 in |
| 4 | Mark only | State silhouette filled Soil, Rust outline, a single Bone "W". No grass or cattails | Favicon, avatar, hat front, stamps | 32 px / 0.5 in |
| 5 | One-color versions of 1, 3 and 4 | Bone only, Soil Black only, Rust only | Embroidery, one-ink print, vinyl, stamps, engraving | As above |
| 6 | Vector masters | AI, EPS, SVG, PDF; PNG at 512, 1024 and 2048; a 512 × 512 avatar | Print, signs, wraps, embroidery | n/a |

When any of these arrives, it goes into `assets/logos/`, the README is updated, and the matching slot in every layout is replaced.

### Until the system is drawn

- Use the emblem from `assets/logos/emblem/` at 240 px wide or larger, on a dark ground.
- **Header:** the wordmark (#3) belongs here and does not exist. In drafts, use a labelled slot: "Wordmark (logo #3), not yet drawn. `CONFIRM BEFORE PUBLISHING`". Where a live page must ship first, place the emblem at 240 px and let the header grow. Never set "WRIGHT CO" in type as a stand-in.
- **The phone banner.** The phone number never lives inside the logo in new work. Use a phone-free emblem where the README lists one. If the only emblem available for a placement carries the banner, it may be used at 240 px or larger on a dark ground, provided the number in it is the confirmed 360-957-5865. Do not crop, mask or paint the banner out of a file; that is a redraw. Where the layout allows, set the phone separately in type as well.
- **Avatar and favicon:** use the files in `assets/logos/avatar/` and `assets/logos/favicon/` as supplied. When mark #4 is delivered, it replaces them.

### Clear space

- **Emblem:** one tenth of its width on every side. At 240 px wide, 24 px.
- **Wordmark** (when it exists): the cap height of the "W" on every side.

| Emblem width | Clear space |
|---|---|
| 240 px | 24 px |
| 320 px | 32 px |
| 480 px | 48 px |
| 2 in | 0.2 in |

### Minimum size

| Mark | Minimum |
|---|---|
| Emblem, on screen | 240 px wide |
| Emblem, in print | 2 in wide |
| Wordmark (#3, when delivered) | 140 px / 1.25 in |
| Mark only (#4, when delivered) | 32 px / 0.5 in |

Below 240 px the emblem's grass, cattails and distressing turn to noise. Switch to the wordmark or the mark, or, until they exist, leave a labelled slot.

### Approved backgrounds

- Soil Black `#120C06`: the full-color emblem. This is its home.
- Soil Surface `#20150C` and Soil Elevated `#2E1D10`: the full-color emblem.
- A photograph under a Soil overlay of 60 percent or more: the full-color emblem.
- Bone `#F9F7F4` or Bone Alt `#ECE1D8`: only inside a square-cornered Soil Black container around the emblem, or with the Soil Black one-color version once it exists.

### Incorrect usage

Do not:

- Stretch, squash, rotate, tilt or re-proportion it.
- Recolor the lettering, swap the rust for another color, or tint the soil.
- Add a shadow, glow, outline, stroke, bevel or gradient. The art already has its own bevel.
- Put it straight onto Bone, white, Copper, Rust or a busy photograph without a dark container or overlay.
- Use it below 240 px.
- Add "LLC", a tagline, a phone number, "Est. 20XX" or any badge to the lockup.
- Redraw, trace, re-vectorize, upscale, clean up or generate the emblem, the lettering, the silhouette, the cattails, a wordmark, a mark, an avatar or a favicon with any tool, AI included.
- Set "WRIGHT CO" in Graduate, or in any typeface, and call it the logo.
- Imitate the emblem's distressing as a texture or font effect on running type.
- Pair it with machine icons, tree silhouettes, shields or arched badges. Those are the category's clichés and another company's look.
- Build a monogram. "WC" is not used.

---

## 2. Color system

The palette is one hue family at one temperature: warm earth, a near-black and an off-white. The core colors were sampled from the client's emblem on 2026-10-14; Copper and Dust Dark were derived for contrast. **Color personality:** weathered, warm, earthy. Wet clay, rusted iron, cattails in October.

No Pantone, vinyl or paint reference is on file. The CMYK figures are straight screen conversions from the style guide, for reference only. For print, give the printer the vector file (once it exists), the hex value and a press proof to match.

### Primary colors

| Name | Token | HEX | RGB | CMYK (approx.) | Source | Use |
|---|---|---|---|---|---|---|
| Cattail Rust | `--brand-primary` | `#A15C27` | 161, 92, 39 | 0, 43, 76, 37 | Sampled | The primary button: the one thing to press. Links on Bone. Rust rules |
| Copper | `--brand-primary-bright` | `#C8783A` | 200, 120, 58 | 0, 40, 71, 22 | Derived | On dark only: links, eyebrows, step numerals, icons, the phone button's ring, focus rings |

### Secondary colors

| Name | Token | HEX | RGB | CMYK (approx.) | Source | Use |
|---|---|---|---|---|---|---|
| Earth Brown | `--brand-secondary` | `#6F482A` | 111, 72, 42 | 0, 35, 62, 56 | Sampled | Primary button hover, dividers, secondary fills, stitched-patch borders. Body text on Bone |
| Clay | `--brand-accent` | `#D4B8A0` | 212, 184, 160 | 0, 13, 25, 17 | Sampled | Icons, borders and subtle highlights on dark |

### Neutral colors

| Name | Token | HEX | RGB | CMYK (approx.) | Use |
|---|---|---|---|---|---|
| Soil Black | `--bg-base`, also `--text-on-light` | `#120C06` | 18, 12, 6 | 0, 33, 67, 93 | Page background (dark-first). Text on Bone. Vehicle and garment base |
| Soil Surface | `--bg-surface` | `#20150C` | 32, 21, 12 | 0, 34, 62, 87 | Cards; alternating dark sections |
| Soil Elevated | `--bg-elevated` | `#2E1D10` | 46, 29, 16 | 0, 37, 65, 82 | Inputs on dark, raised cards, the sticky mobile call bar, badges |
| Bone | `--bg-light`, also `--text-primary` | `#F9F7F4` | 249, 247, 244 | 0, 1, 2, 2 | Text on dark. Light reading sections: the process, the FAQ, the estimate form |
| Bone Alt | `--bg-light-alt` | `#ECE1D8` | 236, 225, 216 | 0, 5, 8, 7 | Alternate light section; print paper tint |
| Dust | `--text-muted` | `#BFA89B` | 191, 168, 155 | 0, 12, 19, 25 | Secondary text and captions on dark |
| Dust Dark | `--text-muted-on-light` | `#5C5048` | 92, 80, 72 | 0, 13, 22, 64 | Secondary text on Bone; form field borders |

Borders in the token file: `--border-subtle` `rgba(212, 184, 160, 0.16)` (Clay at 16 percent, on dark) and `--border-subtle-light` `rgba(18, 12, 6, 0.10)` (Soil at 10 percent, on light).

### Semantic colors

UI states only. Never decorative, never a brand color, never a fill for a section.

| Purpose | Token | HEX | Use |
|---|---|---|---|
| Success | `--success` | `#22A06B` | A form's success state, on dark only. It is the one green in the token file, and it is not a brand color |
| Warning | `--warning` | `#E8A33D` | Warning text and icons on dark only. The `CONFIRM BEFORE PUBLISHING` badge |
| Error | `--error` | `#D9534F` | Error borders and icons. Error text on dark only |
| Info | none | none | There is no info color. A neutral notice is a Soil Elevated panel with Bone text and a Clay icon |

**A finding for the form (contrast checked 2026-10-15).** The estimate form sits on Bone, and all three status colors fail as text on Bone: error 3.71, success 3.11, warning 2.02. Default: on Bone, a field error is a 2 px Error border and an Error-colored icon (both pass the 3 to 1 non-text rule), with the message itself in Soil Black at weight 600. A success message on Bone is Soil Black text with a Success icon.

### Contrast (WCAG 2.1, by calculation)

AA body text needs 4.5. Large text (24 px and larger, or 19 px and larger if bold), icons, field borders and focus rings need 3.0.

**Pairs to use**

| Text or mark | Background | Ratio | Result and use |
|---|---|---|---|
| Bone | Soil Black | 18.17 | AAA. Everything |
| Bone | Soil Surface | 16.73 | AAA. Everything |
| Bone | Soil Elevated | 15.11 | AAA. Everything |
| Dust | Soil Black / Surface / Elevated | 8.59 / 7.91 / 7.15 | AAA. Body and secondary text |
| Clay | Soil Black / Surface / Elevated | 10.33 / 9.51 / 8.59 | AAA. Body, icons |
| White | Cattail Rust | 5.15 | AA. Button label |
| Bone | Cattail Rust | 4.82 | AA. The primary button label |
| Bone | Earth Brown | 7.45 | AAA. The primary button's hover label |
| Soil Black | Copper | 5.74 | AA. Phone button hover label; badges |
| Copper | Soil Black / Surface / Elevated | 5.74 / 5.28 / 4.77 | AA. Links, eyebrows, the phone ring and label on dark |
| Soil Black | Bone / Bone Alt | 18.17 / 15.11 | AAA. Everything on light |
| Dust Dark | Bone / Bone Alt | 7.28 / 6.06 | AAA / AA. Secondary text; field borders |
| Earth Brown | Bone / Bone Alt | 7.45 / 6.19 | AAA / AA. Body text and rules on light; eyebrows on light (Default) |
| Cattail Rust | Bone | 4.82 | AA. Links and body at 16 px or larger only |
| Copper | Bone | 3.17 | Large text and non-text only: step numerals at 24 px or larger, the focus ring |
| Cattail Rust button fill | Soil Black / Surface / Elevated | 3.77 / 3.47 / 3.14 | Non-text: the button's edge against the page |
| Warning | Soil Black / Surface / Elevated | 9.01 / 8.29 / 7.49 | AAA. Warning text and the badge, on dark |
| Success | Soil Black | 5.84 | AA. Success text on dark |
| Error | Soil Black / Surface | 4.90 / 4.51 | AA. Error text on dark |

**Pairs that fail and must not be used**

| Pair | Ratio | Rule |
|---|---|---|
| Earth Brown on Soil Black | 2.44 | Never as text on dark |
| Clay on Bone | 1.76 | Never as text, line or icon on light |
| Copper on Bone | 3.17 | Not for text under 24 px |
| Copper on Bone Alt | 2.63 | Never as text |
| White or Bone on Copper | 3.39 | Never. Copper holds Soil Black text only |
| Cattail Rust text on Bone Alt | 4.01 | Not for body or links. On Bone Alt sections, links are Soil Black with a Rust underline |
| Error / Success / Warning text on Bone | 3.71 / 3.11 / 2.02 | Never as text on light. See the form finding above |
| Error text on Soil Elevated | 4.08 | Not for text under 24 px |

### Color usage ratios

Share of the full scrolled page, photographs excluded. A check, not a formula.

| Color | Share | Where |
|---|---|---|
| Soil Black, Surface, Elevated | About 70 percent | Page ground, dark sections, cards, header, footer |
| Bone and Bone Alt | About 15 percent | Text on dark; the reading sections (process, FAQ, form) |
| Earth Brown and Clay | About 10 percent | Dividers, borders, icons, hover, patches |
| Cattail Rust and Copper | About 5 percent | The primary button, links, step numerals, rust rules |

### Color rules

- **One thing in rust.** The primary button is the rust thing on a screen. Copper numerals and a rust rule may sit with it; a second solid rust fill may not.
- **Never add** green, safety yellow, royal blue or any cool accent as a brand color. Status green is for form success only.
- **No gradients**, rust to copper included. Flat fills only. Texture comes from the emblem, the photographs and the soil grain.
- Copper is a color for dark grounds. On Bone it is a focus ring or a large numeral, never body text or a link.
- Color is never the only signal: links are underlined, errors have text and an icon, the current navigation item has an underline as well as a color.
- No black, champagne, gold or hi-vis yellow fields. No photo tints other than the Soil overlay.

---

## 3. Typography

Two families, both from Google Fonts under the SIL Open Font License. Font files are not bundled in this kit; both load from Google Fonts.

| Role in the template | Font | Weights | Use |
|---|---|---|---|
| Display typeface | **Graduate** | 400 only | Display, H1, H2, eyebrows, step numerals, badges |
| Heading typeface (H3 and down) | **Source Sans 3** | 700 | Card titles, FAQ questions |
| Body typeface | Source Sans 3 | 400 | Paragraphs, lead text, captions |
| Utility typeface | Source Sans 3 | 600, 700 | Buttons, navigation, labels, the phone line |

```css
--font-display: "Graduate", "Rockwell Extra Bold", "Rockwell", "Roboto Slab", "Arial Black", serif;
--font-display-weight: 400;
--font-body:    "Source Sans 3", system-ui, sans-serif;
```

**Graduate is a collegiate block slab,** the same varsity genre the "WRIGHT CO" lettering is drawn in, so headlines look as if they came from the emblem. No local competitor uses it.

- **It ships in one weight, 400, which already reads bold.** Load `family=Graduate` only; a request for `wght@700` errors. Always set `font-weight: 400` and `font-synthesis: none` so no browser fakes a bold.
- **It is wide.** Uppercase only, six to eight words at most, never more than two lines.
- **Never** for H3, buttons, navigation, form labels or paragraphs.

**Source Sans 3** is neutral and very legible on a phone in the sun, and supplies the weights Graduate lacks.

In Office, Canva or Google Docs without the brand fonts: headings in Rockwell Bold, falling back to Arial Black; body in Arial. Graduate is free, so send it with every print and vinyl job.

**Avoid:** Oswald or any condensed grotesk (a competitor's look); distressed or grunge fonts in running text; script or western novelty faces; thin or light weights; all-caps paragraphs; a third typeface.

### Type scale

Sizes from `tokens/css-tokens.css`. Pixel values are at a 16 px root; the clamp minimum is mobile, the maximum desktop.

| Role | Token | Font, weight | Desktop | Mobile | Line height | Case and tracking | Use |
|---|---|---|---:|---:|---:|---|---|
| Display | `--text-display: clamp(2rem, 6vw, 3.25rem)` | Graduate 400 | 52 px | 32 px | 1.1 | Upper, 0 | Hero line only |
| H1 | `--text-h1: clamp(1.75rem, 4.5vw, 2.5rem)` | Graduate 400 | 40 px | 28 px | 1.1 | Upper, 0 | Page title, one per page |
| H2 | `--text-h2: clamp(1.375rem, 3vw, 1.875rem)` | Graduate 400 | 30 px | 22 px | 1.1 | Upper, +0.01em | Section heads |
| Step numerals, badges | none | Graduate 400 | 2 to 4 × body | 2 to 4 × body | 1 | Numerals | "01 CLEAR · 02 DRIVEWAY · 03 PAD · 04 FOUNDATION DIG" |
| Eyebrow | none (0.875rem) | Graduate 400 | 14 px | 14 px | 1.3 | Upper, +0.08em | Small label above an H2. Copper on dark; Earth Brown on Bone (Default) |
| H3 | `--text-h3: 1.5rem` | Source Sans 3 700 | 24 px | 24 px | 1.25 (Default) | Title case | Card titles, FAQ questions |
| Lead | none (1.25rem) | Source Sans 3 400 | 20 px | 20 px | 1.6 | Sentence | Intro under a heading |
| Body | `--text-base: 1.125rem` | Source Sans 3 400 | 18 px | 18 px | 1.6 | Sentence | Paragraphs |
| Button, nav | none (1rem) | Source Sans 3 700 | 16 px | 16 px | 1.2 | Upper, +0.06em | Buttons, menu |
| Small, caption | `--text-small: 0.875rem` | Source Sans 3 400 or 600 | 14 px | 14 px | 1.5 (Default) | Sentence | Photo captions, form hints. Dust on dark |
| Phone line | none | Source Sans 3 700 | Context | Context | 1.2 | Tabular figures | Header, footer, signs, trucks |

The token file holds two line heights, `--leading-heading: 1.1` and `--leading-body: 1.6`. Lead (1.25rem), the eyebrow size and tracking, and the button size are in the style guide but are not tokens yet.

### Type rules

- Display, H1 and H2 are Bone on dark and Soil Black on Bone. Body is Bone on dark, Soil Black on Bone.
- Write source text in sentence case. CSS uppercases display type and buttons. Offer names are proper nouns: the Homeplace Package, the Free Lot Walk, The Dirt Order.
- Line length 60 to 75 characters. Left aligned. Center only a short hero line or a standalone call to action. No justified text.
- No italics for emphasis; use weight 600 or 700.
- Body text is 18 px. Nothing on the website is below 14 px.
- Numbers in tables and phone lines use tabular figures.
- Social graphic (1080 × 1350), Default: Graduate headline at 72 to 96 px, uppercase, two lines and eight words at most; support line Source Sans 3 400 at 40 to 44 px; label Graduate at 28 to 30 px, uppercase, +0.08em. Smallest text 36 px. Margins 80 px. Do not shrink web sizes into a graphic.
- Print: headings Graduate 32 to 40 pt on slides and one-sheets; body Source Sans 3 at 18 pt minimum on slides, 10 pt minimum on paper.

---

## 4. Spacing system

Base unit 8 px. Six steps and nothing between.

| Token | Value | Use |
|---|---:|---|
| `--space-1` | 8px | Between a label and its field; tight internal spacing |
| `--space-2` | 16px | Between related items; mobile side margin; the gap between the two CTA buttons |
| `--space-3` | 32px | Between groups; card padding; desktop gutter |
| `--space-4` | 64px | Section padding on mobile and tablet |
| `--space-5` | 96px | Section padding on desktop |
| `--space-6` | 128px | The hero and the closing call-to-action band only |

## 5. Border radius

Angular. No pill shapes anywhere.

| Token | Value | Use |
|---|---:|---|
| `--radius-sm` | 2px | Buttons, inputs, text badges |
| `--radius-md` | 4px | Cards (or a chamfered corner instead) |
| `--radius-lg` | 8px | Large media, the photo slots |

The **chamfer** is the brand's alternative to a rounded corner: an 8 to 12 px 45° cut, on badges, sequence cards and the top-right corner of service cards. Full-bleed images are square-cornered. Modals are not specified; use 8 px if one is needed (Default).

## 6. Borders

| Border | Value | When used |
|---|---|---|
| Hairline, dark | 1 px `--border-subtle`, Clay at 16 percent | Card edges and dividers on Soil |
| Hairline, light | 1 px `--border-subtle-light`, Soil at 10 percent | Dividers and table rules on Bone. Never the only edge of a form field |
| Form field | 1 px Dust Dark `#5C5048` | Every input, select and text area on Bone |
| Form field, focus | 2 px Cattail Rust | The field in use |
| Form field, error | 2 px Error `#D9534F`, with an icon and a Soil Black message | A field that needs fixing |
| Phone button ring | 2 px Copper on dark; 2 px Soil Black on Bone | The outlined secondary button |
| Rust rule | 3 to 4 px solid Cattail Rust | Under an H2, in the footer, as the before/after divider |
| Stitched-patch frame | Earth Brown border with a dashed inner rule | Badges, the service-area tag, review cards once real reviews exist |

Sections are separated by a change of ground (Soil to Soil Surface, Soil to Bone), not by a line. No waves, torn edges or ornamental rules.

## 7. Shadows

**None.** The sources specify no shadow. Cards carry a hairline and no shadow; nothing glows. The phone button's ring may be built with an inset `box-shadow` in CSS, which renders as a border, not a shadow. The token file has no shadow token.

| Template slot | Value |
|---|---|
| Small | none |
| Medium | none |
| Large | none |

## 8. Layout rules

| | Mobile (under 640 px) | Tablet (640 to 1023 px) | Desktop (1024 px and up) |
|---|---|---|---|
| Columns (Default) | 4 | 8 | 12 |
| Gutter | 16 px | 16 px | 32 px |
| Side margin | 16 px | 32 px | 32 px, content capped at 1200 px |
| Text column | Full width | 60 to 75 characters | 60 to 75 characters |
| Section padding, top and bottom | 64 px | 64 px | 96 px; 128 px for the hero and the closing band |

- Maximum content width: `--container: 1200px`. Minimum tap target 44 px; buttons 52 px tall.
- Design at 360 px wide first. No sideways scrolling at 320 px wide or at 200 percent zoom.
- **Dark-first.** Soil Black is the page. Dark sections alternate Soil Black and Soil Surface. Long reading (the process, the FAQ, the estimate form) sits in Bone sections.
- **Every page follows one order:** outcome line, who it's for, the sequence, what drives the price, one proof (only if real), one call-to-action pair.
- Each section opens the same way: optional eyebrow, H2 with a rust rule under it, optional lead. Then one kind of content.
- No carousel that moves by itself. No pop-ups, countdowns or counters.
- **Header:** Soil Black bar. Wordmark left (see section 1 until it exists). Navigation in Source Sans 3 700, uppercase, Bone. The outlined phone button at right, and "Book a Free Lot Walk" as the solid button. Services are ordered by the sequence (01 to 04), not alphabetically. In a narrow header the phone button may read "Call or Text" with the number in its link.
- **Mobile call bar:** fixed to the bottom, Soil Elevated, the two buttons at equal width (Lot Walk solid, Call or Text outlined).
- **Hero:** Soil ground. Eyebrow "Serving Hammond, Tangipahoa Parish & the Northshore". Graduate display line. Source Sans lead. The button pair. A trust strip of safe facts only: "Free estimates · Clearing and excavating since 2022". No badges. No job photo until a real one exists: the hero is type-led, with the emblem, the sequence and soil texture.
- **Sequence band:** directly under the hero. Four chamfered cards, Copper Graduate numerals, an icon, one line each, each linking to its service page.
- **Footer:** Soil Black. The emblem (no phone, once it exists) at 240 px or larger, then "© 2026 Wright Co. · Land clearing, driveways & house pads · Serving Hammond, Tangipahoa Parish & the Northshore · 360-957-5865 · wrightco504@gmail.com", and the microline "Clearing and excavating since 2022." No street address, no "LLC", no hours until confirmed.
- The emblem appears once large per screen: in the hero or the footer, never both in one view.

## 9. Cards

| Property | Value |
|---|---|
| Background | Soil Surface on a Soil Black section; Soil Elevated on a Soil Surface section; white is never used |
| Border | 1 px `--border-subtle` |
| Radius | 4 px (`--radius-md`), or a chamfered top-right corner |
| Shadow | None |
| Internal padding | 32 px |
| Header treatment | Icon, then H3 in Source Sans 3 700, Bone |
| Hover behavior | Not specified. Default: none on the card; the Copper link inside it underlines. No lift, no shadow |

Card types:

- **Sequence card.** Chamfered. A Copper Graduate numeral (01, 02, 03, 04), a filled icon in Clay, the step name, one line. Same words, same order, every time.
- **Service card.** Soil Surface, Clay hairline, 4 px radius or chamfered top-right. Icon, H3, two lines of body in Dust or Bone, a Copper text link.
- **Offer band.** The Homeplace Package, always with its descriptor: "Clear · Driveway · House Pad. One crew, one scope, build-ready." A stitched-patch badge with the offer name is allowed; no separate logo.
- **Badge.** Stitched-patch style: Graduate uppercase, Copper on Soil Elevated, Earth Brown border with a dashed inner rule, chamfered corners.
- **Review card.** Not built. No review is approved (file 5). When real Louisiana reviews exist: stitched-patch frame, the quote verbatim, the customer's first name and last initial, no stars.
- **Neutral notice.** A Soil Elevated panel, Bone text, a Clay icon.
- **Photo slot.** See file 8.

## 10. Buttons

All buttons: Source Sans 3 700 at 16 px, uppercase, +0.06em tracking, line height 1.2, at least 52 px tall, 16 px top and bottom and 28 px left and right padding, 2 px radius, centered text, no full stop. **The two labels are fixed:** "Book a Free Lot Walk" and "Call or Text 360-957-5865". CSS sets them in capitals.

### Primary: "Book a Free Lot Walk"

- Background: Cattail Rust `#A15C27`
- Text: Bone `#F9F7F4` (4.82 to 1)
- Border: none
- Radius: 2 px
- Hover: Earth Brown `#6F482A` fill (Bone label 7.45 to 1)
- Press: Earth Brown (Default; the sources give hover only)
- Focus: 3 px Copper outline, 2 px offset
- Disabled: not specified. Default: avoid disabled buttons; if one is unavoidable, Dust text on Soil Elevated with the reason in text beside it

### Secondary: "Call or Text 360-957-5865"

**A button, not a text link.** Linked `tel:+13609575865`.

- On dark: transparent fill, 2 px Copper ring, Bone label, a phone icon at left
- On Bone: transparent fill, 2 px Soil Black ring, Soil Black label
- Hover: Copper fill, Soil Black label (5.74 to 1)
- Press: as hover (Default)
- Focus: 3 px Copper outline, 2 px offset

### Text link

- Copper on dark; Cattail Rust on Bone; Soil Black with a Rust underline on Bone Alt
- Underline: always
- Hover: not specified. Default: the underline thickens to 2 px

### The pair

- Primary first and solid; phone second and outlined.
- **Equal width.** A column flex group, `align-items: stretch`, capped at 520 px. Side by side from 640 px only if both stay equal (`flex: 1 1 0`). Stacked on mobile.
- One pair per view. A second "Book a Free Lot Walk" on the same screen is a text link.
- Never a Copper fill as a resting button. Never a pill. Never a rounded button.
- Focus is never removed.

```css
.wc-cta { display:flex; flex-direction:column; align-items:stretch; gap:var(--space-2); max-width:520px; }
@media (min-width:640px){ .wc-cta--row { flex-direction:row; } .wc-cta--row > * { flex:1 1 0; } }
.wc-btn { min-height:52px; padding:16px 28px; border-radius:var(--radius-sm); font:700 1rem/1.2 var(--font-body);
          text-transform:uppercase; letter-spacing:.06em; text-align:center; text-decoration:none; }
.wc-btn--primary { background:var(--brand-primary); color:var(--bg-light); }
.wc-btn--primary:hover { background:var(--brand-secondary); }
.wc-btn--phone { background:transparent; color:var(--text-primary); box-shadow:inset 0 0 0 2px var(--brand-primary-bright); }
.wc-btn--phone:hover { background:var(--brand-primary-bright); color:var(--bg-base); }
.wc-section--light .wc-btn--phone { color:var(--text-on-light); box-shadow:inset 0 0 0 2px var(--text-on-light); }
.wc-btn:focus-visible { outline:3px solid var(--brand-primary-bright); outline-offset:2px; }
```

The `wc-` prefix is a suggestion until the site's CSS prefix is set.

### Form fields

The estimate form sits in a Bone section. One column on every screen size. Labels above the field, always visible, 18 px Source Sans 3 600, Soil Black. Fields 52 px tall, text at 18 px, Bone fill, 1 px Dust Dark border, 2 px radius. Focus: 2 px Cattail Rust border. Hints beneath in Small, Dust Dark. Errors: see section 2. Optional fields are marked "(optional)" in words. The submit button is the primary button at full width. **The form must actually submit.**

## 11. Iconography

**Primary icon system:** Phosphor (Fill) or Tabler (filled) is proposed. Open licenses. No icon files are bundled in this kit. Pick one set, record it and its license, and keep to it.

- Style: solid filled glyphs with square ends and mitred corners, or a stroke of 2 px or more with square caps. No rounded, bubbly or duotone sets.
- Default size: 24 px beside text, 20 px inside a button, 32 px on cards, 48 px at most on a page; 96 px on a social slide (Default).
- Approved colors: Clay or Copper on dark; Soil Black on Bone.
- Emoji: none on the website, in graphics, in headings or on buttons.
- An icon always has a text label. The phone icon never stands in for the number.
- Never a machine as the identity: no excavator arm, dozer or tree silhouette as a logo-like device, no shield, no arched badge.

Icons needed:

| Group | Icons |
|---|---|
| The sequence | tree (clear), stump, driveway or culvert, house pad (a stepped mound), shovel or dig (foundation) |
| Add-ons | pond or water, drainage arrow, dump truck, gravel pile |
| The visit | stake or flag (the lot walk), boots or footprints, map pin (a town, never an address) |
| Contact | phone, message (text), mail |
| Proof | camera (photo credit), check |
| Interface | menu, close, chevron down, arrow right, plus and minus (FAQ), alert (error), info |

The map pin never marks a home or a business address.

## 12. Photography

### What exists

**Nothing.** There are no photographs of Wright Co. work in Louisiana. `assets/photos/PHOTO-MANIFEST.md` lists zero files. Every layout that needs a picture uses a labelled photo slot (file 8). Photos from the owner's Washington business are never used.

### Overall style (for when photos arrive)

Raw documentary. Honest, worked-in, shot on a phone by the crew if that is what exists. Not drone glamour, not stock.

### Subjects, in order of value

1. **The hero asset:** a before, during and after series of one lot from the same spot. Mark a phone position (a stake or a fence post) and shoot woods, cleared and stumped, driveway cut in, pad built.
2. The finished pad with the builder's stakes.
3. A culvert at the drive; gravel being spread.
4. A stump coming out; the mulcher or machine working the ground (the ground in frame, not the machine alone).
5. A pond holding water; drainage running.
6. People in work gear working; Cody walking a lot with a landowner, with permission.
7. Short vertical video, 10 to 30 seconds: brush going down, a pad being rolled, a time-lapse from the fixed spot.

### Lighting and color grade

Daylight as found. One preset on everything: warm and slightly desaturated, greens pulled down 15 to 20 percent so pine and brush sit back toward the palette, shadows lifted a touch, red clay and soil kept true. No heavy HDR, no filters beyond the preset.

### Composition

- Show the ground, not the gear. The lot and the result fill the frame.
- Ratios: 4 to 5 (mobile hero, social), 1 to 1 (cards), 16 to 9 (wide slots, the before/after split). Nothing else (Default).
- Corners: 8 px for media in the layout, square when full-bleed.
- Type on a photo only under a 60 to 75 percent Soil overlay.

### Captions

Every job photo names **the town and the work**, in Source Sans 3 Small, Dust on dark. Format: "Independence · 3 ac cleared · 300 ft drive · pad" (a format example only, not a real job). Never a client's name without permission. Never an invented number.

### Authenticity

Use: real Louisiana Wright Co. jobs only, from `assets/photos/` once they exist.

Avoid:

- Stock photographs of any kind: "worker with clipboard", yellow-excavator stock, transparent machine cut-outs.
- AI-generated or illustrated lots, machines, crews, landowners, houses or landscapes.
- Golden-hour forest heroes.
- Other companies' equipment or logos.
- Photographs from the owner's Washington business, captioned or not.
- Cartoon bayou, gator or crawfish clichés.

### What is retired

| Retired | Replaced by |
|---|---|
| "Built on Hard Work. Driven by Quality." as the hero | "You bought the land. We'll get it ready to build." |
| The emblem with the phone banner on the website and new print | The phone-free emblem once drawn; the phone set in type |
| Oswald and the earlier type pairing | Graduate and Source Sans 3 |
| A grid of unrelated service tiles | The numbered sequence |
| 6 / 12 / 20 px radii | 2 / 4 / 8 px |

## 13. Illustration and generated visuals

There is no illustration style and no mascot. The only permitted non-photographic graphics are built from the tokens: flat fields, the numbered sequence, rust rules, stitched-patch frames, chamfered shapes, the soil grain and contour lines, and an icon-based sequence diagram. File 8 has the rule in full.

## 14. Backgrounds

- **Solid:** Soil Black, Soil Surface and Soil Elevated as dark grounds; Bone and Bone Alt as light grounds.
- **Gradient:** none.
- **Soil grain:** a noise or speckle overlay at 6 percent opacity or less, on dark sections only. Never on Bone, never behind body text at higher opacity. Built in code or as a vector or noise layer, not generated imagery.
- **Topographic contour lines:** Clay at 8 to 10 percent opacity, as an occasional section background on dark. At most one per page.
- **Photography:** behind text only under a 60 to 75 percent Soil overlay. None exists yet.
- **Pattern, texture:** none beyond the two above.
- **Full bleed:** the hero, the closing call-to-action band, the footer, the before/after split.

## 15. The numbered sequence

The one graphic device that is this company's own, taken from the owner's description of the work.

| Rule | Value |
|---|---|
| What it is | Four steps, always the same words in the same order: **01 Clear · 02 Driveway · 03 Pad · 04 Foundation Dig** |
| Type | Graduate, uppercase, Copper numerals on dark |
| Forms | A strip of text (hero, footer, social), four chamfered cards (the sequence band), a numbered list (estimates, The Dirt Order) |
| Arrow form | "clear → driveway → pad" in running text and captions |
| Never | Re-ordered, renamed, shortened differently on different pieces, or mixed with add-ons (ponds, hauling) |

The style guide also shows "01 CLEAR · 02 DRIVE · 03 PAD" in one place. Use "DRIVEWAY" everywhere.

## 16. Motion

The sources specify no motion. Everything below is a restrained default, consistent with the brand's heavy, plain character.

| Item | Value | Source |
|---|---|---|
| Default transition duration | 150 ms | Default |
| Reduced motion | Every transition removed under `prefers-reduced-motion` | Default |
| Autoplay | None. No autoplay video, no carousel that moves by itself | Default |
| Easing | `ease-out` | Default |
| Hover | A fill or color change only: primary to Earth Brown, phone to Copper fill, links underline | Style guide for the values |
| Press | The hover state held. No scale, no bounce | Default |
| Focus | The 3 px Copper ring appears at once | Default |
| Entrance animation | None | Default |
| Avoid | Bounce, parallax, scroll-triggered reveals, counters that count up, sliding carousels | Default |

In video, cuts are plain. No logo sting is specified, and none is designed here.
