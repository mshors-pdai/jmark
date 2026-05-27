# STYLE.md — jmark trip-plan style guide

A reference for building consistent, well-designed trip itineraries in this repo.
Read this before writing a new `trip/<slug>.html`.

> Last updated: 2026-05-27 · Based on `aug_11_provence.html` and `jun_20_kern.html`.

---

## Foundations

### Fonts
- **Display:** [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) — used for `h1`–`h4`, day numbers, hero titles, brand mark. Italic (`<em>`) used as the highlight color treatment.
- **Body:** [Inter](https://fonts.google.com/specimen/Inter) — used for paragraph text, eyebrows, nav, pills, tables, buttons.
- Load via Google Fonts CSS in `<head>`:
  ```html
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,800;1,400&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  ```

### Color system
Each trip gets its own **themed palette** plus the **shared neutrals**.

**Shared neutrals (every trip):**
```css
--ink: #1a1a1a;
--muted: #6b6b6b;
--line: rgba(0,0,0,0.08);
```

**Per-trip palette** — 4–5 named colors that tie to the destination. The pattern is "deep · accent · soft · cream":

- **Provence:** lavender / terra (rust orange) / olive / sky-blue / cream `#faf4e8`
- **Kern:** pine (deep green) / river (blue) / rust (CA orange) / sand / cream `#faf4e8`

Pick a primary accent that lives in the hero title `<em>`, eyebrow text, day numbers, CTA arrows, and the "tier badge" on cards. The deep color does headlines + dark sections. The soft color does badges + secondary highlights. Cream is the page background for hero sections.

### Eyebrow pattern
Short small-caps subtitle that appears above every section title:
```html
<span class="eyebrow">Day by Day</span>
<h2>The Itinerary</h2>
```
Styled: 0.75rem, uppercase, 0.2em letter-spacing, color = accent.

---

## Required sections (in order)

1. **Back-to-index bar** — dark `#1a1a1a` strip at the very top with `← All trips` linking to `../index.html` plus a mini brand mark linking back. See "Back bar" below.
2. **Sticky top nav** — section anchors as pills, themed border color.
3. **Intro hero** — eyebrow + `<h1>` with one or two italic `<em>` words + lede + 4–5 meta items in a horizontal strip.
4. **Index / TOC** — optional but recommended for longer plans. 3-column grouping (the plan / what you'll do / logistics) with numbered links.
5. **Hero destination card** — image + content side-by-side with a 4-stat row at the bottom (temp · crowd · signature · drive).
6. **Flight or drive box** — visual logistics: airport codes or city codes with a route line + transit mode + duration. Footer with 3 meta items.
7. **When to go / timing block** — calendar bar, candidate-date comparison, or special-event highlights.
8. **Day-at-a-glance table** — one row per day, columns: Day · Date · Theme · Highlight · Dinner.
9. **Day-by-day itinerary** — big italic Playfair number (`01`, `02`, …) on the left, date below, location pill + heading + bulleted timeline on the right.
10. **Theme deep-dives** — "wine block" / "off-road routes block" pattern: side-by-side image + 4-spec strip + bulleted notes + links.
11. **Maps section** — embedded OSM/Google maps with share-link buttons (Google Maps · Apple Maps · OSM · Copy link).
12. **Hotels / lodging grid** — 3 cards: image + tier badge + name + location + paragraph + price + book link.
13. **Activities grid** — 4-column emoji+link grid, each item is a 1-sentence pitch.
14. **Packing list** — 4-column checkbox grid (river / mountain / vehicle / kids — adapt to trip).
15. **Quick reference table** — every phone number and URL in one place.
16. **Research deep-links** — 6-column categorized link list for booking + verification.
17. **Booking checklist** — dark `#1a1a1a` section, numbered Playfair italic steps with "when" pill + link.
18. **Footer** — dark, with GitHub link + style guide link.

Skip what doesn't apply. A 2-day domestic trip doesn't need a flight box; a couples' trip doesn't need a kid-comfort packing column.

---

## Components

### Back-to-index bar (shared)
The dark bar above the sticky nav, on every trip page. Theme-color hover on the back link and dot.
```html
<div class="back-bar">
  <div class="container">
    <a href="../index.html" class="back-link"><span class="arrow">←</span> All trips</a>
    <span class="meta-mini">Itinerary No. NN · Trip Name</span>
    <a href="../index.html" class="brand-mini">j<span class="dot">.</span>mark</a>
  </div>
</div>
```

### Hero card
- 2-column grid, left = image with theme overlay, right = white card content.
- Stats row: 4 columns, Playfair value + small-caps label.
- Collapses to single column at 900px.

### Day timeline
- 180px left column with `.day-number .num` (4rem italic Playfair) + uppercase date below.
- Right column: location pill (themed background) + `h3` + `ul` of timeline items.
- Bullets are colored dots (theme accent).

### Hotel / lodging cards
- 220px image header with linear-gradient overlay + tier badge in top-right.
- Body: name + location line + paragraph + price + star rating.
- "Book direct" pill button (themed) + phone link + map share row (Google + Apple).

### Map share-row pattern
For every map-able location, three things:
1. An embedded OpenStreetMap iframe (`https://www.openstreetmap.org/export/embed.html?bbox=...&layer=mapnik&marker=...`)
2. A share button row with:
   - `Google Maps directions` (`https://www.google.com/maps/dir/from/to`)
   - `Apple Maps` (`http://maps.apple.com/?daddr=...&dirflg=d`)
   - `Open in OSM` (`https://www.openstreetmap.org/?mlat=..&mlon=..&zoom=..`)
   - `Copy share link` button (data-share attribute, JS clipboard handler at end of file)
3. A small-caps "Reach via" deep-link if applicable.

Always include the copy-to-clipboard toast snippet at the bottom of the file (see Kern file for working JS).

### Booking checklist (dark section)
- `background: #1a1a1a; color: white;`
- 9 or so numbered steps. Big italic Playfair number, "when" pill ("Now · top priority", "2 weeks out", "Day before"), `h4` title, short paragraph, meta line with `→ phone · link`.

---

## File conventions

### Slug
`trip/<month3>_<dd>_<destinationslug>.html`

Examples:
- `aug_11_provence.html`
- `jun_20_kern.html`

Use the **departure date** in the slug. For a multi-date trip with candidates, use the **recommended** date.

### Title tag
`<title>Month DD → DD, 2026 — Destination Theme</title>` or include recommendation in parens.

### Section ids
Every major section gets an `id` so the TOC and topnav anchors work:
`trip`, `timing`, `itinerary`, `routes`, `map`, `rafting` / `wine` / activity-specific, `lodging`, `truck` / `flight` / vehicle-specific, `packing`, `activities`, `reference`, `research`, `book`.

### Image sources (in order of preference)
1. **Wikipedia Commons** — verified by fetching the imageinfo API; canonical URL pattern `https://upload.wikimedia.org/wikipedia/commons/X/XX/Filename.jpg`. Use for landscapes, specific landmarks, vehicles.
2. **Unsplash** — pattern `https://images.unsplash.com/photo-<id>?w=1400&q=80`. Use for evocative generic shots (hotel interior, food, atmosphere). Verify the photo ID resolves before committing.
3. **Embedded gradient overlay** — always layer a `linear-gradient(135deg, rgba(theme1,0.2), rgba(theme2,0.3))` on top of every photo. Ties the photo to the trip's palette and softens distracting detail.

Never invent Unsplash photo IDs — they 404 and break the page. Search and verify first.

### External links
- Open in new tab: `target="_blank" rel="noopener"`
- Phone numbers: `<a href="tel:+17603763745">760-376-3745</a>`
- Map searches that fall back to a Google query: `https://www.google.com/maps/search/<+separated+name>`
- USGS gauges: `https://waterdata.usgs.gov/monitoring-location/<station_id>/`
- NWS point forecast: `https://forecast.weather.gov/MapClick.php?lat=<lat>&lon=<lon>`

---

## Mobile

### Breakpoints
- **900px:** hero card collapses, hotels grid → 2 col, day timeline number/content stack, wine block stacks
- **600px:** everything is 1 col; hero h1 shrinks; topnav becomes horizontal-scroll tabs

### Mandatory mobile rules in every trip
```css
@media (max-width: 600px) {
  .intro-hero h1 { font-size: 2.2rem; }
  .topnav .container { flex-direction: column; gap: 0.5rem; align-items: flex-start; }
  .topnav .tabs { width: 100%; overflow-x: auto; flex-wrap: nowrap; }
  .topnav .tab { white-space: nowrap; }
  h2 { font-size: 1.8rem !important; }
  h3 { font-size: 1.3rem; }
  .day-number .num { font-size: 2.5rem; }
  .container { padding: 0 1rem; }
  /* Catch-all for inline-styled 2-col grids */
  [style*="grid-template-columns: 1fr 1fr"] { grid-template-columns: 1fr !important; }
  [style*="grid-template-columns: repeat(3, 1fr)"] { grid-template-columns: 1fr !important; }
  [style*="grid-template-columns: 80px 1fr"] { grid-template-columns: 50px 1fr !important; gap: 0.85rem !important; }
}
```

If a section uses inline styles for grid layout (common for one-off blocks), give it a class so a targeted media query can override, OR rely on the attribute selectors above. Test in DevTools at 375px width before shipping.

### Tables on mobile
Wrap any table > 4 columns in `overflow-x: auto` and set `min-width: 540px` on the table itself so it scrolls horizontally instead of crushing.

---

## Index page conventions

Maintained at `/index.html`. Pattern:
- Sticky nav with brand mark + Trips · Style · GitHub
- Hero with `clamp()` `h1` and italic `<em>` accent words
- **Search input** with live filter + tag filter buttons
- Stats band (trips count · year · countries · next departure)
- Trip grid with `.trip-card.large` for featured trips, `.placeholder` for upcoming slots

### Adding a trip card to the index
Every trip card needs two data attributes for search/filter:
```html
<a href="./trip/jun_20_kern.html" class="trip-card large"
   data-search="kern river kernville california sherman pass off-road rafting family lickity split sequoia rivian r1t summer 2026"
   data-tags="2026 family california mountain">
```
- `data-search` — every keyword someone might type, lowercase, space-separated. Include place names, themes, activities, months, vehicle, traveler types.
- `data-tags` — match values from the filter pill buttons. Add new filter buttons to `#filters` if a new tag emerges.

After adding a card, bump the `#stat-trip-count` stat number and update the "Year" / "Countries" / "Next departure" stats if relevant.

---

## Voice + content

- **Opinionated, not exhaustive.** Pick the right option, explain why, and rank backups. Don't list 15 hotels — list 3.
- **Honest about trade-offs.** When a date or hotel has a downside, say it.
- **Concrete URLs and phone numbers** beat generic "search Google" advice — but use a Google search link when the official site is unreliable.
- **No "per person"** in budget breakdowns. State the all-in total.
- **Verify URLs before adding them.** Search for the official site rather than guessing. Test with a `curl -I`.
- **Real research, real numbers.** When asserting weather, flow, prices, dates — pull the data from a primary source and cite the link.
- **Italic `<em>` for emotional accents in the hero** — one or two words per title, never more.

---

## Deploy

```bash
cd /tmp/jmark-deploy
# edit files...
git add .
git -c user.email="mshors-pdai@users.noreply.github.com" \
    -c user.name="mshors-pdai" \
    commit -m "<change>"
git push origin main
# verify
curl -s -o /dev/null -w "%{http_code}\n" https://mshors-pdai.github.io/jmark/
```

Live site: <https://mshors-pdai.github.io/jmark/>
