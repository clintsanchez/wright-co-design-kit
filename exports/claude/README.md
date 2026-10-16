# Claude exports (source files)

**Status: proposal v0.1, 2026-10-15. Not yet approved by the owner.** Every item marked "Confirm before publishing" stays unconfirmed until file 6 is updated.

These are the source files for three artifacts Claude built from this kit:

| Folder | What it is |
| --- | --- |
| `design-system/` | Wright Co. design system: tokens, README, Button and Cover components, Logos and Photos notes |
| `social-templates/` | Social template library: 43 artboards (feed, Google, stories, carousels, covers, video) plus `canvas.json` |
| `brand-kit/` | Comprehensive brand kit: 32 US Letter pages (816×1056) and 3 website mockups (Home, Land Clearing, The Homeplace Package) plus `canvas.json` |

## Read before using

- The `.dc.html` files render only inside Claude's design canvas, because they use its runtime (`sc-for`, `sc-if`, `{{ }}` holes). Opening them directly in a browser will not show the finished layout.
- Images are referenced as `/_blob/<id>`. Those are Claude-hosted copies of the emblem files in `assets/`; they are not included here.
- The brand kit PDF, when added, goes in `exports/` next to this folder.
- No photographs are used anywhere. Every photo position is a "Real job photo:" slot.
