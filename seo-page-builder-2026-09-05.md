# SEO Page Builder — Earnings Calendar

**Date:** 2026-09-05
**Selected cluster:** `earnings calendar` (and its long tails: *earnings this week*, *earnings today*, *[TICKER] earnings date*, *earnings whisper*, *pre-market earnings*, *AMC earnings*)
**Why today:** Q3 2026 earnings season begins in ~5 weeks. Search volume for "earnings calendar" and ticker-specific "earnings date" queries starts climbing in the first two weeks of September and peaks the week banks report. Publishing/refreshing now captures the ramp instead of the peak.

---

## 1. Page Thesis

The **TipRanks Earnings Calendar** is a real-time, personalized command center for every investor tracking upcoming reports — not a static table. It ranks each event by *what actually moves the stock*: analyst revisions, hedge-fund positioning changes into the print, insider activity in the prior 30 days, and TipRanks Smart Score deltas. It deserves to rank because competitors offer flat lists; TipRanks layers proprietary signal on top of the schedule so users know *which* earnings to care about. It converts because the free page shows the "what and when," while Premium unlocks the "will it beat, and what will the reaction be" — a natural upgrade moment two days before every major print.

## 2. Search Intent Breakdown

- **Primary intent:** "Which companies report earnings this week, and when (BMO/AMC)?" — a scannable, filterable schedule with dates, times, EPS estimates, and previous surprise.
- **Secondary intent:** "Is [TICKER] worth trading into earnings?" — beat/miss history, expected move, analyst pre-print revisions, options-implied volatility.
- **What users really want:** A shortlist of the 5–15 reports that matter *to them* (their watchlist, sector, or market cap), with a confidence signal on the outcome.
- **What makes them bounce:** Stale data (yesterday's calendar), no time-of-day (BMO/AMC), missing consensus estimates, ads above the fold, or a paywall on the schedule itself.

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (interactive calendar + per-ticker deep pages beneath it). Hub-and-spoke: `/earnings-calendar` → `/earnings-calendar/[week|date]` → `/stocks/[ticker]/earnings`.
- **Title tag:** `Earnings Calendar 2026 — This Week's Reports, EPS Estimates & Smart Score | TipRanks` (58 chars, refresh dynamically to reflect the current week).
- **Meta description:** `See every earnings report this week with EPS estimates, BMO/AMC timing, analyst revisions, hedge fund positioning, and TipRanks Smart Score. Free & updated live.` (159 chars)
- **H1:** `Earnings Calendar — Week of Sept 8–12, 2026` (dynamic, week-aware).
- **H2/H3 outline:**
  - H2: This Week's Highest-Impact Earnings *(TipRanks Top 10, ranked by Smart Score + est. move)*
    - H3: Before the Bell | After the Close
  - H2: Full Earnings Calendar *(sortable table, filters below)*
  - H2: Earnings by Sector
  - H2: Biggest Expected Movers *(implied move %, from options)*
  - H2: How Analysts Have Revised Estimates in the Last 30 Days
  - H2: Hedge Fund & Insider Activity Ahead of Earnings
  - H2: How to Read an Earnings Report *(collapsed, evergreen educational block for E-E-A-T)*
  - H2: Earnings Calendar FAQ *(schema-marked)*
- **Recommended modules:**
  1. Sticky filter bar: date range, market cap, sector, index (S&P 500 / Nasdaq 100 / Russell 2000), watchlist toggle, Smart Score ≥ 8 toggle, BMO/AMC.
  2. "TipRanks Top 10 This Week" curated tile row above the fold.
  3. Per-row expandable drawer: EPS/revenue estimate, 4-quarter beat/miss streak, analyst consensus & 30-day revision delta, hedge-fund net activity last quarter, insider net buying/selling (90d), options-implied move %, Smart Score.
  4. "Notify me before [TICKER] reports" one-click watchlist add → account signup gate.
  5. Live "Reporting Today" ticker strip fixed to top during market hours.
- **Interactive components:**
  - Sortable/filterable virtualized table (10k+ rows without paginated page loads).
  - Toggle: "Only stocks I own / follow" (auth-gated → conversion moment).
  - Calendar-view / list-view toggle.
  - Weekly heatmap: number of S&P 500 reports per trading day.
- **Visual/data components:**
  - Sparkline of past-4-quarter EPS surprise per row.
  - Analyst revision arrows (▲ / ▼) with 30d delta.
  - Smart Score badge (1–10 gauge).
  - Expected move ± % chip pulled from options.
- **Schema opportunities:**
  - `Event` schema per earnings event (name, startDate, eventStatus, organizer).
  - `FAQPage` on the FAQ block.
  - `BreadcrumbList`.
  - `Dataset` for the calendar itself (rare among competitors — Google Dataset Search visibility).
  - `Organization` sitewide with `sameAs` to strengthen entity.
- **Internal linking strategy:**
  - Every ticker row links to `/stocks/[ticker]/earnings` (spoke page) and `/stocks/[ticker]/forecast`.
  - Sector rows link to `/sectors/[sector]/earnings`.
  - Cross-link from `/analyst-ratings`, `/hedge-funds`, `/insider-trading`, and every stock forecast page's "Next earnings: ___" module back to the calendar week page.
  - Footer hub links: Earnings This Week, Today, Next Week, After-Hours, Pre-Market, By Sector, By Index.

## 4. Differentiation vs. Competitors

### StockAnalysis.com
- **What they do:** Clean, fast, static-feeling weekly calendar with EPS estimate and prior actual. Minimal filtering.
- **Where they're weak:** No analyst revision context, no hedge fund/insider layer, no personalization, no expected-move data, no per-ticker deep drawer.
- **How TipRanks beats them:** Same clean UX + a full proprietary signal layer per row (Smart Score, revisions, HF activity, insider activity, implied move).
- **Above the fold:** TipRanks Top 10 tile with Smart Score badges — instant "which reports matter."

### Barchart.com
- **What they do:** Dense, powerful data table with implied move, IV rank, options data. Loved by traders.
- **Where they're weak:** UI is punishing for non-traders; ads-heavy; long-term fundamentals and analyst quality metrics are thin; hard paywall on advanced filters.
- **How TipRanks beats them:** Match their trader data (implied move, options context) *and* add analyst *track-record-weighted* consensus + hedge fund/insider layer — signal StockAnalysis and Barchart both lack. Free tier remains generous where Barchart gates.
- **Above the fold:** Implied move % chip + Smart Score, presented cleanly rather than in a data-dump grid.

### MarketBeat.com
- **What they do:** Broad earnings calendar with EPS consensus, previous quarter actual, "confirmed vs. estimated" date flag; strong email-newsletter funnel.
- **Where they're weak:** SEO-farm feel, thin per-ticker context, heavy interstitials and upsell CTAs disrupt the table, analyst quality is unweighted (all analysts treated equal).
- **How TipRanks beats them:** *Track-record accuracy scores* on every analyst estimate — MarketBeat cannot match this. Cleaner ad experience. Deeper drawer per row.
- **Above the fold:** "Analyst consensus (top-rated analysts only)" toggle — a differentiator MarketBeat literally cannot render.

## 5. Conversion Strategy

- Free tier: full calendar, EPS estimates, BMO/AMC, prior surprise, Smart Score badge, top-10 curated tile.
- Premium boundary: 30-day analyst revision history, hedge fund net activity trend, top-rated-analyst-only consensus, options-implied move, unlimited watchlist earnings alerts, downloadable weekly earnings preview PDF.
- CTA placement: (1) inline "Unlock revision history" chip inside the expanded row drawer — contextual, not banner-blindness-inducing; (2) sticky footer bar during market hours: "Get pre-earnings alerts for your watchlist"; (3) end-of-page "This week's Premium earnings preview" module.
- Upgrade hook: two trading days before each major print, email/push "Pre-Earnings Brief for [TICKER]" — free users see teaser, Premium sees the full brief. Drives the exact-timing upgrade moment.
- Trust elements above the fold: "Data updated 3 min ago" timestamp; "Coverage: 8,400 US tickers, updated live"; author/editor byline on the educational block; TipRanks accuracy-methodology link.
- Engagement modules: one-click "Add to my earnings watchlist" (soft signup — email only, no card); "Notify me at market open on report day" toggle.
- Social proof: "1.2M investors track earnings on TipRanks" counter (only if real).
- Retention loop: every watchlist add creates a scheduled email touch on report morning — brings the user back to the page.

## 6. Editorial Guidance

- **Tone:** Confident, analyst-grade, jargon-light. No hype. Assume the reader knows what EPS is but not what "revision breadth" means.
- **Depth:** Table-first, education-second. The static evergreen "How to read an earnings report" block sits below the fold and stays under 400 words — it is E-E-A-T fuel, not the product.
- **Freshness:** Calendar data live (sub-5-min lag). Weekly editorial refresh on top-10 curation and "biggest expected movers" every Sunday 6pm ET and Monday 7am ET. Timestamp visible.
- **E-E-A-T signals:** Named editor byline + credentials on the evergreen block; link to TipRanks' analyst accuracy methodology page; disclose data sources (analyst consensus, options pricing origins); reviewed-by date visible.
- **Voice consistency:** Third-person, active. Never "we think" — always "TipRanks data shows."
- **Accessibility:** All Smart Score gauges include text label; sparklines carry aria-labels; table sortable by keyboard.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High evergreen volume ("earnings calendar," "earnings this week") + massive long-tail on `[ticker] earnings date`; Q3 season is 5 weeks out. |
| Business upside | 5 | Pre-earnings is the highest-intent trading moment; direct funnel to Premium alerts and pre-earnings briefs. |
| UX complexity | 4 | Virtualized filterable table + row drawer + real-time updates + watchlist personalization is non-trivial. |
| Engineering complexity | 4 | Live data pipeline (estimates, revisions, options implied move, insider/HF joins), event schema, per-ticker spoke pages, alerting infra for watchlists. |
| Recommended rollout speed | 5 | Ship MVP (calendar + Smart Score + top-10 tile + Event schema) within 3 weeks to capture the Q3 earnings ramp; layer drawer + personalization + alerting in weeks 4–6. |

---

*Prepared 2026-09-05 · TipRanks SEO Page Builder*
