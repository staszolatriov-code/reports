# SEO Page Builder — 2026-08-03

**Selected cluster:** Hedge Fund Holdings
**Primary keyword:** `hedge fund holdings` (head), plus `13F filings tracker`, `top hedge fund stocks`, `[fund name] portfolio`, `hedge fund stock picks`, `what stocks are hedge funds buying`.
**Timing hook:** Q2 2026 13F filing deadline is **August 14, 2026** — search demand for hedge-fund holdings, top buys/sells, and manager-level portfolios peaks in the two-week window bracketing the deadline. Ship the hub + top ~50 manager pages before Aug 12.

---

## 1. Page Thesis
A programmatic **Hedge Fund Holdings hub** — one canonical `/hedge-funds` landing page fronting a directory of ~800 manager sub-pages (`/hedge-funds/[slug]`) — that turns the raw 13F firehose into a ranked, opinionated, decision-ready feed. The reader is a retail or semi-pro investor who wants to know *which managers have skill*, *what they just bought*, and *whether to copy the trade*. It deserves to rank because competitors publish stale holdings tables with no accuracy layer; TipRanks fuses 13F data with proprietary Manager Star Rating, consensus overlap with analyst ratings, and Smart Score on every position. It converts because the "should I buy this?" answer sits behind the Premium wall on every position row.

## 2. Search Intent Breakdown
- **Primary intent:** Investigative — "what are the top hedge funds holding / buying / selling right now?"
- **Secondary intent:** Navigational — "[Buffett / Burry / Ackman / Renaissance] portfolio" and "[TICKER] hedge fund ownership."
- **What users really want:** A ranked, filterable feed of *recent* moves by *skilled* managers, with a one-glance signal on whether the trade is worth mirroring.
- **What makes them bounce:** Stale data (last quarter's 13F with no filed-date stamp), walls of ticker tables without ranking, no manager track record, no "buy/sell delta" — the exact failure mode on the top 3 competitors today.

## 3. 10x Page Blueprint

**Page type:** Programmatic hub + directory (hub `/hedge-funds`, manager detail `/hedge-funds/[slug]`, stock cross-page module `/stocks/[ticker]/hedge-fund-activity`).

**Title tag (hub):** `Hedge Fund Holdings & 13F Tracker — Top Manager Portfolios | TipRanks`
**Meta description (hub):** `Track 800+ hedge fund portfolios, top buys and sells this quarter, and manager star ratings. See what Buffett, Burry, and Ackman just bought — updated within 4 hours of every 13F filing.`
**H1:** `Hedge Fund Holdings — Track What the Smart Money Is Buying`

**H2/H3 outline (hub):**
- H2: Top Hedge Fund Moves This Quarter
  - H3: Biggest Buys (last 30 days of filings)
  - H3: Biggest Sells
  - H3: Highest Conviction New Positions
- H2: Top-Rated Hedge Fund Managers
  - H3: By Manager Star Rating (1-yr, 3-yr, 5-yr)
  - H3: By AUM
  - H3: By Recent Alpha
- H2: What Are Hedge Funds Buying Right Now? (consensus buys)
- H2: Hedge Fund Consensus vs. Analyst Consensus (agreement/disagreement matrix)
- H2: 13F Filing Calendar — Next Deadline & Historical Windows
- H2: How to Use 13F Data (explainer + limitations: 45-day lag, longs only, no shorts, ETF exclusions)
- H2: FAQ (schema-marked)

**Recommended modules:**
1. **Live 13F Filing Ticker** (top of page) — chronological stream of filings from the last 72 hours; each row: filer, AUM, biggest new position, filed-at timestamp.
2. **Top Buys / Sells / New Positions leaderboard** (tabbed) — sort by dollar delta, share delta, or number-of-funds-piling-in.
3. **Manager Star Rating leaderboard** — TipRanks proprietary, tri-period (1/3/5 yr).
4. **Consensus Overlap heatmap** — stocks where hedge funds AND top-rated analysts AND Smart Score ≥ 8 all agree (this is the killer module — no competitor has it).
5. **13F Countdown widget** — days to next filing deadline; last-quarter recap.
6. **Stock-level "Hedge Fund Activity" card** (deployed on `/stocks/[ticker]`) — funds holding, quarter-over-quarter delta, top 5 holders, "smart money score."

**Interactive components:**
- Filter bar: quarter, manager type (activist / quant / long-short / macro), AUM band, Star Rating floor.
- "Compare two managers" side-by-side portfolio diff.
- "Notify me when [manager] files next quarter" — email capture (free-tier lead magnet).
- Follow list — save up to 5 managers free, unlimited on Premium.

**Visual/data components:**
- Sunburst chart: manager portfolio sector allocation.
- Sankey: quarter-over-quarter position flows (rotations in/out).
- Sparkline per manager: rolling alpha vs. S&P 500.
- Concentration meter: top-10 holdings as % of AUM.

**Schema opportunities:**
- `Dataset` schema on the hub (structured 13F dataset with `temporalCoverage`, `variableMeasured`).
- `FAQPage` on the explainer section.
- `BreadcrumbList` on manager detail pages.
- `ItemList` on leaderboards.
- `Organization` schema per manager page (populated with founder, AUM, HQ).
- `Article` schema only for the editorial "13F filing recap" companion posts.

**Internal linking strategy:**
- Hub → each top-50 manager page (rel prev/next chain via directory).
- Every manager page → each held ticker's `/stocks/[ticker]/hedge-fund-activity` module.
- Every `/stocks/[ticker]` page → its hedge-fund-activity module → back to top holders' manager pages.
- Cross-link to `/analyst-ratings/[ticker]` and `/smart-score/[ticker]` on every position row (this is what makes competitors' 13F pages orphaned).
- Editorial "top hedge fund stocks this quarter" recap → hub as canonical.

## 4. Differentiation vs. Competitors

**StockAnalysis.com** — Does: clean per-stock institutional ownership table, top-10 holders. Weak: no manager pages, no manager rating, no cross-quarter delta view, no "smart money consensus" layer, no filing-recency signal. **TipRanks beats them** by making managers first-class entities with track-record scores and by fusing 13F with analyst + Smart Score. **Above the fold:** Manager Star Rating leaderboard + Consensus Overlap heatmap.

**Barchart.com** — Does: raw 13F filings feed with searchable filings, per-fund holdings tables. Weak: unranked (all managers treated equal), no skill signal, sparse editorial context, dated UI, pushes to broker CTAs not to deeper product. **TipRanks beats them** with the Manager Star Rating as the ranking primitive, plus visual portfolio diffs and sector sunbursts instead of pure tables. **Above the fold:** Top Buys/Sells leaderboard weighted by manager rating (not just dollar size).

**MarketBeat.com** — Does: strong per-stock institutional ownership pages, "hedge fund tracker" tied to specific tickers, sturdy email capture flywheel. Weak: manager pages are thin, no proprietary scoring, low-differentiation content ("Institution X bought N shares" listicles), no consensus overlap. **TipRanks beats them** with the proprietary Smart Score + Manager Star Rating combo and by treating hedge fund data as an *analytics product*, not a news feed. **Above the fold:** Live 13F Filing Ticker + Consensus Overlap heatmap.

## 5. Conversion Strategy
- **Above-the-fold CTA:** "See what the top-rated hedge funds bought — Try Premium free for 7 days" attached to the Consensus Overlap heatmap (highest-intent module).
- **Free vs. Premium boundary:** Free = top 5 rows of any leaderboard, one manager watchlist slot, previous-quarter data. Premium = full leaderboards, unlimited watchlist, real-time filing alerts, portfolio diff export, cross-quarter deltas beyond 1 quarter.
- **Upgrade hook #1 — "Blurred row" pattern:** rows 6–20 visible but blurred with "Unlock full leaderboard" chip; industry-proven on comparable data products.
- **Upgrade hook #2 — Filing-alert email capture:** free email signup for next-13F alerts; drip sequence upgrades to Premium after 3 filings.
- **Trust elements:** Data-source footer ("Sourced from SEC EDGAR, updated within 4 hours of filing"), Manager Star Rating methodology link, last-updated timestamp on every table.
- **Engagement modules:** "Follow this manager" (email + in-app), "Compare to another manager," saved leaderboard filters.
- **Cross-sell:** Every position row links to `/stocks/[ticker]` — captures re-entry into the funnel via the stock page paywall.
- **Retention loop:** Post-signup, weekly digest email "Your followed managers filed: 3 new positions this week" — high open-rate hook that pulls users back for another paywall event.

## 6. Editorial Guidance
- **Tone:** Analytical, confident, non-hyped. Assume the reader knows what a 13F is; explain limitations plainly (no shorts, 45-day lag, longs only, ETFs excluded) — trust-building.
- **Depth:** Hub page = scannable data-first, ~1,200 rendered words including module labels. Manager pages = programmatic, sparse copy, dense data. Editorial recaps = 800–1,200 words with a clear POV.
- **Freshness cadence:** Data refresh within 4 hours of every SEC EDGAR filing. Hub leaderboards recompute nightly. Editorial "top hedge fund moves" recap published within 48 hours of the 13F deadline (Aug 14, Nov 14, Feb 14, May 15).
- **E-E-A-T signals:** Byline on editorial recaps with author bio + track record; methodology page for Manager Star Rating linked from every leaderboard; SEC EDGAR source attribution on every dataset; "reviewed by" tag from a named senior analyst.
- **Voice guardrails:** No "this stock is going to the moon" language on ANY hedge-fund page — the moat is being the *serious* source in a spammy vertical.
- **Cannibalization guard:** Editorial recaps must canonical to themselves but internally link the hub as the "live tracker" — do not duplicate the hub's leaderboard content in prose.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume head term with programmatic long-tail (800 manager pages × 4 quarterly freshness cycles). Competitor pages are weak and stale. |
| Business upside | 5 | Hedge-fund followers skew high-intent / high-LTV; multiple natural paywall points; strong recurring engagement loop via quarterly filings. |
| UX complexity | 4 | Requires 3 new templates, interactive leaderboards, cross-manager compare, and a paywall pattern that doesn't nuke SEO crawlability. |
| Engineering complexity | 4 | SEC EDGAR ingestion pipeline with 4-hour SLA, Manager Star Rating batch compute, cross-quarter deltas, and dataset schema at scale. Existing analyst-rating pipeline is a good scaffold. |
| Recommended rollout speed | 5 | **Ship hub + top 50 manager pages by Aug 12** (2 days before deadline) to capture the Aug 14 filing wave. Remaining 750 manager pages and stock-level module in the 30 days after. |

---

**Next actions (owner suggestions):**
1. SEO — lock URL structure `/hedge-funds` and `/hedge-funds/[slug]` this week; reserve slugs for top 50 managers.
2. Data eng — SLA the EDGAR ingestion at 4 hours; wire Manager Star Rating batch job.
3. Design — mock the Consensus Overlap heatmap and the blurred-row paywall pattern.
4. Editorial — draft the "Q2 2026 13F Recap" template so it can publish within 48 hours of Aug 14.
