# AGENT.md — Personal Index Context

> Handoff doc for future Claude sessions. Read this first, then read [STYLE.md](./STYLE.md).
> Last updated: 2026-05-27 — expanded from trips-only to multi-domain personal index.

## What this repo is

`jmark` is **Mark Shors' personal index** — trips, daily practice, ideas, articles, supplements, and reference — hosted on GitHub Pages.

- **Live site:** https://mshors-pdai.github.io/jmark/
- **Repo:** https://github.com/mshors-pdai/jmark
- **Deploy:** GitHub Pages from `main` branch, root `/`. Push to update (~30–60s to go live; new files can take up to 2 min).
- **Local working copy:** `/tmp/jmark-deploy/` on the operator's MacBook.
  Note: `/tmp` survives only until reboot — if missing, `gh repo clone mshors-pdai/jmark /tmp/jmark-deploy` to restore.

### Structure

```
jmark/
├── index.html                       # HUB: now-band + trips catalog + previews of every domain
├── STYLE.md                         # Style guide — read before building a new trip page
├── AGENT.md                         # This file
├── trip/                            # Travel itineraries (existing — preserved exactly)
│   ├── aug_11_provence.html         # Itinerary No. 01 — couples', Aug 2026
│   └── jun_20_kern.html             # Itinerary No. 02 — family, summer 2026
├── practice/                        # Daily / weekly / monthly protocols
│   └── index.html                   # The full practice prescription (sage palette)
├── article/                         # Finished essays & frameworks
│   └── index.html                   # Article catalog (indigo palette)
├── idea/                            # Seeds, drafts, half-formed thoughts
│   └── index.html                   # Status-tagged catalog (amber palette)
├── supplement/                      # Quarterly stack with retained history
│   └── index.html                   # Current Q2 2026 stack (clay palette)
└── reference/                       # Quick lookups: gear, contacts, recurring numbers
    └── index.html                   # Reference utility drawer (slate palette)
```

**Trip URLs are stable.** Existing pages like `/trip/jun_20_kern.html` were preserved exactly when expanding to multi-domain. The root `index.html` was edited additively — the original trip catalog (search + filter + cards) is intact below a new "Now" band.

**Future trips:** add `trip/<mon3>_<dd>_<slug>.html` and a card to `index.html`. STYLE.md has the full pattern.

**Future content in other domains:** each section index is self-contained with its own palette. Add items by editing the appropriate section's `index.html` — promote ideas → articles, version supplements by quarter, add reference blocks as patterns repeat.

---

## Active trips

### Trip No. 01 · Cassis & the Calanques (Provence)

**Status:** planned, not yet booked
**Dates:** Tue Aug 11 → Mon Aug 17, 2026 (6 days, **5 hotel nights**)
**Origin:** LAX · **Travelers:** 2 · **Selected tier:** Standard (~$9,580 total all-in)

**Selected logistics (operator decisions):**

| What | Choice | Notes |
|------|--------|-------|
| Flight | **Air France AF65** LAX→CDG→MRS · Aug 11 1:40 PM dep · arrives MRS **1:05 PM Aug 12** | Daytime departure chosen specifically to land at lunch, not midnight |
| Hotel (all 5 nights) | **The Address Cassis** | Adults-only 5-star boutique, hillside, ~€420–€680/night |
| Big dinner | **La Villa Madie ★★★** (Day 3 · Fri Aug 14) | Now 3 Michelin stars (promoted 2022). Book 60+ days ahead. |
| Boat | **L'Eden Boat private RIB · 6h · Day 2** | Aug 13 morning, before crowds |
| Wineries | 4: Clos Sainte Magdeleine, Domaine du Bagnol, Domaine Tempier, Château de Pibarnon | All require phone appointments |

**Time-locked events on these exact dates:**

- **☄️ Perseid meteor shower peak** — night of Aug 12→13. 2026 is the **best Perseid year of the decade** (new moon Aug 12 = moonless sky, 90+ meteors/hour). Day 1 itinerary includes a late-night Cap Canaille viewing.
- **🎆 Aug 15 Assumption Day** — Cassis throws its biggest party. Apéro 7 PM, fireworks 10 PM, ball 10:30 PM at Place Baragnon. Day 4 is built around this — no out-of-town trips Saturday.
- **🎹 Festival de La Roque d'Anthéron** — world's largest piano festival, runs through Aug 16. Optional Day 5 alternative.
- **🎨 Cassis Night Market & Quai des Artistes** — every evening 7 PM–midnight, June 25 → Aug 31.

**Open booking items (Provence):**

- [ ] **Book the AF65 flight.** Air France direct, Aug 11 1:40 PM LAX dep.
- [ ] **Book The Address Cassis** — 5 nights Aug 12–17. Booking.com listing exists; consider emailing direct for room assignment.
- [ ] **Reserve La Villa Madie ★★★** for Fri Aug 14. ~60 days lead time. lavillamadie.com/en/reservation/. Phone +33 4 96 18 00 00.
- [ ] **Book L'Eden Boat private RIB** for Thu Aug 13 morning, 6-hour tour. rent.ledenboat.com.
- [ ] **Phone calls to wineries:**
  - Domaine Tempier (+33 4 94 98 70 21) — Fri Aug 14 morning
  - Château de Pibarnon (+33 4 94 90 12 73) — Fri Aug 14 afternoon
  - Clos Sainte Magdeleine (+33 4 42 01 70 28) — Sat Aug 15, 10 AM
  - Domaine du Bagnol (+33 4 42 01 32 16) — walk-in OK
- [ ] **Verify Atelier Cézanne reopening status** before counting on Aix day trip — closed Nov 2025 for renovation, reopen TBD.
- [ ] **Optional bookings:** bouillabaisse cooking class with Chef Gilles (provence-plaisirs.com), helicopter Calanques tour (sport-decouverte.com), Cosquer Méditerranée tickets.

---

### Trip No. 02 · Kern River Weekend

**Status:** planned, not yet booked
**Dates:** **Sat Jun 20 → Sun Jun 21, 2026** (recommended) · candidates also Jul 18, Aug 1
**Origin:** Orange County · **Travelers:** 2 adults + 3 kids (ages 7, 10, 12) · **Vehicle:** Rivian R1T

**Why Jun 20 won over Jul 18 / Aug 1:** pulled NOAA 5-year reanalysis (2020–2024, ±3d windows) via Open-Meteo archive API. Triple-digit-day probability: **Jun 20 = 23%**, Jul 18 = 46%, Aug 1 = 31%. Plus by Aug 1 the Kern is reliably below rafting flow (most outfitters closed).

**Selected logistics (operator decisions):**

| What | Choice | Notes |
|------|--------|-------|
| Rafting | **Lickity Split** (Class II–III, ~1 hr) | Sierra South top pick — min age 6 covers the 7-year-old. Do NOT get upsold to Powerhouse Run. |
| Outfitter (primary) | **Sierra South** · sierrasouth.com · 760-376-3745 | Best family-trip reputation |
| Outfitter (backup) | Kern River Outfitters · 760-376-3370 | If Sierra South full |
| Lodging | **Whispering Pines Lodge** (riverside) | Call directly · 760-376-3733 |
| Lodging backup | Kernville Inn · 760-376-2206 | Central, simpler |
| Off-road primary | **Sherman Pass Road 22S05** | Graded dirt to 9,200 ft. Drive mode All-Terrain, 25 PSI. R1T-appropriate. |
| Off-road backup | Cherry Hill / Greenhorn | Use if Sherman snowed |
| Off-road avoid | Jawbone Canyon, Piute technical, anything 3+ rated | R1T too wide (87") and heavy (~7,000 lbs) |

**Operator constraints for this trip (extracted from session):**

- **Beginner posture · nervous family.** Drove every recommendation. No upsells, no technical trails. The Powerhouse Run was rejected specifically because of the 7-year-old.
- **R1T off-road**: All-Terrain mode only (never Rally with kids aboard). Air down to ~25 PSI on dirt. Plan one DCFC stop each way in Bakersfield.
- **The "no" rule:** anyone in the family (including the 7-year-old) can opt out of any activity. Win condition = everyone wants to come back next year, not finishing the itinerary.

**Open booking items (Kern):**

- [ ] **Book Whispering Pines Lodge** for Jun 20→21. Call directly. Ask about R1T parking + 110V outlet for overnight trickle charge.
- [ ] **Book Lickity Split** with Sierra South for Sat Jun 20 morning (10:30 or 11:00 AM slot). Specify ages 7/10/12, beginners. Confirm 7yo meets min age.
- [ ] **Charging recon:** test EVgo + ChargePoint apps; identify primary + backup Bakersfield stations on PlugShare.
- [ ] **Two days before:** call Sequoia NF Kern River District (760-376-3781) to confirm Sherman Pass open to saddle.
- [ ] **One week before:** check USGS gauge "Kern River at Kernville" and NWS 10-day. Heat-bail rule: if forecast > 100°F, postpone a week.
- [ ] **Download offline maps:** Kern River area in Gaia GPS or onX Offroad (cell service dead above Kernville).

---

## Operator preferences (durable — apply to future trips too)

These were extracted from the iterative back-and-forth across both trip planning sessions. Treat as constraints unless explicitly relaxed.

**Travel style (couples' trips):**
1. **Weather sweet spot: 75–80°F highs.** Above 82°F is "too hot." Below 70°F is "too cold."
2. **Crowds: low.** Will skip a famous place if it's a zoo in peak season.
3. **No bugs.** Tropical destinations with mosquito pressure are out. Mediterranean dry climates are fine.
4. **Hotels: $500–$1,000/night.** Will flex up by ~$200/night for an iconic property; will not flex up by $400+.
5. **≤ 2 hotels total across a trip.** One base preferred if drives allow.
6. **≤ 1.5 hour drives** between activities.
7. **Arrival time at destination: ~1 PM ideal.**
8. **Wine matters.** Trip is built around wine experiences. Named wineries with appointments.
9. **Food matters.** Always at least one Michelin-tier dinner. Local seafood emphasized.
10. **Nightlife: lively dinners + wine bars OK, clubs not necessary.**
11. **Romance is the through-line.** Couples' escape.

**Travel style (family weekends):**

12. **Beginner posture by default** when nervous travelers are involved. Don't upsell.
13. **The youngest age is the constraint** — every activity has to work for the 7-year-old, even if older kids could handle more.
14. **R1T off-road only on graded scenic roads.** Not technical trails. The truck is wider/heavier than typical off-road vehicles.

### Communication preferences

- **Terse responses; no unnecessary preamble.** Operator pushes back on long explanations.
- **Concrete options with prices/URLs > abstract recommendations.**
- **Be honest about trade-offs.** When operator's constraints conflict, surface the conflict.
- **Web research expected** when there's any doubt about prices, hours, weather, river flow, or current status. Operator explicitly asks for "actual research."
- **Verify URLs before adding them.** Search for the official site rather than guessing the URL pattern.
- **Don't say "per person"** in budget breakdowns. (Operator preference, stated explicitly.)

---

## Decision history (Provence)

| Round | Considered | Outcome |
|-------|-----------|---------|
| 1 | Amalfi, Greek islands, Mallorca, Croatia, Mauritius | Amalfi initial top pick |
| 2 | Italy excluded by operator | Pivot |
| 3 | Mallorca · Milos · Hvar · Mauritius | Mallorca top until temperature constraint |
| 4 | Galicia introduced | Top pick on most criteria (75–78°F, uncrowded, world-class wine) but only Spanish-style nightlife |
| 5 | Galicia + Porto combo | Operator added "≤ 1.5h drive" → Porto dropped (2.5h from Galicia) |
| 6 | Three-way: Galicia · Provence · Mallorca | Operator dropped Galicia and Mallorca; Provence selected |
| 7 | Within Provence: Cassis vs. other bases | Cassis selected; 1 hotel for all 5 nights |
| 8 | Within Cassis: 6 hotels presented | The Address Cassis chosen for adults-only + budget fit |

**Why Provence won:** dramatic scenery (Calanques), serious wine (Cassis AOC + Bandol), cleanest hit on the $500–1000 hotel budget, earliest LAX-to-Europe daytime arrival (1:05 PM at MRS via AF65), and a single hotel works.

---

## Decision history (Kern River)

| Round | Considered | Outcome |
|-------|-----------|---------|
| 1 | "What are off-road and rafting options in Kern?" | Sherman Pass / Cherry Hill / Keyesville for off-road; Lickity Split rafting |
| 2 | R1T + beginner + nervous family added as constraints | Ruled out Jawbone + Piute + technical Keyesville; locked in graded-dirt routes only |
| 3 | "When's the best date?" — Jun 13–14 first picked | Recommended early-to-mid June for snowmelt flow + heat |
| 4 | Operator added candidates: Jun 20 · Jul 18 · Aug 1 | Pulled NOAA 5yr reanalysis; built side-by-side comparison; Jun 20 chosen on heat numbers |

**Why Jun 20:** lowest triple-digit-day probability of the three candidates (23% vs 46%/31%), highest probability of raftable flow, snowmelt still feeding the Lickity Split section.

---

## Style + components

**Read [STYLE.md](./STYLE.md) before building a new trip.** It's the source of truth for:
- Fonts (Playfair Display + Inter)
- Color palette pattern (deep · accent · soft · cream — picked per destination)
- Required sections in order
- File slug convention (`mon3_dd_slug.html`)
- Component patterns (back-bar, hero card, day timeline, hotel cards, map share-row, booking checklist)
- Mobile breakpoints + mandatory rules
- Index card pattern with `data-search` + `data-tags`
- Image source rules (Wikipedia Commons preferred for landscapes, Unsplash for atmosphere — always verify URLs)

---

## How to update the site

```bash
# 1. Edit locally
cd /tmp/jmark-deploy
# ...edit trip/<slug>.html, index.html, or STYLE.md...

# 2. Commit and push
git add .
git -c user.email="mshors-pdai@users.noreply.github.com" \
    -c user.name="mshors-pdai" \
    commit -m "<change description>"
git push origin main

# 3. Verify deploy (~30–60s for existing files, up to 2 min for new files)
curl -s -o /dev/null -w "%{http_code}\n" https://mshors-pdai.github.io/jmark/
```

### To add a new trip

1. Read STYLE.md first.
2. Create `trip/<mon3>_<dd>_<slug>.html` (mirror the structure of the most recent itinerary).
3. Add a `<a class="trip-card large">` to the grid in `index.html` with `data-search` and `data-tags` populated.
4. Bump `#stat-trip-count` and update other stats (year, countries, next departure) if relevant.
5. Add a new section to this AGENT.md under "Active trips" with status + decisions + open items.
6. Update the "Next trip" card in the Now band on `index.html` if this becomes the next one.
7. Commit + push.

### To add to a non-trip section

Each section index is self-contained. The pattern is consistent across domains:
- Back-bar (`../index.html` link)
- Hero with eyebrow + italic-accent h1
- Content area (list, grid, or stack depending on domain)
- Footer with cross-links to related sections

**Practice** (`practice/index.html`) — single comprehensive page. Update in place when the protocol evolves. Hash anchors `#daily`, `#morning`, `#midday`, `#evening`, `#weekly`, `#cycles`, `#substrate`, `#avoid`, `#ranked`, `#compression`.

**Articles** (`article/index.html`) — add `<a class="article-card">` to `.article-list`. Article body pages live as `article/<slug>.html` once an idea is mature enough. Promote from `idea/` when an idea survives reality-testing.

**Ideas** (`idea/index.html`) — add `<div class="idea" data-status="seed|drafting|published|dropped">` to `.idea-grid`. Update the status attribute as the idea progresses. When `published`, also create an article entry and link forward.

**Supplements** (`supplement/index.html`) — current quarter is at the top. When rotating, move current to history list and start a new quarter section. Versioned as `supplement/<yyyy>_q<n>_stack.html` if a quarter deserves its own page; otherwise inline.

**Reference** (`reference/index.html`) — add a `<div class="ref-block">` with `<h2>` category + `<ul class="ref-list">` of label/value rows. Add a category when you find yourself looking up something more than twice.

After any change to a section, update the Now band and the section preview cards on root `index.html` if the displayed item changes.

### To take the site down

```bash
gh repo delete mshors-pdai/jmark --yes
```

---

## Source files

- **Canonical local edit copies (per trip):**
  - Provence: `/Users/markshors/embeddedLayers/trip-aug-2026.html`
  - Kern: `/Users/markshors/embeddedLayers/jmark/kern-trip.html`
- **Deploy copy:** `/tmp/jmark-deploy/` — what GitHub sees.

The two-file workflow exists because the local files were written before the deploy structure was set up. For new trips, simpler to edit the deploy copy directly under `/tmp/jmark-deploy/trip/`.

---

## Quick context for a cold session

If a future Claude has read nothing else: **operator runs two active trip plans through this repo — a romantic 6-day Provence trip in August 2026 and a 2-day Kern River family weekend in June 2026. Both are planned, neither fully booked. Open items are mostly booking calls. The site is searchable by topic at https://mshors-pdai.github.io/jmark/ and has a STYLE.md for adding new trips. Stick to the durable preferences above.**
