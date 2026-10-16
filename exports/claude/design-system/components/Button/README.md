# Button

The Lot Walk / Call or Text button pair: the only two buttons Wright Co. uses, set side by side at equal width with the solid primary first.

Hand-written from `3 - Visual Identity.md` §10; the CSS is the source's own, in `components/bundle.css`.

**The consumer supplies** plain markup: a `div.wc-cta` (add `wc-cta--row` for side by side from 640px) holding two links, `a.wc-btn.wc-btn--primary` and `a.wc-btn.wc-btn--phone` with `href="tel:+13609575865"`. On a Bone section, put the pair inside `.wc-section--light` so the phone ring turns `text-on-light`.

**Labels are fixed:** "Book a Free Lot Walk" and "Call or Text 360-957-5865" (CSS uppercases them; no full stop). In a narrow header the phone button may read "Call or Text" with the number in its link.

- Primary: `brand-primary` fill, `bg-light` label (4.82:1); hover `brand-secondary` (7.45:1).
- Phone: transparent, 2px inset `brand-primary-bright` ring, `text-primary` label, phone icon at left on dark; hover fills `brand-primary-bright` with a `bg-base` label (5.74:1). On Bone: 2px `text-on-light` ring and label.
- The phone glyph in the preview is a placeholder until an icon set (Phosphor Fill or Tabler filled, proposed) is chosen.
- Focus: 3px `brand-primary-bright` outline, 2px offset, never removed. Press holds the hover state.
- 52px minimum height, 16px × 28px padding, `radius-sm`, capped at 520px wide as a pair, stacked on mobile.

**Don't:** use a pill or rounded button, a Copper resting fill, a second solid Lot Walk button on the same screen (make it a text link), the phone as a bare link, or a disabled button (if unavoidable: `text-muted` on `bg-elevated` with the reason beside it).
