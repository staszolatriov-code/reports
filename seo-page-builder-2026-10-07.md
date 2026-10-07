# SEO Page Builder — Earnings Calendar
**Date:** 2026-10-07
**Selected cluster:** `earnings calendar`
**Rationale for pick:** Q3 2026 earnings season opens this week (JPMorgan, Delta, Citi report Oct 10–14). Volume on "earnings calendar" and long-tails ("earnings this week", "earnings before market open today", "stocks reporting earnings tomorrow") triples from early-October through mid-November. Competitors publish static tables; TipRanks can ship an intelligence surface — the single highest-leverage SEO page we can build this quarter.

---

## 1. Page Thesis

The Earnings Calendar is TipRanks' flagship data hub for the single most predictable traffic spike of each quarter: earnings season. It's for active retail investors (and lurking pros) who want to know what's reporting today/this week, what the market expects, and — the differentiator — how analyst accuracy, Smart Score, insider trades, and hedge-fund positioning around a report shape the probability of an EPS beat and post-earnings drift. It deserves to rank because it fuses a canonical calendar table with pre- and post-earnings proprietary signals no competitor exposes above the fold. It converts because every row is an invitation into a stock page gated by a Smart Score preview, an "Earnings Beat Probability" paywall tease, and a one-click watchlist CTA that lands users in the registered-user funnel.

## 2. Search Intent Breakdown

- **Primary intent:** "What's reporting earnings this week / today / before open / after close?" — a scannable, filterable schedule with EPS/revenue consensus.
- **Secondary intent:** "Will this stock beat?" — users want pre-earnings edge: history of beats/misses, analyst accuracy on this ticker, options-implied move, insider/hedge-fund activity in the last 90 days.
- **What users really want:** A tradeable view — not a table, a *watchlist builder* with reasons to care about each row. "Which 3 of this week's 220 reports should I actually watch?"
- **What makes them bounce:** Walls of unsorted tickers, no logos, stale consensus numbers, no filtering by market cap/sector/time-of-day, mobile tables that side-scroll, and gating the calendar itself (gate the *insights*, never the dates).

## 3. 10x Page Blueprint

- **Page type:** Dynamic data hub (template, not article). Static shell + hydrated table + per-row drawer. SSR for crawlability; client hydration for filters/sorting.
- **Title tag:** `Earnings Calendar — This Week's Earnings Reports & EPS Estimates | TipRanks` (58 chars)
- **Meta description:** `Track every earnings release this week with analyst consensus, Smart Score, insider activity, and beat probability. Updated live before and after market close.` (158 chars)
- **H1:** `Earnings Calendar: Companies Reporting This Week`
- **H2/H3 outline:**
  - H2: This Week's Earnings at a Glance *(hero stats: # of S&P 500 reports, # of mega-caps, aggregate expected EPS growth YoY)*
  - H2: Earnings Calendar *(the main table — see modules)*
    - H3: Today's Earnings
    - H3: Tomorrow Before Market Open
    - H3: Tomorrow After Market Close
  - H2: Most-Watched Reports This Week *(top 10 by TipRanks follower count + options volume)*
  - H2: Pre-Earnings Movers *(stocks up/down > 5% in the 5 days before their report)*
  - H2: How to Use the Earnings Calendar *(three-step: Filter → Scan Smart Score → Add to Watchlist)*
  - H2: What Smart Score Tells You Before Earnings *(product explainer, 150 words, Smart Score backtested beat-rate chart)*
  - H2: Last Week's Beats & Misses *(evergreen traffic — reverse-chronological)*
  - H2: Earnings Calendar FAQ *(FAQ schema target)*
    - H3: When do companies report earnings?
    - H3: What is EPS and how is it estimated?
    - H3: How accurate are analyst estimates?
    - H3: What is a "whisper number"?
    - H3: How does TipRanks' Smart Score predict earnings beats?
- **Recommended modules:**
  1. **Date range tabs** — Today / Tomorrow / This Week / Next Week / Custom.
  2. **Filter rail** — sector, market cap, exchange, country, time of day (BMO/AMC/during), Smart Score band (8+/5–7/<5), analyst coverage count.
  3. **The table** — Logo · Ticker · Company · Report Date · Time · Period · EPS Est · EPS Prior · Rev Est · **Smart Score (free preview, numeric)** · **Analyst Consensus (Buy/Hold/Sell + avg price target % upside)** · **Insider Signal (90-day net $)** · **Beat Probability (gated — show %-locked tease)** · Add-to-Watchlist star.
  4. **Row drawer (expand without navigation)** — mini chart (90d), last 8 quarters of beat/miss bars, top 3 analysts by track-record accuracy on this ticker, hedge-fund 13F delta last quarter, options-implied earnings move.
  5. **Download CSV** — gated behind free account (lead capture).
- **Interactive components:** multi-select filter chips, saved-filter presets ("Mega-caps this week", "Dividend aristocrats reporting"), column sort, sticky header on scroll, keyboard navigation (j/k), per-row watchlist toggle, email-this-row (lead capture).
- **Visual/data components:**
  - Weekly heatmap strip (M–F) showing report-count density, color-ramped by aggregate market cap.
  - Sector sunburst of this week's reporters.
  - Smart Score distribution bar for this week's reporters vs. historical average.
  - Per-row sparkline (90d price) + beat/miss history bars (last 8 Q).
- **Schema opportunities:**
  - `WebPage` + `BreadcrumbList`.
  - `ItemList` → each entry `Event` with `name`, `startDate`, `location: VirtualLocation`, `organizer: Corporation`, `eventStatus`.
  - `FAQPage` for the FAQ H2.
  - `Dataset` for the calendar itself (strong signal for Google Dataset Search).
- **Internal linking strategy:**
  - Every ticker row → `/stocks/{ticker}` and `/stocks/{ticker}/earnings`.
  - Hub links to: Analyst Ratings, Smart Score, Insider Trading, Hedge Fund Activity, Options Activity, Dividend Calendar.
  - Breadcrumb: Home → Research Tools → Earnings Calendar.
  - Weekly recap posts link back to the hub with anchor to that week's section.
  - Reciprocal: every `/stocks/{ticker}/earnings` page links back to the hub when the ticker is reporting in the next 14 days (dynamic injection).

## 4. Differentiation vs. Competitors

| Competitor | What they do | Where they're weak | How TipRanks beats them | TipRanks data above the fold |
|---|---|---|---|---|
| **StockAnalysis.com** | Clean, fast table: ticker, date, time, EPS est, EPS prior. Minimal filters. | No forward-looking signal — it's a schedule, not a decision tool. No analyst track-record data. No insider/HF overlay. Weak mobile drawer. | Add Smart Score column + Beat Probability + 90-day insider net + analyst accuracy — all without losing their speed. | Smart Score chip + analyst consensus + 90d insider $ net on every row. |
| **Barchart.com** | Dense table with analyst estimate counts, surprise history, and a "flag" column. Pro-trader UX. | Overwhelming for retail; buries the "why should I care about this row?" Behind a hard paywall for most useful columns. Ad-heavy. | Retail-first layout, free Smart Score preview, insider + HF signals Barchart doesn't carry at all. Clean mobile. | Smart Score + "Top Analyst Rating" (name + track-record %) above the fold. |
| **MarketBeat.com** | SEO-heavy table with lots of ads, "upcoming earnings" with consensus. Decent long-tail coverage. | Thin per-row signal — mostly consensus EPS and a buy/hold/sell summary. No proprietary score. Interstitials and ad density hurt UX + Core Web Vitals. | Proprietary Smart Score, hedge-fund 13F delta, insider cluster-buy flags — none of which MarketBeat has. Faster LCP by removing ad stack from above the fold. | Smart Score + hedge-fund 90d net flow + insider cluster-buy badge. |

**TipRanks' unfair advantage above the fold:** a single composite row that fuses analyst accuracy (not just consensus), proprietary Smart Score, 90-day insider net, and hedge-fund delta — a package no competitor can replicate without licensing TipRanks data.

## 5. Conversion Strategy

- **CTA #1 (sticky, soft):** "Add to Watchlist" star on every row → free-account signup prompt on first click (not before — let them scan).
- **CTA #2 (above fold):** "Get Beat Probability for every stock reporting this week — free trial" — single primary button, no competing CTAs in the hero.
- **Free vs. premium boundary:** Free users see Smart Score number, analyst consensus, insider net $. Premium gates: Beat Probability %, full top-analyst accuracy table, options-implied move, CSV export of the full week.
- **Upgrade hooks:** Each gated cell shows a blurred value + "See probability — 7-day free trial"; drawer "Top analysts" shows 1 of 3 with the other 2 blurred and labeled with track-record % to prove value.
- **Trust elements:** Analyst-accuracy methodology link, "Backtested: Smart Score 9/10 stocks beat EPS 73% of the time (2019–2025)" stat bar, SEC-source-of-record badge on insider rows, logos of outlets citing TipRanks (press strip in footer only, never hero).
- **Engagement modules:** Save filter preset (requires free account), "Email me when a Smart Score 9/10 stock reports next week" (lead magnet), live countdown to next mega-cap report.
- **Post-earnings re-engagement:** Users who starred a stock receive an in-app and email digest within 60 min of its release with the beat/miss, Smart Score shift, and a one-tap "see analyst reactions" link.
- **Social proof in-row:** "N TipRanks users watching" badge on top 20 rows — real-time, drives both FOMO and watchlist click-through.

## 6. Editorial Guidance

- **Tone:** Decisive and data-forward. "Smart Score 9. 73% historical beat rate on 9s. Three top analysts (87% accuracy) bullish." Not "Analysts are watching this report with interest."
- **Depth:** The hub itself is thin on prose (data does the work). Earnings-preview articles for the top 10 reports/week — 400–600 words each, author-bylined, cite TipRanks data points with internal links back to the hub.
- **Freshness frequency:** Table hydrates on every page load (TTL 60s during market hours, 5 min off-hours). Consensus EPS refreshes on analyst-update events. "Last week's beats & misses" section auto-rotates Monday 9am ET. Hero stats recompute hourly.
- **E-E-A-T signals:** Byline every preview article; author pages with credentials, LinkedIn, prior coverage; methodology page for Smart Score linked from every row drawer; cite SEC filings on insider rows with direct links; data-provider attribution footer.
- **Author authority:** Rotate 3–5 named analysts across preview articles; interlink to their author pages; schema `Person` + `sameAs` to their social profiles.
- **Mobile-first copy:** Every H2 and every drawer label must read in <40 characters without wrapping on a 375px viewport.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Quarterly spike + evergreen table; competitors are all beatable on signal density; "Dataset" schema opens Google Dataset Search surface. |
| Business upside | 5 | Highest-intent audience of the quarter; Beat Probability is a credible premium gate; watchlist CTA has clear downstream LTV. |
| UX complexity | 4 | Filter rail + per-row drawer + mobile parity + accessible keyboard nav is non-trivial but a known pattern. |
| Engineering complexity | 4 | Data pipeline exists; new work is Beat Probability model productionization, 60s TTL cache, Dataset schema, drawer component, email-trigger service. |
| Recommended rollout speed | 5 | Ship v1 (table + Smart Score column + drawer) within 2 weeks to catch the Oct 10 kickoff; iterate Beat Probability gate and email digest in weeks 3–5. |

---

### Rollout sketch (not part of required deliverable, but worth noting)

- **Week 1:** Ship static shell, SSR table, Smart Score column, analyst consensus column, basic filters, `ItemList`+`Event`+`FAQPage` schema, `Dataset` schema. Catch the Oct 10 wave.
- **Week 2:** Row drawer, insider net $ column, hedge-fund delta, sector sunburst, mobile polish.
- **Weeks 3–5:** Beat Probability gating + 7-day trial flow, saved-filter presets, post-earnings email digest, 10 top preview articles/week with byline author pages.
- **Ongoing:** Weekly "Last Week's Beats & Misses" auto-generated recap; monthly refresh of methodology stat bar with latest backtest.
