# longlostforgotten.com

Personal site / blog. Currently in holding pattern.

---

## Status

**Phase:** Coming soon  
**Holding page:** `index.html` — self-contained, no build step required  
**Full site:** Planned, Astro + TinaCMS (see Site Brief)

---

## Repo Structure

```
longlostforgotten/
├── index.html          # Coming soon page (deploy to site root)
├── README.md           # This file
├── SITE-BRIEF.md       # Full aesthetic and technical brief
└── src/                # (future) Astro project lives here
```

---

## Holding Page

`index.html` is fully self-contained — one file, no bundler, no build step. It loads three Google Fonts and everything else is inline.

**To deploy:** Drop `index.html` into your site root. Done.

**Fonts used (via [Bunny Fonts](https://fonts.bunny.net)):**
- [Barlow Condensed](https://fonts.bunny.net/family/barlow-condensed) — headline ("Long Lost"), weight 900
- [Josefin Sans](https://fonts.bunny.net/family/josefin-sans) — UI / labels
- [Share Tech Mono](https://fonts.bunny.net/family/share-tech-mono) — subheading, status, monospace chrome

No JavaScript dependencies. All animation is CSS. Fonts load from Bunny Fonts — no Google Fonts.

---

## Full Site Build (future)

### Stack

- **Framework:** Astro (latest stable)
- **CMS:** TinaCMS (Git-backed, local + cloud)
- **Hosting:** Self-hosted VPS
- **CI/CD:** GitHub Actions
- **CSS:** Scoped CSS + CSS custom properties (no Tailwind)
- **Reset:** normalize.css

### Setup (when starting the Astro project)

```bash
npm create astro@latest
# choose: empty project, TypeScript optional
# then:
npx astro add tinacms
```

Reference `SITE-BRIEF.md` for palette, typography, and design system specs before building any components.

### CSS conventions

- All color tokens defined as CSS custom properties on `:root`
- Scoped `<style>` blocks per Astro component
- `normalize.css` imported globally in layout
- No utility frameworks

---

## Design Reference

See `SITE-BRIEF.md` for:
- Full color palette with hex values
- Typography stack and usage
- Visual language / texture system
- Page structure and future scope

---

## Notes

- Dark only — no light mode planned
- Add `prefers-reduced-motion` media query to disable flicker/noise animations before launch
- Favicon TBD — target a simple diamond or signal-mark form
- Hero images: AI-generated via NightCafe or Leonardo.ai (Phoenix), abstract/graphic style

---

*longlostforgotten.com*
