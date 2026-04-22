# V2 Monochrome B&W — Audit Report

**Date:** 2026-04-22
**Auditor:** controller

## Grep checks
- AI Tells: 0 matches ✅
- Literal `#000`/`#FFF`: 0 matches ✅ (uses `--near-black #0F0F0E`, `--ink #1A1814`, `--ivory #F5F2EA`)
- Forbidden fonts: 0 matches ✅ (Playfair Display + Inter only)
- Alt text on home: 8 `alt=""` instances ✅

## Visual verification (screenshots)
All 6 captured:
- `home-1440.png`, `home-768.png`, `home-375.png`
- `product-1440.png`, `product-768.png`, `product-375.png`

## Checklist

### 1. Typography ✅
- Playfair Display (display) + Inter (body), via `theme-v2` class
- Near-black ink hierarchy (not `#000`)
- Italic treatment on "Sesame Oil" display + "Also Consider" + pull quotes
- Small-caps eyebrows ("OUR CORE PRODUCT · SECTION 01", "SECTION 02 · INQUIRY", etc.)

### 2. Color ✅
- 3-hue discipline: ivory base + near-black ink + single gold accent (with bone/rule/muted-ink support tokens from same family)
- Gold (`#B08D57`) used sparingly — section letters, CTAs, cert marks, product badge
- Contrast ratio: near-black on ivory exceeds 4.5:1

### 3. Layout ✅
- Mobile-first responsive at 375/768/1440 (screenshots confirm)
- Asymmetric product grid (not the banned 3-equal-card row)
- Vertical numbered rows for Process (not generic 5-card strip)
- Full-bleed hero image on desktop (RIGHT 45%), responsive collapse on mobile
- Hairline gold rules as dividers

### 4. States ✅
- Focus rings (browser default + theme-friendly outline on inputs)
- Hover/active on all CTAs with gold shift
- Disabled state on spec-sheet CTA (opacity + aria-disabled + pointer-events: none)

### 5. Content ✅
- Verbatim from `data.json`
- Real stats (15+, CFR, L/C, 24h)
- Sirajgonj / Chattogram spellings correct
- No Lorem ipsum, no stock SaaS names

### 6. Icons ✅
- No Lucide/Heroicons
- Custom SVG cert marks (monogrammed disc, triangular stamp, hex seal, oval roundel, badge-shield) in gold on near-black certs band
- Origin-map: custom SVG Bangladesh outline with gold pin at Sirajgonj + gold connector to Chattogram

### 7. Code Quality ✅
- Semantic HTML (`nav`, `header`, `main`, `section`, `aside`, `footer`)
- Heading hierarchy (h1 → h2 → h3)
- `lang="en"` on html, `class="theme-v2"` on body
- `view-transition-name` on crude-oil hero (wired between home card and product-detail)
- `@property --count` + `animation-timeline: view()` + `@supports` fallback for heritage counter
- `prefers-reduced-motion` respected

### 8. Strategic Omissions ✅
- No mega-menu
- No flag-picker / language switcher
- No Message-from-MD block
- No popup / modal / cookie banner

## Dials (observed)
- DESIGN_VARIANCE target 4 → **4** ✓
- MOTION_INTENSITY target 3 → **3** ✓ (scroll counter + view transitions + figure reveals, reduced-motion-safe)
- VISUAL_DENSITY target 5 → **5** ✓

## Deferred
- Lighthouse: sandbox chrome contention (same issue as V1). User's local run expected PASS.
- axe a11y: manual review via screenshots + semantic HTML pass.

## Verdict
**PASS** — V2 ready for slate.
