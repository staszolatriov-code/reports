# SEO Page Builder — 2026-09-15

**Selected opportunity:** Earnings Calendar

**Why today:** Q3 2026 earnings season kicks off in ~3 weeks (mid-October). Search volume for "earnings calendar," "earnings this week," and "earnings today" begins its seasonal ramp in mid-September and peaks the week banks report. Building/refreshing the hub now captures rising volume before the peak and lets us rank for the sub-cluster of ticker-level "when does $TICKER report" queries.

---

## 1. Page Thesis

TipRanks' Earnings Calendar is the destination for anyone deciding *what to trade around earnings this week*. It serves active retail investors and options traders who need not just a date grid, but the four questions no competitor answers in one view: **who's reporting, what analysts expect, how they've done historically, and how the Smart Score reads the setup**. It deserves to rank because we can layer analyst-track-record–weighted EPS/revenue consensus onto the standard calendar and expose expected move + post-earnings drift patterns. It converts because the natural next click — "see the full pre-earnings dossier for $NVDA" — is a gated Smart Score / Analyst Forecast deep-dive.

## 2. Search Intent Breakdown

- **Primary intent:** Find which companies report on a specific date/week (calendar lookup, high recurrence).
- **Secondary intent:** Assess whether an upcoming report is a *tradeable* event — beat/miss odds, implied move, historical reaction.
- **What users really want:** A ranked shortlist ("what actually matters this week") plus a way to filter by their watchlist, sector, or market cap — not a 400-row unfiltered dump.
- **What makes them bounce:** Slow load, ad-heavy layout, dates without consensus numbers, no filtering, or a paywall on the calendar itself (only the deep-dive should be gated).

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (`/earnings-calendar`) with dynamic sub-pages (`/earnings-calendar/[date]`, `/earnings-calendar/week/[isoweek]`, `/stocks/[ticker]/earnings`).
- **Title tag:** `Earnings Calendar 2026 — This Week's Earnings Reports & EPS Estimates | TipRanks`
- **Meta description:** `See every company reporting earnings this week with analyst-weighted EPS & revenue estimates, expected move, Smart Score, and historical beat rate. Free earnings calendar updated live.`
- **H1:** `Earnings Calendar — Reports This Week`
- **H2/H3 outline:**
  - H2: This Week at a Glance (Mon–Fri strip with count + notable tickers)
  - H2: Full Earnings Calendar (the interactive table)
    - H3: Filter by date, sector, market cap, index, watchlist
  - H2: Top 10 Most-Watched Reports This Week (editorial + algorithmic)
  - H2: How to Read an Earnings Report on TipRanks (short educational block, once)
  - H2: Post-Earnings Drift & Historical Beat Rates (methodology + link out)
  - H2: Earnings Calendar FAQ (structured Q&A)
- **Recommended modules:**
  - Live calendar table (date, ticker, company, BMO/AMC, EPS est. vs. prior, revenue est. vs. prior, expected move %, Smart Score, analyst consensus rating, prior 4-quarter beat rate).
  - "Analyst Track-Record–Weighted Consensus" toggle (our differentiator vs. flat consensus).
  - Watchlist filter (logged-in users see their tickers first — soft conversion for signup).
  - Sector heatmap of the week.
  - Notable reports rail with Smart Score badges.
- **Interactive components:**
  - Column-sortable, sticky-header table with virtualized rows (handles 500+ names).
  - Date-picker + weekly/monthly toggle; URL-persistent filters for shareability.
  - "Add to my calendar" (.ics export) per row.
  - Hover-card previews: 1-year price chart + last 4 EPS surprises without leaving the page.
- **Visual/data components:**
  - Expected-move bar (options-implied %) rendered inline.
  - Prior-4Q beat/miss dot strip per ticker.
  - Smart Score badge (color-coded 1–10).
  - Sector heatmap (report count + weighted market cap).
- **Schema opportunities:**
  - `ItemList` for the calendar rows.
  - `Event` schema per earnings release (`name`, `startDate`, `organizer`).
  - `FAQPage` on the FAQ block.
  - `BreadcrumbList` for date/week sub-pages.
  - `Dataset` on the calendar itself (methodology + last-updated).
- **Internal linking strategy:**
  - Every ticker row → `/stocks/[ticker]/earnings` (the deep-dive money page).
  - Cross-links to Analyst Forecast, Smart Score, Insider Trading, and Hedge Fund Activity for each ticker.
  - Sector rows link to sector overview pages.
  - Weekly recap posts link back into the hub for freshness/topical authority.
  - Homepage + "Tools" nav slot for site-wide equity.

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast earnings calendar with EPS/revenue estimates and surprise history.
- *Where they're weak:* No analyst-track-record weighting, no proprietary composite score, no expected-move data, no watchlist personalization, thin editorial layer.
- *How TipRanks beats them:* Track-record–weighted consensus + Smart Score + expected move + watchlist filter surface the *decision*, not just the data.
- *Above the fold:* Smart Score badge, analyst-weighted EPS delta vs. consensus, expected move %.

**Barchart.com**
- *What they do:* Dense, powerful calendar with options overlays; strong for pros.
- *Where they're weak:* Cluttered UI, paywalls on core filters, no analyst reputation layer, weak mobile experience, no "why this matters" editorial curation.
- *How TipRanks beats them:* Cleaner UX with the pro-grade data (implied move, historical drift) kept free, plus the human-readable Smart Score.
- *Above the fold:* Curated "Top 10 this week" rail + one-click watchlist filter.

**MarketBeat.com**
- *What they do:* SEO-heavy earnings pages, lots of AdSense, decent estimate coverage.
- *Where they're weak:* Ad density hurts UX and Core Web Vitals; no proprietary scoring; consensus is flat (all analysts weighted equally); email-gated tools.
- *How TipRanks beats them:* Ungated calendar, minimal ads, proprietary Smart Score, and hedge fund / insider signals that MarketBeat can't match.
- *Above the fold:* Hedge fund activity + insider trades badges alongside consensus — signals nobody else surfaces on a calendar row.

## 5. Conversion Strategy

- Keep the calendar itself 100% free (indexability + trust); gate the per-ticker *pre-earnings dossier* behind Premium.
- Inline "Unlock full analyst breakdown for $NVDA" CTA on hover-card, with 1 free unlock per session as a taste.
- Persistent right-rail: "Save this filter to your watchlist" — free signup gate, feeds email nurture.
- Weekly "Earnings Week Ahead" email opt-in above the fold (top-of-funnel capture).
- Trust elements: "Data updated 4× daily," analyst count per ticker, sourced-from-filings badge, methodology link.
- Social proof: "12,438 investors tracking $NVDA earnings" (counter, live).
- Post-earnings return visit: auto-email subscribers a "How your watchlist reported" recap Monday morning.
- Upgrade hook: "See which hedge funds bought $TICKER before last earnings" — links to 13F module, Premium.

## 6. Editorial Guidance

- Tone: neutral, data-first, second-person ("here's what to watch"). No hype, no clickbait tickers.
- Depth: calendar hub stays scannable; depth lives in the per-ticker sub-pages and the weekly recap posts.
- Freshness: calendar refreshed 4×/day from filings + IR pages; "This Week" curation republished every Sunday 18:00 ET and Wednesday 06:00 ET.
- E-E-A-T — Experience: cite analyst names + track records inline (our moat).
- E-E-A-T — Expertise: byline weekly recap by a named TipRanks analyst with author schema.
- E-E-A-T — Trust: visible "Last updated" timestamp, methodology page linked from the FAQ, corrections policy in footer.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Evergreen seasonal spikes 4×/year; strong featured-snippet + PAA capture on "earnings this week"; enormous long-tail via `/stocks/[ticker]/earnings`. |
| Business upside | 4 | High-intent traffic that converts to Premium via ticker deep-dives and weekly email; lifts session depth site-wide. |
| UX complexity | 3 | Table virtualization, filter persistence, and hover-cards are non-trivial but well-scoped. |
| Engineering complexity | 3 | Data pipeline (filings + consensus + options IV + track-record join) is the real work; front-end is standard. |
| Recommended rollout speed | 5 | Ship v1 within 2 weeks to catch Q3 season; iterate filters and email in v1.1. Phase gates: v1 = free calendar + Smart Score column; v1.1 = watchlist + email; v1.2 = expected move + drift analytics. |
