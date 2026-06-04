# AGENT.md — Personal Index Context

> Handoff doc for future Claude sessions. Read this first, then read [STYLE.md](./STYLE.md).
> Last updated: 2026-06-04 — **Trip 03 criteria recalibrated to active+nightlife+late-dinners+good-food** (Joann said original brief was boring). Hub expanded 6 → 9 options: Mykonos, Hvar+Split, Côte d'Azur added. New standings: **San Sebastián 36 = Côte d'Azur 36 (tied)**; Cascais 35; Mallorca 34.5; Annecy 34 (old winner, drops on nightlife); Hvar+Split 34; Madeira 32.5; Mykonos 32; Provence 31.5 (booked baseline). Criteria reshape: out "less seafood / low crowds" as hard filters, in "nightlife & late energy / activity density" as hard filters; seafood demoted to soft modifier. Each option backed by 3,000–5,000-word deep-research dossier (web-cited; ~80 tool calls / agent). Per-page over-packed itinerary rewrites still pending; hub scoring + verdict already reflect the recalibration.
> 2026-06-02 — Mallorca added as Trip 03 Option F; criteria + scoring-matrix section added to the hub (Annecy then led at 38/39); repo moved out of `/tmp/jmark-deploy/` to `~/embeddedLayers/jmark/`; legacy local edit copies archived to `.archive-pre-merge-2026-06-02/`.

## What this repo is

`jmark` is **Mark Shors' personal index** — trips, daily practice, ideas, articles, supplements, and reference — hosted on GitHub Pages.

- **Live site:** https://mshors-pdai.github.io/jmark/
- **Repo:** https://github.com/mshors-pdai/jmark
- **Deploy:** GitHub Pages from `main` branch, root `/`. Push to update (~30–60s to go live; new files can take up to 2 min).
- **Local working copy:** `/Users/markshors/embeddedLayers/jmark/` on the operator's MacBook.
  (Moved out of `/tmp/jmark-deploy/` on 2026-06-02 — `/tmp` doesn't survive reboot.)
  If missing, restore with: `gh repo clone mshors-pdai/jmark /Users/markshors/embeddedLayers/jmark`

### Structure

```
jmark/
├── index.html                       # HUB: now-band + trips catalog + previews of every domain
├── STYLE.md                         # Style guide — read before building a new trip page
├── AGENT.md                         # This file
├── trip/                            # Travel itineraries
│   ├── aug_11_europe.html           # Trip No. 03 HUB — 9-option Aug 11-17 decision · recalibrated 2026-06-04 · SS + Côte d'Azur tied 36/39
│   ├── aug_11_provence.html         # Itinerary No. 01 — couples', Aug 2026 (also Trip 03 · Option A · booked baseline · new score 31.5)
│   ├── aug_11_cascais.html          # Trip 03 · Option B — Portugal Atlantic · new score 35 (+8 from old criteria — biggest jump)
│   ├── aug_11_san_sebastian.html    # Trip 03 · Option C — Basque · TIED LEADER 36 · Aste Nagusia Aug 8-15 lands inside trip
│   ├── aug_11_madeira.html          # Trip 03 · Option D — Atlantic island · new score 32.5 (-1.5 on nightlife)
│   ├── aug_11_annecy.html           # Trip 03 · Option E — French Alps · new score 34 (-4 from old 38, was old winner)
│   ├── aug_11_mallorca.html         # Trip 03 · Option F — Balearic, Deià · new score 34.5 (+4.5)
│   ├── aug_11_mykonos.html          # Trip 03 · Option G — Cycladic nightlife · new score 32 · NEW added 2026-06-04
│   ├── aug_11_hvar.html             # Trip 03 · Option H — Dalmatian sailing · new score 34 · NEW added 2026-06-04
│   ├── aug_11_cote_dazur.html       # Trip 03 · Option I — French Riviera grand · TIED LEADER 36 · NEW added 2026-06-04
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

**Decision hubs:** when a trip has multiple candidate destinations under active deliberation, build a hub page at `trip/<mon3>_<dd>_<region>.html` that side-by-sides them. Pattern: hero + N-card option grid + criteria-card section + scoring matrix + comparison table + pros/cons grid + budget side-by-side + verdict. Hub grid + pros-cons-grid use 2-col layout (rows of 2); odd-numbered options get a `style="grid-column: span 2;"` to fill. See `trip/aug_11_europe.html` for the canonical example — now 6 options A–F with an 8-criterion scoring matrix (5 hard / 3 soft, scored /39). Each option file gets a back-bar `meta-mini` that links back to the hub via `compare N options ↗`.

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

> **Note (added 2026-06-02):** Cassis is now also the **Option A · booked baseline** under the Trip No. 03 Europe deliberation (see below). If the operator decides to swap, the Provence file stays as a fallback. Don't delete or renumber it.

---

### Trip No. 03 · Europe Decision Hub · Aug 11–17, 2026

**Status (recalibrated 2026-06-04):** active deliberation · 9 plans on the table, Provence is the booked baseline, **San Sebastián and Côte d'Azur tied at 36/39** under the new criteria.
**Dates:** Tue Aug 11 → Mon Aug 17, 2026 (6 days, **5 hotel nights**) — same dates as Trip No. 01
**Origin:** LAX · **Travelers:** 2 · **Decision deadline:** by July 1, 2026 (to keep Belcanto + Berasategui + 3★ tables + Voro ★★ + Caves du Roy + Le Louis XV on the table)

**The 9 options (linked from `trip/aug_11_europe.html`):**

| Option | Where | Slug | Standard tier | New /39 | Old /39 | Differentiator |
|--------|-------|------|---------------|---------|---------|----------------|
| **C** | San Sebastián / Basque (Spain) | `aug_11_san_sebastian.html` | **$11,254** | **36** ⭐ | 32 | **Aste Nagusia Aug 8–15 lands inside trip** · fireworks 22:45 every night · up to 10 Michelin stars possible across 5 dinners · pintxos + txosnas = built-in nightlife · value pick at $12–15K |
| **I** | Côte d'Azur (France/Monaco) | `aug_11_cote_dazur.html` | **$25,000+** | **36** ⭐ | NEW | **3× ★★★ in 90 min** (Louis XV + Vague d'Or + Mirazur) · Cannes fireworks Aug 15 22:00 Finland team · Caves du Roy + Jimmy'z + Bâoli · glamour pick at $25–40K |
| **B** | Cascais / Guincho (Portugal) | `aug_11_cascais.html` | **$9,815** | **35** | 27 | **Biggest jump (+8)** · Lisbon ★★ ×3 (Belcanto/Henrique Sá Pessoa/Fifty Seconds) · Bairro Alto + Lux Frágil · Aug 15 Armand Van Helden DJ · Perseids Cabo da Roca · only US nonstop (TAP) |
| **F** | Mallorca / Deià + Palma (Spain) | `aug_11_mallorca.html` | **$17,050** | **34.5** | 30 | Belmond + Voro ★★ + Palma nightlife (Abaco + Santa Catalina + Tito's BCM + Purobeach) · 3 Palma + 2 Deià split recommended · 85–90°F · Cap Formentor road closed 10 AM–10 PM through Oct 18 |
| **E** | Annecy / French Alps (France) | `aug_11_annecy.html` | **$11,160** | **34** | **38** | **Old winner drops −4 on nightlife** · 13 stars / 7 restaurants in basin · Le Brise Glace closed Jul 10–Aug 24 · Fête du Lac Aug 1 missed · Fête des Guides Chamonix Aug 15 salvage anchor |
| **H** | Hvar + Split (Croatia) | `aug_11_hvar.html` | **$9,650** | **34** | NEW | Pakleni Islands sail + Vis Blue Cave + Brač Vidova Gora · Hvar Town nightlife to 5 AM · Krug ★ Split (only ★ in range) · 43% cheaper than Mallorca |
| **D** | Madeira / Funchal (Portugal) | `aug_11_madeira.html` | **$10,748** | **32.5** | 34 | Perseids above cloud sea Pico do Arieiro · Il Gallo d'Oro ★★ + William ★ + Desarma ★ · Belmond Reid's · **Wine festival starts Aug 27 — missed by 10 days** · nightlife real but small |
| **G** | Mykonos / Cyclades (Greece) | `aug_11_mykonos.html` | **~$15,000+** | **32** | NEW | Best beach-club nightlife in Med Aug (Scorpios/SantAnna/Cavo Paradiso · Diplo Aug 16 confirmed) · Greek meat tradition (Beefbar + Kiki's) · **no Michelin stars on island** · Meltemi cancels 30%+ boat days |
| **A** | Cassis / Provence (France) | `aug_11_provence.html` | **$9,580** | **31.5** | 31 | **Booked baseline** · La Villa Madie ★★★ + Bandol wines locked · Cassis quiet at night (last seatings 21:30) · Marseille nightlife requires 35-min drive · seafood-capital cuisine works against new brief |

**Recalibrated criteria (locked 2026-06-04):** Out: "less seafood" (demoted to soft modifier), "low crowds" (dropped — festivals are now a feature). In: "nightlife & late energy" (hard ×2), "activity density" (hard ×2). Reframed: "Michelin" → "Food caliber" (Michelin + late-dinner culture + non-seafood depth). Held: Weather (hard), Safety (hard), Wine (soft), Romance (soft). Scored on the hub at `#scoring`. Hard ×2, soft ×1. Max 39.

**Critical findings from research (2026-06-04 deep web research, 9 agents, ~80 tool calls each):**
- **🌑 Aug 12 2026 = total solar eclipse over northern Spain** — flight/hotel disruption risk for San Sebastián trip; SS is in deep-partial coverage zone, central Spain (Aragón/Castilla) on centerline.
- **Etxebarri ★ closed all of August** — confirmed from restaurant site; swap to Azurmendi ★★★ (Bilbao, 1h) for the wood-fire fix.
- **Cap de Formentor road closed 10 AM–10 PM May 15–Oct 18 2026** — kills the planned Perseids viewing at the lighthouse for Mallorca; substitute Mortitx / Coll de sa Batalla / Cap de ses Salines.
- **Plage Keller (Cap d'Antibes) closed for 2026 renovation** — operates as "La Piscine Keller" at Palm Beach Cannes (Côte d'Azur).
- **Madeira Wine Festival starts Aug 27** — we miss by 10 days; mitigate with Blandy's + Pereira d'Oliveira + Barbeito cellar visits.
- **Cannes International Fireworks Festival Aug 15 22:00** — Finland team (Joho Pyro) confirmed; free, La Croisette.
- **Diplo at Cavo Paradiso Sun Aug 16** — confirmed Mykonos late-Sunday anchor.

**Time-locked events shared across all 6 options:**

- **☄️ Perseid meteor shower peak** — night of Aug 12→13. Best vantage per option: Cap Canaille (Provence), Cabo da Roca (Cascais), Monte Igueldo (Basque), Pico do Arieiro (Madeira — the singular one, above the cloud sea), Col de la Forclaz (Annecy), Cap de Formentor lighthouse (Mallorca — road opens 10 PM, ideal for the 1–4 AM peak).
- **🎆/⛪ Aug 15 Assumption** — Catholic national holiday in France, Spain, Portugal. Each town has its own tradition; the Basque one (Aste Nagusia finale at La Concha) is the most spectacular fireworks; Mallorca = island-wide religious processions and "Els Llits de la Mare de Déu" displays, restaurants packed, coastal roads gridlocked.
- **🎵 Music festival** — Provence has Festival de La Roque d'Anthéron (through Aug 16); Basque has Aste Nagusia; Cascais has Festival de Sintra; Madeira's Wine Festival opens Aug 27 (just misses).

**Hub page recommendation (recalibrated 2026-06-04):** Per the new criteria, **San Sebastián (C) and Côte d'Azur (I) tie at 36/39** — the value pick (SS at $12–15K with Aste Nagusia overlay) vs. the glamour pick (Côte d'Azur at $25–40K with 3× ★★★ stacked). **Cascais (B, 35)** is the dark horse +8 jumper — Lisbon's three ★★ + Bairro Alto crawl + Lux Frágil + Perseids at Cabo da Roca with the only US nonstop. **Mallorca (F, 34.5)** rises on Palma's nightlife + beach-club density. **Annecy (E, 34)** — the old 38 winner — drops 4 on nightlife (Le Brise Glace closed all trip, Fête du Lac missed); still elite on food + activity if pure-nightlife isn't the dominant axis. **Provence (A, 31.5)** is the booked-default fallback.

**Open booking items (decision phase):**

- [ ] **Pick the destination by July 1, 2026.** Belcanto, Kappo, the 3-star Basque tables, and Voro ★★ all need 60–90 day lead time.
- [ ] **If swapping from Provence:** notify all booked vendors (hotel cancellation, La Villa Madie release, L'Eden Boat cancellation, winery calls). Most have 48-hour-out cancellation windows.
- [ ] **If staying with Provence:** complete the Trip No. 01 booking checklist above.
- [ ] **If picking Cascais (B):** book TAP TP224 (LAX→LIS nonstop), Fortaleza do Guincho hotel, Belcanto ★★ + Kappo ★ + Fortaleza ★.
- [ ] **If picking San Sebastián (C):** submit 3★ requests same day (Arzak + Akelarre + Berasategui + Azurmendi), book Maria Cristina (nights 1–3) + Akelarre (4–5).
- [ ] **If picking Madeira (D):** book Belmond Reid's Palace HB, Il Gallo d'Oro ★★, TAP LAX-LIS-FNC routing.
- [ ] **If picking Annecy (E):** book Swiss LX41 LAX→ZRH→GVA routing, La Maison Bleue (R&amp;C, 11 rooms, books fast), Le Clos des Sens ★★★ + Yoann Conte ★★ + Père Bise ★★, paragliding (Fly Annecy), Aiguille du Midi 9 AM slot. Note: Fête du Lac (Aug 1) is missed.
- [ ] **If picking Mallorca (F):** book Iberia IB6172 LAX→MAD + IB3946 MAD→PMI, Belmond La Residencia 5 nights in Deià (use Amex FHR 15% off July–Aug 2026 if booked by May 15), Voro ★★ in Canyamel (60+ day lead), Marc Fosh ★ Palma + Béns d'Avall ★ Sóller + DINS Santi Taura ★ Lloseta, Bodega Ribas + Macià Batle wine day with driver, Sa Calobra/Cap de Formentor driver day. Verify Cap de Formentor daytime road closure (10 AM–10 PM, Jun–Sept) one week out — affects Perseids routing.

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
cd /Users/markshors/embeddedLayers/jmark
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

The deploy *is* the source of truth as of 2026-06-02. Edit `/Users/markshors/embeddedLayers/jmark/trip/*.html` directly — there are no other canonical copies.

Pre-merge legacy copies are preserved (but no longer maintained) at:
- `/Users/markshors/embeddedLayers/jmark/.archive-pre-merge-2026-06-02/` — `basque-romance-aug.html`, `cascais-romance-aug.html`, `madeira-romance-aug.html`, `kern-trip.html` (predecessors to the `trip/aug_11_*` and `trip/jun_20_kern.html` files).
- `/Users/markshors/embeddedLayers/trip-aug-2026.html` — the previous Provence-only file at the repo root.
- `/Users/markshors/embeddedLayers/jmark/europe-aug-2026/` — scratchpad from the same merge session: a criteria-driven scoring matrix index across 6 candidate destinations. Not deployed; kept for reference if the hub page later wants a scoring-matrix enhancement.

---

## Quick context for a cold session

If a future Claude has read nothing else: **operator runs two active trip plans through this repo — a romantic 6-day Provence trip in August 2026 and a 2-day Kern River family weekend in June 2026. Both are planned, neither fully booked. Open items are mostly booking calls. The site is searchable by topic at https://mshors-pdai.github.io/jmark/ and has a STYLE.md for adding new trips. Stick to the durable preferences above.**
