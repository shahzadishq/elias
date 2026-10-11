# Elias Kaltenberger — Premium Landing Pages

Two premium, high-converting landing pages for photographer & photo-business
mentor **Elias Kaltenberger**, built to match the existing brand
([eliaskaltenberger.com](https://www.eliaskaltenberger.com/)).

| Page | File | Audience | Goal |
|------|------|----------|------|
| **Landing Page 1** | [`vom-nebenberuf-zum-profi.html`](vom-nebenberuf-zum-profi.html) | Part-time photographers | Go full-time — book a free strategy call |
| **Landing Page 2** | [`vom-fotograf-zum-unternehmer.html`](vom-fotograf-zum-unternehmer.html) | Self-employed photographers | Scale to a business with studio & team |

See **[BRAND-STRATEGY.md](BRAND-STRATEGY.md)** for the full brand analysis,
strategy and section structure. Rendered previews are in [`previews/`](previews/).

## How to view
Open either `.html` file directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/vom-nebenberuf-zum-profi.html
```

## Tech & decisions
- **Stack:** semantic HTML5 + modern CSS + a little vanilla JS. No build step,
  no framework, no dependencies — fast and easy to hand off or drop into
  WordPress/Elementor.
- **Fonts:** Montserrat + Cormorant Garamond (Google Fonts), matching the
  brand's existing type stack.
- **Design system:** one shared token set (`:root` custom properties for the
  black + champagne-gold palette, type, spacing, motion) used by both pages for
  brand consistency, with distinct section layouts so the pages don't look
  identical.
- **CSS/JS are inlined per page** on purpose — a single request per page means
  a fast LCP and a fully portable file. Both pages share the same token block,
  which is the single source of truth for the brand look.
- **Images** are the client's own assets (`assets/img/`), downloaded from the
  live site so the pages belong to the same brand ecosystem.
- **Responsive:** mobile-first, verified with no horizontal overflow at
  360 / 390 / 768 / 1024 / 1440 px.
- **Accessibility:** semantic landmarks, focus-visible states, keyboard-friendly
  mobile menu, reduced-motion support, alt text, and content that stays visible
  even if JavaScript is disabled (`no-js` guard).
- **SEO:** unique titles/descriptions, canonical, Open Graph, and
  JSON-LD structured data per page.

## Call-to-action
Every CTA links to the existing booking flow at
`https://www.eliaskaltenberger.com/kontakt/` (questionnaire → appointment).
Swap this URL if the booking destination changes.

## Project structure
```
.
├── vom-nebenberuf-zum-profi.html      # Landing Page 1
├── vom-fotograf-zum-unternehmer.html  # Landing Page 2
├── assets/img/                        # brand images (client's own)
├── previews/                          # rendered desktop/mobile/hero screenshots
├── BRAND-STRATEGY.md                  # brand analysis + strategy + structure
└── README.md
```
