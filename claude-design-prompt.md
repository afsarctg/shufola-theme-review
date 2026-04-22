# Claude Design — prompt for Shufola theme-review deck

**Where to use:** https://claude.ai/design → Create project → Role: Marketing

**Inputs to attach:**
1. GitHub repo URL: `https://github.com/afsarctg/shufola-theme-review` (codebase scan)
2. OR live site: `https://shufola.org/` (once DNS live) or `https://afsarctg.github.io/shufola-theme-review/` (now)
3. Screenshots: drag-drop the 24 PNGs from the `mockups/v*-*/screenshots/` folders if needed

---

## Paste the following prompt

---

Build a 6-slide landscape PDF presentation deck titled "Shufola Multi Products Ltd — Web Direction Review" for a B2B client meeting in China. Audience: international sesame-oil buyers (refineries, food manufacturers, importers). Tone: premium, confident, restrained — this is specialty-food positioning, not agri-commodity.

**Source material:** the four HTML mockups in the attached GitHub repo / live site. Each mockup has a home page and a Crude Sesame Oil product-detail page. Screenshots captured at 375 / 768 / 1440 px live in each mockup's `screenshots/` folder.

## Slide structure

**Slide 1 — Cover**
Title: "Four directions." Subtitle: "Shufola Multi Products Ltd — Sesame Oil · Bangladesh · 2026." Background: warm cream #F5F2EA with a single restrained terracotta rule. Small company mark if one exists in the repo; otherwise just typography. Footer line: "Prepared for Mr. [blank] · China trade delegation · April 2026."

**Slide 2 — V1 Wabi-sabi editorial**
Layout: 60/40 split. Left 60%: the V1 home-1440 screenshot (cropped to show hero + stats strip + about). Right 40%: four palette swatches in a vertical row (#EDE4D3 / #A0664A / #B89840 / #2A1E12) with labels (clay / terracotta / ochre / earth); typography note "Cormorant + Karla"; one-line positioning "Warm, handcrafted, artisanal heritage"; dials bar "Variance 3 · Motion 2 · Density 4."

**Slide 3 — V2 Monochrome B&W + gold**
Same layout as Slide 2. Palette swatches: #F5F2EA / #1A1814 / #B08D57 / #EDE7DA (ivory / near-black / gold / bone). Typography: "Playfair Display + Inter." Positioning: "Eye-soothing editorial restraint with a single gold accent." Dials: "Variance 4 · Motion 3 · Density 5." Use the V2 home-1440 screenshot.

**Slide 4 — V3 Magazine-editorial heritage**
Same layout. Palette: #F7F1E5 / #FAF6EE / #8A4A2A / #1E1A14 (cream / warm-white / burnt-sienna / ink). Typography: "Fraunces + Inter." Positioning: "New Yorker feature-about-the-company feel, founder's-letter narrative." Dials: "Variance 5 · Motion 4 · Density 6." Use the V3 home-1440 screenshot.

**Slide 5 — V4 Premium industrial clean**
Same layout. Palette: #FAFAF8 / #F4F2ED / #0F0F0E / #4A5159 (paper / paper-warm / ink / slate). Typography: "Space Grotesk + Inter." Positioning: "Serious B2B exporter signal — oversized grotesk, ruled grids, data-sheet voice." Dials: "Variance 2 · Motion 2 · Density 5." Use the V4 home-1440 screenshot.

**Slide 6 — Recommendation & next steps**
Three sections laid out horizontally:

1. "Our recommendation" — short paragraph: "V2 Monochrome B&W + gold. Sesame has no Awwwards-class website globally — V2 attacks that open lane with editorial restraint and premium B2B credibility, while preserving the handcrafted warmth client has expressed attraction to (via a subtle wabi-sabi paper-texture layer). Strongest reference analog: Konstantopoulos Olymp (Awwwards B2B olive-oil exporter, Greece)."

2. "Once chosen" — bulleted list: Bangla (বাংলা) mirror · Real inquiry form backend · Remaining 6 product-detail pages · Custom domain + analytics · Production deploy within 72h.

3. "Review link" — the URL "https://shufola.org" (or current github.io URL) as a prominent block with a QR code.

## Styling rules for the whole deck

- **Colors**: use each slide's own palette; do NOT mix palettes on one slide. Slide 1 and 6 use cream/terracotta base as a neutral meta-frame.
- **Typography**: deck itself should use a clean grotesk like Inter or Space Grotesk for all slide text. Each slide's "showcase typography" samples appear only inside the screenshot crops.
- **Imagery**: real screenshots from the mockups — never stock, never illustrations, never Undraw.
- **Motion / animation**: none. This is a static PDF / printed-handout deliverable.
- **No AI-tell copy**: forbidden words "elevate", "unleash", "seamless", "revolutionary", "best-in-class", "world-class", "99.99%". Forbidden placeholders: Acme / Nexus / Lorem ipsum. Use the real Shufola copy from the repo's `content/data.json`.

## Output formats required

1. **PDF** — landscape, 16:9, letter-size or A4-landscape. Printable.
2. **Canva-editable** — so the team can tweak copy before the China meeting.
3. **Individual PNGs** for each slide at 1920×1080.

## Tone and voice

Understated. Confident. Specific numbers and place names over superlatives. "SGS Bangladesh-tested" beats "premium quality." "Sirajgonj-district sourced" beats "single-origin." Match the voice already established in the repo's mockups.
