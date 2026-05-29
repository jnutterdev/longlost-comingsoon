# longlostforgotten.com — Site Brief

## Overview

**Domain:** longlostforgotten.com  
**Type:** Personal blog / long-form personal site  
**Status:** Coming soon (holding page deployed)  
**Author:** Single author

---

## Concept & Voice

*longlostforgotten* is a personal site and social handle. The name carries a dry, melancholic wit — something recovered, something half-remembered, something that maybe shouldn't have been found. The voice should feel like a noir narrator who reads too much, thinks too hard, and finds the whole situation mildly inconvenient.

The site's thesis statement — used as the hero line on the coming soon page and carried forward as a kind of slogan — is:

> **"long lost: the terrible inconvenience of"**

The sentence is intentionally incomplete. It's a heading without a subject. The reader supplies the rest.

---

## Aesthetic Direction

**Primary:** Film noir / Art Deco  
**Secondary influence:** Sci-fi neo-noir (Blade Runner-era, not synthwave)  
**Texture:** Analog signal degradation layered over geometric structure — like a 1940s broadcast tower trying to reach you from 2049

The aesthetic should feel like a recovered artifact: designed with intention, then partially consumed by time and interference. Clean bones beneath the noise.

**Not:** neon synthwave, vaporwave, retrowave. The neon is implied, not announced.

---

## Color Palette

| Role | Value | Notes |
|------|-------|-------|
| Background | `#0a0906` | Near black, warm ink |
| Pink primary    | `#fb66a4` | Headline color, used boldly |
| Sand / khaki    | `#c8c88d` | Secondary warm tone, labels, rules |
| Teal accent     | `#4a8fa0` | Cool counterpoint, corner ornaments, transmission label |
| Magenta ghost   | `rgba(251,102,164,0.12)` | Ghost ellipse in SVG only |
| Line / rule     | `rgba(200,200,141,0.14)` | Faint structural elements |

Magenta is intentionally suppressed. It should read as warmth in the geometry, not as color.

---

## Typography

| Role | Font | Weight/Style |
|------|------|-------------|
| Display / headline | Barlow Condensed | 900 — "Long Lost" only |
| Subheading         | Share Tech Mono  | 400 — "the terrible inconvenience of" |
| Monospace / status / data | Share Tech Mono | 400 |

Bunny Fonts (fonts.bunny.net). All fonts loaded via Bunny Fonts for privacy. No Google Fonts. Federo is not used.

---

## Visual Language

- **Scanlines** — subtle CRT horizontal line texture over all content
- **Vignette** — radial darkening toward edges, simulates phosphor fall-off
- **Noise overlay** — low-opacity grain, animated in short steps
- **Deco geometry** — faint Art Deco structural elements (double-ruled frames, center diamond motifs, corner bracket ornaments, sunburst rays). Should feel watermarked, not foregrounded
- **Signal bar** — thin amber rule across top of viewport, slowly pulsing
- **Corner ornaments** — L-bracket style deco corners, fixed to viewport edges
- **Status line** — monospace readout at bottom, simulated frequency/carrier data

Animations should be slow and atmospheric — pulse, drift, flicker. Nothing frantic. One brief text flicker on the headline every ~8 seconds is enough to feel alive.

---

## Coming Soon Page

**File:** `index.html`  
**Implementation:** Pure HTML/CSS/JS, no dependencies except Google Fonts  
**Hosting:** Drop into site root, replace when full site launches

Key elements:
- Transmission label: `— transmission recovered █` (cursor blinks)
- Hero statement: `long lost: the terrible inconvenience of`
- Domain stamp: `signal pending / stand by`
- Status bar: `STA-7 · FREQ: 47.223 · CARRIER LOST · SEEKING…`
- Staggered fade-in animation on all elements, ~0.8–3s delay sequence

---

## Full Site — Future Scope

To be built in **Astro + TinaCMS**.

### Pages
- `/` — Index / home (featured post, recent entries)
- `/archive` — Full post archive with filtering
- `/about` — Author page

### Post types
- Standard long-form posts
- Possibly: micro/note format (shorter, more frequent)

### Technical stack
- Astro (latest version at time of build)
- TinaCMS (Git-backed)
- Self-hosted VPS
- GitHub Actions CI/CD
- Scoped CSS + CSS custom properties (no Tailwind)
- normalize.css as baseline reset

### Design notes for full build
- Carry forward all three fonts
- Preserve the scanline/noise/vignette aesthetic as a lighter background treatment on content pages
- Deco geometry becomes structural UI — dividers, pull-quote treatments, category labels
- Consider a reduced-motion media query that disables flicker/noise animations
- Dark only — no light mode planned

---

## Assets

- `index.html` — Coming soon page (self-contained)
- Hero images: generate via AI (NightCafe / Leonardo.ai Phoenix model), target abstract/graphic over figurative
- Favicon: to be designed — consider a simple diamond/signal mark

---

*Brief version 1.0 — coming soon phase*
