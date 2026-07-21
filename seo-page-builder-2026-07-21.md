# SEO Page Builder — 2026-07-21

**Selected cluster:** ETF comparison
**Rotation rationale:** Recent reports covered analyst ratings and competitor intelligence (StockAnalysis.com). ETF comparison is the highest-conversion product-led surface TipRanks has not yet stress-tested against Barchart/StockAnalysis head-to-head templates, and mid-year 2026 flows into thematic and dividend ETFs make comparison queries structurally rising.

---

## 1. Page Thesis

A dynamic, two-and-three-way ETF comparison template (`/etf/compare/[TICKER-A]-vs-[TICKER-B]`) that renders side-by-side scoring, holdings overlap, expense-vs-return efficiency, and TipRanks Smart Score for ETFs — for every meaningful ETF permutation retail investors actually search. It targets the mid-funnel decision-maker who has narrowed to 2–3 tickers (SCHD vs VYM, QQQ vs QQQM, VOO vs VTI, JEPI vs JEPQ, IBIT vs FBTC) and needs one page to commit. It deserves to rank because programmatic comparison URLs are underserved by Barchart's bare tables and MarketBeat's thin content, and it converts because the "which one is better right now" answer requires TipRanks' analyst consensus on underlying holdings — a moat competitors cannot replicate.

## 2. Search Intent Breakdown

- **Primary intent:** Transactional decision — "should I buy A or B?" User has a brokerage tab open.
- **Secondary intent:** Portfolio construction — overlap, correlation, tax efficiency, income vs growth tradeoff.
- **What users really want:** A recommendation with defensible reasoning, not a spec sheet. They want the page to pick a winner for a stated goal (income, growth, low-cost core, downside protection).
- **What makes them bounce:** Wall of numbers with no synthesis; static data (stale expense ratios, missing YTD); requiring signup to see holdings overlap; no mobile-friendly side-by-side.

## 3. 10x Page Blueprint

- **Page type:** Programmatic comparison template, one URL per unique unordered pair (canonical: alphabetical). Extend to 3-way `/etf/compare/[A]-vs-[B]-vs-[C]` for top 500 triads.
- **Title tag:** `{A} vs {B} ETF Comparison ({YEAR}) — Holdings, Returns & Smart Score | TipRanks` (60 chars target with 5-char tickers)
- **Meta description:** `Compare {A} and {B} side by side: holdings overlap, 1/3/5-yr returns, expense ratio, dividend yield, analyst consensus on top holdings, and TipRanks Smart Score. Updated {DATE}.`
- **H1:** `{A} vs {B}: Which ETF Is the Better Buy Right Now?`
- **H2/H3 outline:**
  - H2: The 30-Second Verdict *(auto-generated recommendation with confidence tag)*
  - H2: Side-by-Side Overview *(key metrics table)*
  - H2: Holdings Overlap
    - H3: Shared Positions & Weight Difference
    - H3: Unique-to-A / Unique-to-B
  - H2: Analyst Consensus on the Underlying Basket *(weighted analyst score of holdings)*
  - H2: Smart Score Comparison
  - H2: Performance & Risk *(1M/YTD/1Y/3Y/5Y, max drawdown, Sharpe, beta)*
  - H2: Income Profile *(yield, growth streak, payout schedule, tax character)*
  - H2: Cost & Tax Efficiency
  - H2: Hedge Fund & Insider Activity in Top Holdings
  - H2: Which One Fits Your Goal? *(4 personas: Income, Growth, Core, Defensive)*
  - H2: Alternatives to Consider *(links to other comparison pages)*
  - H2: FAQ
- **Recommended modules:**
  - Verdict card (with "changed since last visit" indicator)
  - Overlap Venn/donut with hover-to-inspect
  - Weighted-analyst-consensus module (unique to TipRanks)
  - Smart Score radar chart (Analyst Signals, Hedge Fund, Insider, Blogger, News Sentiment, Fundamentals for holdings)
  - Persona selector that re-weights the verdict
  - "Add a third ETF" pivot to 3-way page
  - Live price + intraday spark
  - Portfolio-fit widget: "How would adding {A} vs {B} change my portfolio?" (logged-in state)
- **Interactive components:**
  - Toggle: total return vs price return; net vs gross of fees
  - Time-range slider driving performance and drawdown charts
  - Holdings filter (sector, market cap, region) with re-computed overlap
  - Currency selector (USD/EUR/GBP/CAD) — expands international traffic
- **Visual/data components:** overlap Venn, sector-allocation stacked bar, returns line, drawdown mountain, dividend-growth bar, expense-ratio dollar-cost-over-10-years horizontal bar.
- **Schema opportunities:**
  - `FinancialProduct` for each ETF
  - `ComparisonPage` (using `WebPage` + `ItemList` of `FinancialProduct`)
  - `FAQPage` for the FAQ block
  - `Table` markup for spec table
  - `Review` / `AggregateRating` mapped to Smart Score (with clear methodology disclosure)
- **Internal linking strategy:**
  - Every ETF profile page links to its top 5 comparisons (based on search volume + user co-view data)
  - "Alternatives" module links to 4–6 adjacent comparisons and one 3-way pivot
  - Hub page `/etf/compare` clusters by theme (Dividend ETFs, Bitcoin ETFs, S&P 500 ETFs, Semiconductor ETFs, Covered Call ETFs)
  - Cross-link into individual holding stock pages, dividend calendar, and Smart Score explainer
  - Author cluster: link to "How TipRanks scores ETFs" methodology page (E-E-A-T)

## 4. Differentiation vs. Competitors

**StockAnalysis.com** — Clean side-by-side spec tables, strong on fundamentals. **Weak:** static, no proprietary scoring, no view into underlying-holding sentiment, weak on income/tax nuance, thin verdict. **TipRanks beats them:** verdict card driven by analyst consensus on the actual underlying basket, plus dynamic re-ranking by persona. **Above the fold:** verdict + Smart Score delta + weighted-analyst-consensus badge.

**Barchart.com** — Raw data density and technicals. **Weak:** UX is dated, comparison is bolted onto quote pages, no synthesis, monetizes via paywall on the useful views, no natural language. **TipRanks beats them:** narrative verdict + interactive persona selector + holdings overlap visualization that isn't behind a login. **Above the fold:** the same, plus a "why this changed this week" freshness cue.

**MarketBeat.com** — SEO-heavy, article-style comparisons ("SCHD vs VYM: Which Is Better?"). **Weak:** written content that goes stale, no live data widgets, thin visuals, aggressive ad density hurts UX. **TipRanks beats them:** template that stays fresh automatically, live data, and proprietary Smart Score. **Above the fold:** verdict + last-updated timestamp + Smart Score, all before the first ad slot they would show.

**TipRanks' unique above-the-fold stack:** (1) One-line verdict with confidence, (2) Smart Score gap with directional arrow, (3) weighted analyst consensus on the underlying basket (no competitor computes this), (4) hedge-fund-flow signal into top holdings over the last quarter.

## 5. Conversion Strategy

- Primary CTA above the fold: "See both ETFs in your Portfolio" (free, requires signup) — highest-intent moment on the page.
- Secondary CTA in the verdict card: "Get alerts when the verdict changes" — email capture with low friction.
- Free vs premium boundary: overview, verdict, Smart Score, top-10 holdings overlap, and 1Y performance are free; full holdings overlap, weighted-analyst-consensus detail, hedge-fund flow beyond top 5, and historical Smart Score are Premium (Plus/Ultimate tier).
- Upgrade hook: blurred "Weighted Analyst Consensus — Full Basket" module with a specific dollar-savings framing ("Analysts price the {A} basket 8.2% above current NAV").
- Trust elements: methodology link on every proprietary number, "last updated" timestamp, analyst-count and hedge-fund-count sourcing, cite S&P/CFRA data provenance.
- Engagement module: persona selector re-computes verdict — moves session depth and returns users to the page.
- Comparison-history strip for logged-in users ("You compared VOO vs VTI 3 days ago — verdict is unchanged") to drive returns and personalization.
- Exit-intent: "Save this comparison" to a watchlist rather than a heavy modal — non-blocking, higher acceptance.

## 6. Editorial Guidance

- Tone: decisive and analyst-grade. First sentence of the verdict must pick a side or explicitly say "tie for [goal]." No hedging in the summary.
- Depth: synthesis over spec dumping. Every metric shown must resolve into a "so what" caption underneath.
- Freshness: verdict re-computed daily at market close; performance intraday; holdings weekly; hedge-fund positioning quarterly (with days-since indicator).
- E-E-A-T: byline the ETF research team, link to methodology, show reviewer credentials, disclose data providers, disclose that TipRanks does not offer personalized advice.
- Consistent glossary tooltips (Smart Score, Weighted Analyst Consensus, Sharpe, drawdown) — lowers bounce for beginners without cluttering the page for pros.
- Explicitly cover the top 3 objections in the FAQ per pair (tax treatment, tracking error, liquidity) — steals featured snippets from MarketBeat's article pages.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Programmatic wins across thousands of "X vs Y ETF" queries; template pattern compounds; steals from MarketBeat article pages and Barchart quote-adjacent comparisons. |
| Business upside | 5 | Mid-funnel intent → premium upsell is natural via full weighted-analyst-consensus and hedge-fund flow paywall. |
| UX complexity | 4 | Persona selector, interactive overlap, and dynamic verdict need careful IA; performance budget matters on mobile. |
| Engineering complexity | 4 | Ranking service for verdict, holdings-diff service, canonicalization of pair URLs, 3-way pivots, schema, and data-freshness pipeline. Reuses existing ETF and analyst infrastructure. |
| Recommended rollout speed | 4 | Ship v1 (verdict, overview, holdings overlap, Smart Score, performance) for top 500 pairs in 6–8 weeks; layer persona selector and 3-way in v2. |
