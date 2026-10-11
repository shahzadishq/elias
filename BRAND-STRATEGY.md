# Elias Kaltenberger — Brand Direction & Landing Page Strategy

Prepared before implementation. Covers (1) brand analysis of the existing
website, (2) the strategy for each landing page, and (3) the section
structure that was built.

---

## 1. Brand Direction Report

### Positioning
Elias Kaltenberger is an Austrian **premium photographer turned photo-business
mentor**. The brand sells *certainty and freedom* to photographers: planbare
Anfragen (predictable enquiries), premium prices, and a life that isn't ruled
by the next random booking. It is a high-ticket, trust-led coaching brand — not
a cheap course.

### Target audience
German-speaking (DACH) photographers & videographers, split into two maturity
stages — which is exactly why there are two landing pages:
- **Part-time photographers** who want to go full-time (Landing Page 1).
- **Established self-employed photographers** who want to scale into a real
  business with studio & team (Landing Page 2).

### Brand personality & tone of voice
- **Personal, direct, "du"** throughout — a peer who has walked the path
  (Tischler → Premiumfotograf), not a distant guru.
- **Honest & transparent** ("Wir sind 100% transparent", "kein Verkaufspitch").
- **Aspirational but grounded** — real numbers, real names, real stories.
- Emotional triggers: financial security, family time, freedom, recognition of
  one's worth, the fear of staying stuck.

### Trust-building elements (reused on both pages)
- **238+** photographers coached · **107 Trustpilot** reviews · **826+** paid
  shoots · press mentions · named case studies with revenue figures · the free,
  no-pressure strategy call · studio in St. Pölten (30 min from Vienna).

### Visual identity (extracted from eliaskaltenberger.com)
- **Colour:** Black / near-black (`#0B0B0C`, `#151515`) + a signature
  **champagne-gold / bronze `#B07F2C`** (the single most-used colour on the live
  site, 190+ occurrences), with lighter golds `#D9BE7E`, `#D3B379` and a warm
  off-white `#F8F7F4`. This is a classic **luxury black-and-gold** system.
- **Typography:** **Montserrat only** — per the client's CI, Montserrat is the
  single typeface of the system; hierarchy comes from weight/size/spacing
  (headlines bold/extrabold, body regular). No secondary serif.
- **Gold gradient (official CI "Goldverlauf"):** `#B07F2C → #F3E07A → #B07F2C`
  for accents/numbers; button variant `#9A6F24 → #E2CD68 → #9A6F24`. Applied
  via the `--grad-gold` / `--grad-gold-btn` tokens in both pages.
- **Design language:** dark, editorial, generous whitespace, thin gold
  hairlines, uppercase letter-spaced labels, framed imagery, restrained motion.

### Design principles applied
- Premium = **restraint**: sharp 5px radii, hairline borders, one accent colour,
  no rainbow gradients, no cheap SaaS tropes.
- **Real brand assets only** — every photo is Elias's own (portrait, studio,
  client success photos), so the pages sit inside the existing brand ecosystem.
- Motion is subtle and purposeful (scroll reveals, hover lifts, image zoom),
  and fully disabled under `prefers-reduced-motion`.

---

## 2. Landing Page Strategy

Both pages share one brand system but are deliberately **not identical** (per the
client note in the source document: the pages must not look like the same page).
They differ in composition, section language, step count and proof layout.

### Landing Page 1 — `vom-nebenberuf-zum-profi.html`
- **Goal:** convert part-time photographers into free strategy-call bookings.
- **Audience:** hobby-to-pro photographers who already shoot well but have no
  predictable business.
- **Emotional arc:** recognition → empathy ("I was exactly there") → proof →
  plan → reassurance → book the call.
- **Conversion goal:** one primary CTA — *Kostenloses Strategiegespräch* — to
  the existing `/kontakt/` booking flow (questionnaire → appointment, per the
  client's CTA rule).
- **Tone:** warmer, story-driven, encouraging.

### Landing Page 2 — `vom-fotograf-zum-unternehmer.html`
- **Goal:** convert already-successful self-employed photographers into calls.
- **Audience:** full-time photographers hitting a ceiling, everything depends on
  them personally.
- **Emotional arc:** ambition → the bottleneck problem → the self-employed vs.
  entrepreneur contrast → the 5-step system → proof (bigger numbers) → book.
- **Conversion goal:** same single CTA to `/kontakt/`.
- **Tone:** more strategic / business-forward, metric-led.

---

## 3. Section Structure

### Landing Page 1
1. Sticky header + mobile menu
2. Hero — headline, sub, dual CTA, portrait card, trust row
3. Trust bar — 238+ · Trustpilot 107 · 3.000–6.000€ · 100% transparent
4. Problem / empathy (light) — "das Business drumherum"
5. Story / turning point — *Vom Tischler zum Profifotograf* timeline
6. The 4 steps — Denken · Angebot · Anfragen · Wertkommunikation
7. Benefits grid — planbare Anfragen, faire Preise, Hauptberuf, Zeit für Familie
8. Testimonials — Michele Peloza, Michael Winter, Claudia Edhofer + mini-results
9. Audience fit — passt / passt noch nicht
10. Process — Kennenlernen → Strategiegespräch → Fahrplan
11. About Elias + studio
12. Final CTA
13. Footer

### Landing Page 2
1. Sticky header + mobile menu
2. Hero — architectural, studio backdrop, metric-led
3. Stat band — 200.000€ · 60 Hochzeiten · 15–20k€ · 3× Preise
4. Problem — Umsatzschwankungen · alles hängt an dir · keine Freiheit
5. Comparison — selbstständiger Fotograf **vs.** Fotounternehmer
6. The 5-step process (vertical timeline)
7. Systems grid — the 5 systems + dashboard
8. Testimonials (editorial rows) — Anna, Barbara, Steve, Claudia Brandl
9. About Elias + portrait
10. Audience fit
11. Final CTA
12. Footer

---

## Content source & accuracy
All copy is adapted from the client's reference document (Tab 2 → LP1, Tab 3 →
LP2) and the live website. Numbers, names and client stories are taken directly
from those sources. Wording was tightened for conversion where helpful; no
claims were invented.
