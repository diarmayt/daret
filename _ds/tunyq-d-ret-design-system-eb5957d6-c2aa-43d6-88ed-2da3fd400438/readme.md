# Tunyq — DÄRET Design System

**DÄRET by SAUAPKER** makes portable touchless dispensers for ritual ablution (wudu). One 420 ml device performs a complete wudu anywhere — in the car, at the office, in transit — using a fraction of the water a tap or bottle wastes. Kazakhstan-made, built for people who keep their prayers on time without leaving a mess behind.

**Tunyq** (Kazakh «тұнық» — clear, still water) is the brand's design system: deep petrol green on white and wheat straw, generous whitespace, soft droplet geometry. Calm and understated — the quiet dignity of the ritual. Never religious kitsch, never gadget hype.

## Sources
- 13 uploaded brand files (product renders, backgrounds, logo SVG) — see `assets/`; those files are the originals. Only the raw logo trace is kept separately in `uploads/`.
- Brand brief (palette, type, tone) supplied in chat. No Figma, no codebase — components below are authored from the brief and renders, not recreated from a source library.

## Products
One physical product in two finishes: **DÄRET White** (pure white shell) and **DÄRET Straw** (speckled wheat-straw composite). Both: 420 ml tank, IR hand sensor, chrome trim rings, dark top display disc. Surfaces represented here: the **marketing site** (`ui_kits/site/`).

## CONTENT FUNDAMENTALS
- **Voice:** calm, factual, dignified. Speak plainly about the ritual (wudu, ablution) with respect; never preachy, never novelty-gadget hype ("revolutionary!", "game-changer") and no religious ornamentation in copy.
- **Person:** "you" for the reader, "DÄRET" (not "we") for the product where possible. Imperatives are gentle: "Perform a complete wudu anywhere."
- **Casing:** sentence case everywhere. UPPERCASE reserved for the wordmark, eyebrow labels, and buttons (Montserrat, tracked wide).
- **Wordmark:** always "DÄRET" (with umlaut), sub-line "by SAUAPKER". System name "Tunyq".
- **Numbers are the argument:** water saved, 420 ml, minutes — state them quietly and precisely ("One fill. A complete wudu. ~0.4 L of water."). No exclamation marks.
- **Emoji:** never.
- **Languages:** default English; brand is Kazakh — Kazakh/Russian strings may appear in real usage; keep layouts tolerant of longer strings.
- Example hero: eyebrow "PORTABLE WUDU" · h1 "Clear water, wherever prayer finds you." · body "One 420 ml fill performs a complete ablution — in the car, at the office, in transit."

## VISUAL FOUNDATIONS
- **Palette:** deep petrol `#0B3D3A` on white `#FFFFFF`; wheat straw `#DCCFB6` and mist aqua `#E8F1EF` as quiet surface tints; chrome silver `#C9CDD1` for hardware accents/hairlines; ink charcoal `#1A1F1E` body text. Petrol is the only "loud" color — used for headings, buttons, and one inverse band per page. Max two background colors per composition.
- **Type:** Montserrat 600 for headings/buttons/labels with letter-spacing `0.04em` (+40); uppercase eyebrows tracked `0.14em`. Inter 400/500 body, line-height 1.6. Headings in petrol, body in ink, muted at 60% ink.
- **Spacing:** generous — 8px base scale up to 128px; sections breathe (96–128px vertical). Whitespace is a brand feature, not a gap.
- **Geometry:** soft droplet radii — cards 24–32px, pills for buttons/badges, signature `--radius-droplet` (32/32/32/8) putting one quiet corner on imagery and feature cards.
- **Backgrounds:** mostly flat white or mist aqua; one full-bleed petrol band per page (use `assets/bg-petrol-gradient-1920.webp` — dark petrol water gradient) for the "quiet statement" moment; `assets/bg-water-ripples-1920.webp` (near-white ripples) as a subtle hero texture. Straw tint `--surface-warm` for the Straw-finish story. No purple gradients, no patterns.
- **Imagery:** studio product renders on travertine/mist backdrops; cool, airy, high-key; water rendered as clear glassy streams. People appear only as hands. Warm straw tones balance the cool aqua. No grain, no B&W.
- **Motion:** still water — opacity/transform fades, 160–320ms, `--ease-calm`; no bounces, no springs.
- **Hover:** darken petrol slightly (`--accent-hover`), or lift card shadow `--shadow-card → --shadow-float`; links darken. **Press:** darker still (`--accent-pressed`), no shrink transforms.
- **Borders:** 1px hairlines in `--border-subtle` (petrol at 12%) or silver; cards prefer shadow + hairline over heavy borders. Chrome silver appears as thin horizontal rules echoing the device's trim rings.
- **Shadows:** barely-there, petrol-tinted, two levels (card, float). No inner shadows.
- **Transparency/blur:** rare; white at 70% + `backdrop-blur` only for the fixed nav over imagery.
- **Layout:** 1200px content column; nav fixed, all else flows. Feature grids 3-up; product duo 2-up.

## ICONOGRAPHY
- No icon set was provided. Use **Lucide** (CDN) at `stroke-width:1.5` — its thin, quiet line style matches the logo's line-drawn droplet. Petrol strokes on light, white on petrol. This is a **flagged substitution** — replace if the brand adopts an icon set.
- The logo (`assets/logo.svg`, petrol droplet forming an "Ä" with umlaut dots + DÄRET wordmark + "by SAUAPKER") is the only illustration. Never redraw it; never recolor beyond all-white on petrol.
- No emoji, no unicode-as-icon.

## Intentional additions
- Standard component set (Button, Input, etc.) authored from the brief — no source component library existed. Kept minimal.
- Lucide icons (CDN substitution, flagged above).

## Index
- `styles.css` → `tokens/` (fonts, colors, typography, shape)
- `assets/` — logo.svg, product renders (white/straw hero + front), lifestyle (hand-sensor, travel-car, water-stream), textures (straw), backgrounds (petrol gradient, water ripples), banner
- `guidelines/` — foundation specimen cards (colors, type, spacing, radii, shadows, imagery, logo)
- `components/core/` — Button, IconButton, Badge, Input, Select, Switch, Card, FeatureCard, ProductTile, Stat, NavBar, Footer, SectionHeader
- `ui_kits/site/` — DÄRET marketing site (index.html + screens)
- `templates/` — (reserved for deck/doc templates)
- `SKILL.md` — agent skill entry point
