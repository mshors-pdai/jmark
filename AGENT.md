# AGENT.md — Trip Planning Context

> Handoff doc for future Claude sessions. Read this first.
> Last updated: 2026-05-26

## What this repo is

`jmark` is **Mark Shors' personal travel index**, hosted on GitHub Pages.

- **Live site:** https://mshors-pdai.github.io/jmark/
- **Repo:** https://github.com/mshors-pdai/jmark
- **Deploy:** GitHub Pages from `main` branch, root `/`. Push to update.
- **Local working copy:** `/tmp/jmark-deploy/` on the operator's MacBook.
  Note: `/tmp` survives only until reboot — if missing, `gh repo clone mshors-pdai/jmark /tmp/jmark-deploy` to restore.

### Structure

```
jmark/
├── index.html                       # Trip index landing page
├── trip/
│   └── aug_11_provence.html         # First (and only) itinerary so far
└── AGENT.md                         # This file
```

Future trips go in `/trip/<slug>.html` and get a card added to `index.html`.

---

## The trip · Cassis & the Calanques

**Status:** planned, not yet booked
**Dates:** Tue Aug 11 → Mon Aug 17, 2026 (6 days, **5 hotel nights**)
**Origin:** LAX
**Travelers:** 2
**Selected tier:** Standard (~$9,580 total all-in)

### Selected logistics (operator decisions)

| What | Choice | Notes |
|------|--------|-------|
| Flight | **Air France AF65** LAX→CDG→MRS · Aug 11 1:40 PM dep · arrives MRS **1:05 PM Aug 12** | Daytime departure chosen specifically to land at lunch, not midnight |
| Hotel (all 5 nights) | **The Address Cassis** | Adults-only 5-star boutique, hillside, ~€420–€680/night |
| Big dinner | **La Villa Madie ★★★** (Day 3 · Fri Aug 14) | Now 3 Michelin stars (promoted 2022). Book 60+ days ahead. |
| Boat | **L'Eden Boat private RIB · 6h · Day 2** | Aug 13 morning, before crowds |
| Wineries | 4: Clos Sainte Magdeleine, Domaine du Bagnol, Domaine Tempier, Château de Pibarnon | All require phone appointments |

### Time-locked events on these exact dates

- **☄️ Perseid meteor shower peak** — night of Aug 12→13. 2026 is the **best Perseid year of the decade** (new moon Aug 12 = moonless sky, 90+ meteors/hour). Day 1 itinerary includes a late-night Cap Canaille viewing.
- **🎆 Aug 15 Assumption Day** — Cassis throws its biggest party. Apéro 7 PM, fireworks 10 PM, ball 10:30 PM at Place Baragnon. Day 4 is built around this — no out-of-town trips Saturday.
- **🎹 Festival de La Roque d'Anthéron** — world's largest piano festival, runs through Aug 16. Optional Day 5 alternative.
- **🎨 Cassis Night Market & Quai des Artistes** — every evening 7 PM–midnight, June 25 → Aug 31.

---

## Operator preferences (durable — apply to future trips too)

These were extracted from the iterative back-and-forth. Treat as constraints unless explicitly relaxed.

1. **Weather sweet spot: 75–80°F highs.** Above 82°F is "too hot." Below 70°F is "too cold."
2. **Crowds: low.** Will skip a famous place if it's a zoo in peak season. Cassis was acceptable only because we engineered around the crowds (early boat, sunrise hikes, weekday wineries).
3. **No bugs.** Tropical destinations with mosquito pressure are out. Mediterranean dry climates are fine.
4. **Hotels: $500–$1,000/night.** Splurge tier was rejected for Belmond La Residencia ($1,400+) as out of range. Will flex up by ~$200/night for an iconic property; will not flex up by $400+.
5. **≤ 2 hotels total across a trip.** No nightly changes. One base preferred if drives allow.
6. **≤ 1.5 hour drives.** Originally 1 hour, relaxed to 1.5h. Anything beyond is a "long day trip" with caveats.
7. **Arrival time at destination: ~1 PM ideal.** Wants the first day usable — lunch + first swim, not just checking in at midnight.
8. **Wine matters.** Trip is built around wine experiences. Researched, named wineries with appointments — not "stop by random tasting rooms."
9. **Food matters.** Always at least one Michelin-tier dinner. Local seafood emphasized.
10. **Nightlife: lively dinners + wine bars OK, clubs not necessary.** Wants late dinners and the option of a port-side cocktail at 11 PM, not a 4 AM rave.
11. **Romance is the through-line.** Trip is a couples' escape.
12. **Skip lavender expectations in August** — fields cut by mid-July except Sault (which is 2h+ away).

### Communication preferences

- **Terse responses; no unnecessary preamble.** Operator pushes back on long explanations.
- **Concrete options with prices/URLs > abstract recommendations.**
- **Be honest about trade-offs.** When operator's constraints conflict, surface the conflict.
- **Web research expected** when there's any doubt about prices, hours, or current status. Operator explicitly asked for "actual research."
- **Verify URLs before adding them.** When adding links, search for the official site rather than guessing the URL pattern.
- **Don't say "per person"** in budget breakdowns. (Operator preference, stated explicitly.)

---

## Decision history (why we landed where we did)

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

**Why not Galicia (even though it fit most criteria):** operator wanted nightlife the Galician model doesn't deliver, and the "warm sea swim" expectation was a quiet priority.

**Why Provence won:** dramatic scenery (Calanques), serious wine (Cassis AOC + Bandol), cleanest hit on the $500–1000 hotel budget, earliest LAX-to-Europe daytime arrival (1:05 PM at MRS via AF65), and a single hotel works.

---

## Open items / not yet done

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

## How to update the site

```bash
# 1. Edit locally
cd /tmp/jmark-deploy
# ...edit trip/aug_11_provence.html or index.html...

# 2. Commit and push
git add .
git -c user.email="mshors-pdai@users.noreply.github.com" \
    -c user.name="mshors-pdai" \
    commit -m "<change description>"
git push origin main

# 3. Verify deploy (~30s)
curl -s -o /dev/null -w "%{http_code}\n" https://mshors-pdai.github.io/jmark/
```

### To add a new trip

1. Create `trip/<slug>.html` (mirror the structure of `aug_11_provence.html`)
2. Add a `<a class="trip-card">` to the grid in `index.html`
3. Bump the stat counter at the top of `index.html`
4. Commit + push

### To take the site down

```bash
gh repo delete mshors-pdai/jmark --yes
```

---

## Source files

- **Canonical local edit copy:** `/Users/markshors/embeddedLayers/trip-aug-2026.html` — operator edits here first, then we sync to `/tmp/jmark-deploy/trip/aug_11_provence.html`.
- **Deploy copy:** `/tmp/jmark-deploy/trip/aug_11_provence.html` — what GitHub sees. Keep these in sync.

The two-file workflow exists because the local file was written before the deploy structure was set up. If a future session wants to simplify, it can edit the deploy copy directly and delete the embeddedLayers copy.

---

## Quick context for a cold session

If a future Claude has read nothing else: **operator is planning a romantic 6-day Provence trip in August 2026, has selected The Address Cassis hotel + La Villa Madie 3-Michelin restaurant, and the page lives at https://mshors-pdai.github.io/jmark/trip/aug_11_provence.html. Open items are mostly booking calls. Stick to the durable preferences above.**
