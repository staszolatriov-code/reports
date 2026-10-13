# SEO Page Builder — Earnings Calendar

**Date:** 2026-10-13
**Opportunity:** `earnings calendar` cluster
**Why today:** Q3 2026 earnings season officially opens this week with the big US banks (JPM, Wells, Citi) reporting Oct 14–15, followed by Netflix, Tesla, and the mega-cap tech print the following week. Search volume for "earnings calendar" and tail terms ("earnings this week", "earnings today", "earnings next week", "{ticker} earnings date") spikes 3–5x during the first two weeks of each earnings season. This is the single most time-sensitive, highest-intent moment of the quarter for this cluster.

---

## 1. Page Thesis

TipRanks' `/earnings-calendar` should be the live, filterable, personalized earnings radar that institutional-grade retail traders use to plan the week — not a static grid dump. It is for self-directed investors who want to decide *which* earnings to trade, not just which companies are reporting. It deserves to rank because every incumbent treats this as a commodity table with ticker, date, EPS estimate — none of them attach **analyst track-record accuracy, Smart Score, hedge-fund positioning changes going into print, or insider activity in the last 30 days**, which is exactly the context that converts a glance into a trade thesis. It converts because the free table is a credible hook, and the "pre-earnings signal stack" (locked analyst accuracy, locked hedge-fund 13F deltas, locked AI pre-earnings summary) is the natural premium wall.

## 2. Search Intent Breakdown

- **Primary intent:** "What is reporting today / this week, and when (BMO/AMC)?" — fast, scannable schedule lookup.
- **Secondary intent:** "Which of these prints actually matters, and how is it likely to go?" — context, estimates, revisions, positioning.
- **What users really want:** a watchlist-aware calendar that filters to *their* names, flags unusually risky prints (big implied move, big analyst estimate dispersion, recent insider selling), and lets them queue reminders.
- **Bounce triggers:** stale date (yesterday's earnings still above fold), no BMO/AMC split, no implied-move column, no filter, slow load, forced login before seeing the grid, ad-choked layout (MarketBeat's failure mode).

## 3. 10x Page Blueprint

- **Page type:** Dynamic, programmatic hub page (`/earnings-calendar`) with sub-templates per view (today / this-week / next-week / by-sector / by-market-cap) and per-ticker spoke pages (`/stocks/{ticker}/earnings-date`).
- **Title tag:** `Earnings Calendar Today & This Week (Oct 2026) — Analyst Accuracy, Smart Score, Hedge Fund Moves | TipRanks` (58 chars for primary variant; template auto-rotates "Today / This Week / Next Week" based on the view).
- **Meta description:** `Live earnings calendar for Oct 13, 2026. See who's reporting BMO/AMC with EPS and revenue estimates, analyst track-record accuracy, Smart Score, hedge-fund positioning changes, and implied move. Filter by your watchlist.`
- **H1:** `Earnings Calendar — Who's Reporting This Week`
- **H2 / H3 outline:**
  - H2 `Earnings This Week (Oct 13–17, 2026)` — the primary interactive table
  - H2 `Highlighted Reports` — curated 3–5 cards for the week's most-watched names, auto-selected by weighted market cap + search volume + Smart Score change
    - H3 one card per highlighted ticker
  - H2 `How to Read an Earnings Print on TipRanks`
    - H3 `Analyst estimate accuracy — not all estimates are equal`
    - H3 `Smart Score going into print`
    - H3 `Hedge-fund positioning in the last 13F cycle`
    - H3 `Insider activity in the 30 days before earnings`
    - H3 `Options-implied move vs. historical realized move`
  - H2 `Earnings Calendar by Date`
    - H3 `Earnings Today` (link to `/earnings-calendar/today`)
    - H3 `Earnings Tomorrow`
    - H3 `Earnings Next Week`
  - H2 `Earnings Calendar by Sector` (links to sector-filtered views)
  - H2 `Confirmed vs. Estimated Earnings Dates`
  - H2 `Frequently Asked Questions` (FAQ schema)
- **Recommended modules:**
  - Live earnings grid with sticky column headers and column-based filters
  - Watchlist overlay toggle ("Only show my tickers")
  - "Pre-earnings signal stack" row expand — one click reveals analyst accuracy, Smart Score, 13F delta, insider activity, implied move
  - "After the bell" strip at the top during AMC window (6:00–8:00 PM ET) showing live beats/misses as results drop
  - Email + push alert signup inline ("Alert me 30 min before {ticker} reports")
  - Earnings-season heatmap: compressed 4-week view by sector
- **Interactive components:**
  - Column sort on every metric (date, time, market cap, EPS surprise history, implied move, Smart Score)
  - Multi-select filters (market cap buckets, sectors, Smart Score ≥ 8, confirmed-only, has-options)
  - Save-filter-as-view (requires free login — the first real auth hook)
  - Expand-row inline chart (last 8 quarters: estimate vs. actual EPS + revenue, with 1-day post-earnings move)
- **Visual / data components:**
  - EPS beat/miss sparkline per row (last 8 quarters, encoded by TipRanks' palette — green beat, red miss, size by surprise magnitude)
  - Implied move pill (color-ramped: green <3%, amber 3–7%, red >7%)
  - BMO / AMC icon in the time column (sun / moon), not a text string
  - "Why it matters" hover card on each highlighted ticker: 2-sentence AI-generated setup summary
- **Schema opportunities:**
  - `FinancialProduct` → `Corporation` for each ticker row (with `tickerSymbol`, `earningsAnnouncement`)
  - `Event` schema per earnings event with `startDate`, `eventStatus` (confirmed vs. estimated), `location: online`
  - `FAQPage` schema on the FAQ block
  - `BreadcrumbList`
  - `ItemList` wrapping the main grid for rich-result eligibility
- **Internal linking strategy:**
  - Each ticker row → `/stocks/{ticker}` and the dedicated `/stocks/{ticker}/earnings-date` spoke
  - Highlighted-ticker cards → `/stocks/{ticker}/smart-score`, `/stocks/{ticker}/analyst-forecast`, `/stocks/{ticker}/hedge-fund-activity`
  - Sector blocks → sector hub pages
  - "How to read a print" H3s → evergreen explainer pages (analyst track record, Smart Score methodology, 13F explainer)
  - Reciprocal: every `/stocks/{ticker}` page already carries an "Earnings" tab that back-links to this calendar

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast, well-designed static table. Date, time, EPS estimate, revenue estimate. That's it.
- *Where they're weak:* No positioning context (no hedge funds, no insiders, no analyst accuracy), no watchlist overlay, no post-print follow-up, no alerts. It's a reference, not a workflow.
- *How TipRanks beats them:* We keep their clarity but layer the signal stack. Match their load speed and column discipline; add context they structurally don't have.
- *Above the fold:* Smart Score column + Analyst Accuracy column (both unique to us).

**Barchart.com**
- *What they do:* Deep data, including surprise history and estimate counts. Power-user feature set.
- *Where they're weak:* UI is cluttered, modal-heavy, and gates meaningful features behind a paid tier early. Mobile is punishing. No proprietary scoring.
- *How TipRanks beats them:* Modern, mobile-first table; equal or better data density without the modal maze. Our Smart Score is a cleaner anchor than their raw ratings aggregation.
- *Above the fold:* Mobile-usable grid + Smart Score; "Pre-earnings signal stack" that doesn't exist on their page at all.

**MarketBeat.com**
- *What they do:* Volume play — thin pages per ticker/day, aggressive AdSense, heavy email capture.
- *Where they're weak:* Ad load degrades Core Web Vitals; data is shallow; "analyst ratings" column is unweighted and misleading; thin content gets outranked once Google notices usefulness signals.
- *How TipRanks beats them:* We weight analyst calls by individual track-record accuracy — the single most defensible SEO moat we have on this cluster. Ship a 90+ Lighthouse score to flip the UX comparison.
- *Above the fold:* Analyst Accuracy % (visible on every row), minimal ads, no email-wall interstitial.

## 5. Conversion Strategy

- Free tier shows: full calendar, EPS/revenue estimates, Smart Score numeric value, implied move, basic sort/filter. Enough to be the daily default.
- Premium wall sits on the "expand row" interaction: analyst accuracy breakdown by individual analyst, full 13F delta for the ticker, insider activity ledger, AI pre-earnings summary.
- Primary CTA: inline "Unlock the full pre-earnings stack" button inside the expanded row, in-context — not a sidebar banner.
- Secondary CTA: free-account hook for "Save filter as view" and "Alert me 30 min before this prints" (lower friction, high retention value, builds email list for the earnings-recap email sequence).
- Trust elements above the fold: "Analyst accuracy backed by 15+ years of tracked calls" micro-badge; count of total analyst calls tracked; "Updated 2 min ago" freshness stamp.
- Engagement module: live post-earnings strip (BMO window 7:30–9:30 AM ET and AMC window 4:00–6:00 PM ET) — reason to keep the tab open all day.
- Social proof: compact "Top-rated analysts going into this print" chip row per highlighted card, linking to their track-record page.
- Upgrade hook timing: after a free user has saved 2+ tickers or expanded 3+ rows in a session, show a one-time inline upsell card ("You're clearly researching earnings — Premium unlocks the full stack for every ticker").

## 6. Editorial Guidance

- Tone: trader-literate, not finance-blog breezy. "BMO/AMC", "implied move", "revisions ratio" without being over-explained — but hover definitions available for newer readers.
- Depth: the week's highlighted-ticker cards each carry a 60–90 word pre-earnings setup written by a credentialed TipRanks analyst or editor (byline required). Everything else is data-driven.
- Freshness: data refreshes every 15 minutes during market hours, every 60 minutes off-hours; editorial setups refresh at least daily during earnings season, twice weekly off-season. Mark `dateModified` in schema.
- E-E-A-T signals: visible byline + credentials on every highlighted-ticker setup, methodology links (Smart Score, analyst accuracy) one click away, data-source footer ("Earnings dates sourced from company IR filings and confirmed by TipRanks data operations").
- Avoid: generic earnings-season "what to expect" filler, horoscopic predictions, clickbait "will beat / will miss" headlines. We own context, not predictions.
- Compliance: no implied investment advice; frame everything as "pre-earnings signals to weigh", not "buy/sell before earnings".

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Evergreen high-volume cluster with recurring quarterly spikes; competitors are all weak on quality signals; Smart Score and analyst accuracy give defensible rich-content moat. |
| Business upside | 5 | Highest-intent audience in the funnel — traders active during earnings season are the most likely to convert to Premium. Pre-earnings signal stack is the strongest premium wall on the site. |
| UX complexity | 3 | Dense table with filters, expand rows, watchlist overlay, and live refresh. Known patterns, but mobile needs real care. |
| Engineering complexity | 4 | Live data pipeline (earnings dates + confirmations + consensus + 13F delta + insider feed + options IV for implied move), BMO/AMC-aware refresh cadence, schema generation per row, alerting infra. |
| Recommended rollout speed | 5 | Ship v1 before the Q3 2026 heavy weeks (Oct 20–31): grid + Smart Score + analyst accuracy + implied move + expand-row premium wall. Highlighted-ticker editorial cards + live post-earnings strip + alerts can follow in v1.1 within the same quarter. |
