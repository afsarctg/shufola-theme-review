# V2 Monochrome B&W — VERIFIED

**Date:** 2026-04-22
**Verified by:** controller

## Files
- `home.html` — 1605 lines
- `products/crude-sesame-oil.html` — 774 lines
- `dials.md`
- `audit-report.md`
- `screenshots/` — 6 PNGs
- `lighthouse.json` — deferred (sandbox)

## Gates
| Check | Result |
|---|---|
| 6/6 screenshots | ✅ |
| HTTP 200 both pages | ✅ |
| AI Tells: 0 | ✅ |
| #000/#FFF: 0 | ✅ |
| Forbidden fonts: 0 | ✅ |
| Alt text | ✅ |
| Dials 4/3/5 | ✅ |
| Lighthouse ≥90 | ⏸ deferred |

## Signature moves delivered
- Roman numeral section spine (I-V across home; I./II./III./IV. on product-detail Related)
- Editorial split-screen hero (55/45 text-L / full-bleed B&W photo-R)
- Scroll-driven heritage counter via `@property --count` + `animation-timeline: view()` with static fallback
- `view-transition-name: crude-oil-hero` wired between home product card and product-detail hero
- Gold accent single-channel (section letters, CTAs, cert marks, core-product badge, hairline rules)
- B&W photo filters: `.photo-bw` (pure grayscale) + `.photo-bw-warm` (sepia 0.07 for documentary warmth)
- Dark near-black certs band with 5 custom gold SVG marks + Playfair italic separator
- Drop-cap on product-detail narrative first paragraph

## Next
V3 Magazine-editorial heritage.
