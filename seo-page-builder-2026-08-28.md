# SEO Page Builder — 2026-08-28

**Opportunity selected:** `hedge fund holdings`
**Rationale for today:** Q2 2026 13F filings were due Aug 14; the search cluster is at its seasonal peak (institutional-holdings queries spike for ~4 weeks after each 13F deadline). This is the annual window where TipRanks' hedge-fund data has the strongest topical relevance signal for Google and the strongest user demand — perfect timing to publish or refresh the hub.

---

## 1. Page Thesis

A product-led hub page at `tipranks.com/hedge-funds` that positions TipRanks as the single most useful destination for tracking what smart money owns, when they moved, and whether their track record is worth copying. Target audience: retail investors and prosumers who read WhaleWisdom / MarketBeat 13F trackers but want ranked, scored, and cross-referenced institutional data instead of raw filings dumps. The page deserves to rank because it converts a static filing archive into a decision-ready leaderboard (top funds by return, most-bought stocks this quarter, biggest new positions, consensus overlap with analyst upgrades). It converts because every fund/stock row is a gateway into TipRanks' fund pages, Smart Score, and premium alerts for "notify me when this hedge fund moves."

## 2. Search Intent Breakdown

- **Primary intent:** "Show me what hedge funds are buying/selling right now so I can copy or fade them."
- **Secondary intent:** Look up a specific manager (Buffett, Burry, Ackman, Pelosi-adjacent funds) or a specific stock's institutional ownership.
- **What they really want:** A ranked, filterable list with (a) fund track record, (b) recency of the move, (c) confidence it isn't stale from the 45-day 13F lag, and (d) a "what do I do with this" signal.
- **What makes them bounce:** Walls of raw 13F PDFs, tables without sort/filter, no fund performance context, requiring a login before showing any data, or a page that is just an SEO wrapper around a link to a Bloomberg-style paywall.

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (evergreen, refreshed nightly + on each 13F cycle) with programmatic sub-pages for each fund and each holding.
- **Title tag:** `Hedge Fund Holdings & 13F Tracker — Top Funds, Latest Trades | TipRanks` (58 chars)
- **Meta description:** `Track what hedge funds are buying and selling. Ranked by Smart Score and fund track record. See top managers, new positions, and consensus overlap with analyst ratings. Updated with the latest 13F filings.` (203 chars — trim to ~155 in prod)
- **H1:** `Hedge Fund Holdings — Track What Smart Money Owns`
- **H2/H3 outline:**
  - H2: Top Hedge Funds by Track Record (last 4 quarters, TTM, 3Y)
    - H3: Best-performing funds you can actually copy
  - H2: This Quarter's Biggest Moves
    - H3: Most-bought stocks by hedge funds
    - H3: Most-sold stocks by hedge funds
    - H3: New positions initiated
    - H3: Positions fully closed
  - H2: Hedge Fund Consensus vs. Analyst Consensus (crossover module)
  - H3: Where funds and analysts agree — high-conviction longs
  - H3: Where funds are ahead of analysts — contrarian bets
  - H2: Follow a Fund — Manager Profiles (Buffett, Ackman, Burry, Icahn, Loeb, Marks, …)
  - H2: Latest 13F Filings (real-time feed)
  - H2: How to Read a 13F (short primer, collapsible)
  - H2: Methodology & Data Freshness
- **Recommended modules:**
  - "Smart Money Movers this week" hero band (3 cards: top buy, top sell, top new position)
  - Sortable/filterable fund leaderboard (return, AUM, turnover, sector concentration)
  - "Most-owned by top-decile funds" table with Smart Score column
  - Filing recency badge on every row (e.g. `Filed 6 days ago`, `Stale — pre-quarter`)
  - Personalized "Funds that own stocks you own" (logged-in state)
- **Interactive components:**
  - Filter chips: quarter, sector, market cap, position size %, fund track record decile
  - "Copy this portfolio" side-by-side comparison against user's holdings
  - Sparkline of each fund's TTM alpha vs. S&P 500
  - Alert bell: "Notify me when [fund] files a new 13F or changes >5% in [ticker]"
- **Visual/data components:**
  - Heatmap of sector rotation across top 50 funds QoQ
  - Sankey of flows: sold-from → bought-into (across the top-50 fund cohort)
  - Bar chart: consensus-buy stocks with count of top-decile funds owning
  - Small-multiples of each top manager's top 5 positions
- **Schema opportunities:**
  - `Dataset` schema on the aggregate table (freshness, license, spatial coverage: US)
  - `FinancialProduct` on each linked stock
  - `FAQPage` on the primer section
  - `BreadcrumbList` (Home > Experts > Hedge Funds)
  - `ItemList` on each ranking module
- **Internal linking strategy:**
  - Every ticker row deep-links to `/stocks/{ticker}` with `#hedge-fund-activity` anchor
  - Every manager row links to `/hedge-funds/{slug}` programmatic pages (huge long-tail farm)
  - Cross-link to `/analyst-ratings`, `/insider-trading`, `/smart-score` — reinforce the "four expert crowds" story
  - Contextual link from `/stocks/{ticker}` "Institutional Ownership" widget back to this hub
  - Footer link cluster: `hedge fund tracker`, `13F filings`, `Warren Buffett portfolio`, `Michael Burry portfolio`, etc. — one anchor per programmatic child

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean institutional-ownership tables per stock; minimal fund-level pages.
- *Where they're weak:* No fund track record, no cross-signal with analysts/insiders, no alerting, no "what do I do with this."
- *How TipRanks beats them:* Rank funds by realized alpha, not AUM; overlay analyst consensus and insider activity on every row; add alerting.
- *Above the fold:* Smart Money Movers band + top-decile-fund leaderboard with realized-return column that StockAnalysis simply doesn't compute.

**Barchart.com**
- *What they do:* 13F data behind heavy paywalls; utilitarian, screener-first UX.
- *Where they're weak:* Poor storytelling, no manager profiles at scale, dated visual design, hostile to logged-out users.
- *How TipRanks beats them:* Free above-the-fold rankings with Smart Score; premium gates only the alerts and full history; visually modern and mobile-first.
- *Above the fold:* Free sortable leaderboard (Barchart hides this); one-click drill into a manager profile.

**MarketBeat.com**
- *What they do:* Individual "insider & institutional ownership" pages per ticker; heavy ad load; solid SEO but shallow analytics.
- *Where they're weak:* Fund pages are thin, no aggregate leaderboard, no track record scoring, ad-heavy UX kills engagement.
- *How TipRanks beats them:* Consolidated hub + deep fund pages + Smart Score + track record; cleaner UX = better dwell time = better SERP performance over time.
- *Above the fold:* Consensus overlap module (hedge funds + analysts + insiders agreeing) — a unique three-signal view MarketBeat cannot assemble.

## 5. Conversion Strategy

- Above-the-fold CTA is data, not a signup — earn trust by showing the leaderboard for free.
- Sticky right-rail CTA: "Get alerted when your favorite fund files" — collects email for free tier, gates real-time alerts to Premium.
- Free vs. Premium boundary: current quarter data free; historical 4-quarter comparison and consensus-overlap filtering behind Premium; alerting behind Premium+.
- Row-level upgrade hooks: "See this fund's full 47-position portfolio → Premium" after showing top 10.
- "Copy this portfolio to your watchlist" is free (creates account); "auto-mirror rebalances" is Premium.
- Trust elements: filing-freshness badge, source link to SEC EDGAR, methodology accordion, TipRanks accuracy score for each fund displayed inline.
- Engagement modules: comments on each fund profile, "followed by N TipRanks users" social proof, weekly digest opt-in ("This week in Smart Money").
- Exit-intent modal only on the primer section, offering a free "How the pros use 13Fs" PDF in exchange for email.

## 6. Editorial Guidance

- Tone: confident, data-forward, no hype; treat the reader as a serious retail investor, not a beginner.
- Depth: enough context that a first-time visitor can act; primer content lives in collapsibles so it doesn't dilute the SERP snippet.
- Freshness cadence: nightly recompute of aggregates; hard refresh within 24h of each 13F filing; a visible "Last updated" timestamp is mandatory.
- Quarterly editorial pass: rewrite the intro paragraph and top-movers copy after each 13F deadline (Feb 14, May 15, Aug 14, Nov 14) — this is the moment SERPs re-crawl heavily.
- E-E-A-T signals: byline from a named TipRanks analyst with credentials, link to methodology, cite SEC EDGAR as primary source, show TipRanks' own accuracy track record on hedge-fund predictions.
- Never fabricate manager quotes or intent; write about what the filings show, not why the manager did it, unless the manager publicly commented.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume evergreen cluster + strong programmatic long-tail (one page per fund, per manager, per quarter). Seasonal spikes 4×/year align with 13F cycle. |
| Business upside | 5 | Hedge-fund data is a top-3 reason paid users cite for Premium; alerting is a natural upsell with clear willingness-to-pay. |
| UX complexity | 4 | Sortable tables, cross-signal overlays, and consensus modules require careful information hierarchy to avoid overwhelming users. |
| Engineering complexity | 4 | 13F parsing is solved; the lift is the ranking/alpha computation layer, alerting infra, and the programmatic manager-page generator. |
| Recommended rollout speed | 4 | Ship the hub + top-50 manager pages within one 13F cycle (≤6 weeks) to catch the Nov 14 filing window; layer alerts and consensus module in phase 2. |

---

*Report generated 2026-08-28. Next rotation candidate: `price target tracker` (aligns with Q3 earnings-preview season starting mid-September).*
