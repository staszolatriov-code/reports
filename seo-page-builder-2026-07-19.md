# SEO Page Builder — 2026-07-19

**Selected opportunity cluster:** `earnings calendar`

**Why today:** Q2 2026 earnings season is at peak volume this week (mega-caps reporting Mon–Fri). Search demand for "earnings calendar," "earnings this week," and ticker-specific "AAPL earnings date"-style queries is at its quarterly high. A best-in-class calendar hub compounds seasonal traffic four times per year and captures ticker-level intent that funnels into TipRanks' stock pages.

---

## 1. Page Thesis

TipRanks' **Earnings Calendar Hub** is a live, filterable, forecast-rich event tracker that turns the flat "what's reporting this week" query into an actionable pre- and post-earnings workflow. It targets active retail investors, options traders, and news-driven momentum traders who need to see *what's reporting, what analysts expect, how the stock has behaved historically around earnings, and what happened after the print* — all in one place. It deserves to rank because competitors publish sortable tables; TipRanks publishes a **Smart Score-graded, analyst-track-record-weighted, whisper-vs-consensus, EPS-surprise-history** calendar. It converts because each row is a doorway into a Premium-gated pre-earnings brief (analyst accuracy on this exact ticker, hedge-fund positioning changes into the print, insider selling in the 30 days prior).

## 2. Search Intent Breakdown

- **Primary intent:** "What companies are reporting earnings today / this week / next week?" — a scannable, filterable, date-ranged list.
- **Secondary intent:** Pre-earnings prep for a specific ticker (consensus EPS, whisper number, implied move, historical beat rate, price action ±1 day).
- **What users really want:** A defensible edge — "who's likely to beat, who's likely to miss, and how should I position?" — not just a schedule.
- **What makes them bounce:** Login walls on the calendar itself, stale/missing confirmed dates, no timezone handling, no BMO/AMC labeling, no filters for market cap or sector, and calendars that don't link out to a real research page per ticker.

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (calendar template) with per-ticker earnings sub-pages as programmatic children (`/earnings-calendar/[ticker]`).
- **Title tag:** `Earnings Calendar 2026 — Confirmed Dates, EPS Estimates & Smart Score | TipRanks` (58 chars visible portion)
- **Meta description:** `Track every U.S. earnings report with confirmed dates, analyst consensus EPS, whisper numbers, historical surprise rates, and Smart Score. Filter by day, sector, and market cap.` (177 chars)
- **H1:** `Earnings Calendar — Reports This Week`
- **H2/H3 outline:**
  - H2: This Week's Earnings (default view, current week)
    - H3: Monday BMO / Monday AMC / Tuesday BMO … (day-part grouping)
  - H2: Confirmed vs. Estimated Report Dates (freshness signal)
  - H2: Biggest Movers Expected — Highest Implied Moves
  - H2: Top Smart Score Companies Reporting This Week
  - H2: Analyst Sentiment Into Earnings (aggregate ratings drift, last 30 days)
  - H2: Hedge Fund & Insider Activity Ahead of Print
  - H2: Last Week's Earnings Recap — Beats, Misses, Reactions
  - H2: How to Use TipRanks Before an Earnings Report (workflow explainer)
  - H2: Earnings Calendar FAQ
- **Recommended modules:**
  - Sticky top filter bar: date range, sector, market cap, Smart Score threshold, "confirmed only" toggle, "has options" toggle, timezone selector
  - Row-level expandable drawer: consensus EPS, revenue, whisper, YoY, last-4-quarter beat/miss pattern, implied 1-day move from options, top analyst's forecast + their track record
  - "Reporting after the bell today" pinned widget
  - Post-earnings reaction ticker (live during earnings weeks)
  - Save-to-Watchlist per row (logged-in hook)
- **Interactive components:**
  - Column sort on every metric; multi-column filter persistence via URL params (SEO-shareable views)
  - Ticker hover-card with mini Smart Score gauge + last 4 quarters bar chart
  - "Set alert for this print" (email/push, converts anonymous → registered)
  - Comparative select: check 2–3 rows → side-by-side pre-earnings compare card
- **Visual/data components:**
  - Heatmap grid: sector × day-of-week showing report density
  - Sparkline per row: last-8-quarters EPS surprise (green/red)
  - Implied move donut vs. historical realized move (calibration signal)
- **Schema opportunities:**
  - `Event` schema per earnings event (name, startDate, organizer, eventStatus, offers optional)
  - `FAQPage` for the FAQ section
  - `BreadcrumbList`
  - `ItemList` for the primary calendar table
  - `Dataset` schema for the aggregate calendar (helps Google Dataset Search)
- **Internal linking strategy:**
  - Every ticker row → deep link to `/stocks/[ticker]/earnings` (dedicated earnings history + forecast page)
  - Every sector filter → `/sectors/[sector]/earnings-calendar` programmatic pages
  - Hub links up to `/earnings` (parent) and cross-links to `/analyst-ratings`, `/insider-trading`, `/hedge-funds` filtered to "activity in past 30 days for tickers reporting this week"
  - Related pages sidebar: "Dividend Ex-Dates This Week," "IPO Calendar," "Economic Calendar" (build an event-hub cluster)

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- **What they do:** Clean, fast calendar table with confirmed/estimated status, EPS estimate, prior EPS, market cap, and time (BMO/AMC).
- **Where they're weak:** No analyst quality overlay, no whisper number, no options-implied move, no post-earnings reaction data, no per-analyst track-record context, weak logged-in engagement layer.
- **How TipRanks beats them:** Layer Smart Score, top-analyst forecasts weighted by historical accuracy, and hedge-fund/insider activity into the print onto every row — StockAnalysis stops at consensus; TipRanks tells you which analysts to trust and who's positioning ahead of the print.
- **Above the fold:** Smart Score column, "Top Analyst Estimate vs. Consensus" delta column, "Insider Selling Last 30 Days" flag icon.

**Barchart.com**
- **What they do:** Dense, professional-trader calendar with heavy options data (implied move, IV rank), sortable multi-column tables.
- **Where they're weak:** UI is dated and intimidating for retail; no analyst track-record context; no narrative synthesis; premium wall obscures much of the value; weak mobile experience.
- **How TipRanks beats them:** Keep Barchart's options-implied-move data but pair it with retail-friendly Smart Score + one-line AI-generated pre-earnings synthesis ("Consensus $2.14; top-ranked analyst on this stock (73% accuracy) forecasts $2.28; hedge funds added 4.2M shares last quarter"). Modern, mobile-first UI.
- **Above the fold:** Implied move column + Smart Score + AI pre-earnings blurb — Barchart makes you dig for context; TipRanks surfaces it.

**MarketBeat.com**
- **What they do:** Popular earnings calendar with ratings-change context and email newsletter cross-sell.
- **Where they're weak:** Ad-heavy, editorial-first not data-first, no proprietary scoring, thin per-analyst credibility data, tables are basic sortable HTML with limited filtering.
- **How TipRanks beats them:** Proprietary Smart Score is the moat MarketBeat lacks; TipRanks' analyst accuracy database gives real weight to "who upgraded ahead of earnings" — MarketBeat lists ratings changes flat; TipRanks tells you whether the analyst making the change has been right 71% of the time or 34%.
- **Above the fold:** Smart Score + "Top Analyst Just Raised PT" flag (linked to that analyst's track record page).

## 5. Conversion Strategy

- **Above-the-fold CTA:** "Get pre-earnings brief for [next mega-cap reporting today]" — clicks into a Premium-gated deep-dive teaser.
- **Free vs. Premium boundary:** Free = calendar table, consensus EPS, Smart Score visible, confirmed/estimated status, basic filters. Premium = whisper numbers, top-analyst-weighted forecasts, hedge-fund positioning delta, insider activity in past 30 days, implied-move calibration history, alerts.
- **Upgrade hooks:** Row-level "🔒 See top analyst's forecast" badges (visible teaser, click reveals paywall with the specific analyst's name + accuracy score to sharpen the loss).
- **Trust elements:** "Analyst accuracy verified across 47,000+ ratings since 2010" strip; sample analyst track-record card in the sidebar; media logos.
- **Engagement modules:** Save-to-Watchlist per row (anonymous → registered), "Set earnings alert" (email capture), "Compare pre-earnings" multi-select tool.
- **Sticky mobile CTA:** "Notify me before [next report]" — one-tap alert setup drives registration.
- **Post-earnings return hook:** Once a stock reports, the row transforms into a "Reacted +/− X%; see updated Smart Score and analyst reactions" CTA — brings users back the next day.
- **Exit-intent module:** "Get every Monday's earnings brief in your inbox" newsletter capture (repeat-visit engine).

## 6. Editorial Guidance

- **Tone:** Data-forward, plain-English, zero hype. Every claim traceable to a data point on the page.
- **Depth:** Programmatic pages (light editorial per ticker) + one weekly human-written "Earnings Week Ahead" recap piece linked from the hub as an E-E-A-T anchor.
- **Freshness frequency:** Calendar table auto-refreshes intraday for confirmed-date changes; post-earnings reaction data updates within 15 min of report; weekly recap published every Sunday PM.
- **E-E-A-T signals:** Byline the weekly recap with a TipRanks markets analyst (photo, bio, LinkedIn); cite the analyst-accuracy dataset methodology page; timestamp "last updated" prominently.
- **Voice-and-tone don'ts:** No clickbait ("SHOCKING earnings incoming"); no unsourced "expected to beat" language — always attribute to consensus or a named analyst.
- **Localization:** Timezone auto-detect + explicit label ("2:00 PM PT / 5:00 PM ET"); currency labels on every EPS figure.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Massive evergreen + seasonal peaks 4×/year; captures ticker-level long-tail via `/earnings-calendar/[ticker]` children; competitors rank flat tables that TipRanks can 10x with proprietary signals. |
| Business upside | 5 | Pre-earnings intent is peak-value: users are about to make a trade. Highest-converting moment for Premium upsell in the entire TipRanks funnel. |
| UX complexity | 3 | Table + filters + drawers is well-trodden UX; complexity is in the multi-column filter state + mobile responsiveness of dense data rows. |
| Engineering complexity | 4 | Confirmed-date scraping/ingest pipeline, options-implied-move calc, whisper aggregation, and real-time post-earnings reactions require solid data-eng plumbing; schema and programmatic sub-pages add scope. |
| Recommended rollout speed | 4 | Ship v1 (free calendar + Smart Score + basic filters + schema) within 4 weeks to catch the tail of Q2 season and be ready for Q3 in October; layer Premium hooks and programmatic ticker pages in v2 through August. |
