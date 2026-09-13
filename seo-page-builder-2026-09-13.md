# SEO Page Builder — 2026-09-13

**Selected opportunity:** Hedge fund holdings
**Primary head term:** `hedge fund holdings` (+ tail: `top hedge fund stocks`, `13F filings tracker`, `what hedge funds are buying`, `<manager name> portfolio`, `<ticker> hedge fund ownership`)
**Why today:** Q2 13F filings deadline (Aug 14) is now fully digested and Q3 positioning chatter is dominating financial media through September; search demand for "what hedge funds are buying" spikes in the 4–6 weeks after each 13F deadline. This is also TipRanks' single strongest data moat vs. StockAnalysis, Barchart, and MarketBeat.

---

## 1. Page Thesis
A product-led hub — `/hedge-funds` — that turns raw 13F filings into a live, rankable, filterable intelligence layer: top managers by AUM and track record, most-bought and most-sold tickers this quarter, consensus positions, and per-manager portfolios with performance scoring. It's built for retail investors who want to mirror smart-money moves and for advisors who need a defensible "what the pros own" reference. It deserves to rank because no competitor combines manager-level track record accuracy with ticker-level consensus and Smart Score overlays. It converts because the highest-signal columns (manager track record %, portfolio alpha, next-quarter conviction) sit behind Premium.

## 2. Search Intent Breakdown
- **Primary intent:** transactional-informational — "show me what hedge funds are holding/buying right now" with sortable data.
- **Secondary intent:** navigational — users searching a specific manager (Buffett, Burry, Ackman, Griffin) or a specific ticker's institutional owners.
- **What users really want:** a shortcut to conviction — one screen that says *which managers are worth copying, what they bought last quarter, and which of those names still look good today.*
- **What makes them bounce:** stale filings with no "as of" date, walls of raw 13F text, no filtering, no accuracy scoring on the manager, and paywalls hit before the user has seen any value.

## 3. 10x Page Blueprint

- **Page type:** Data hub landing page with three tab-linked template children (`/hedge-funds`, `/hedge-funds/<manager-slug>`, `/stocks/<ticker>/hedge-fund-activity`).
- **Title tag:** `Hedge Fund Holdings & 13F Tracker — Top Managers & Stocks | TipRanks`
- **Meta description:** `Track hedge fund holdings from the latest 13F filings. See top managers by track record, most-bought stocks, and per-portfolio performance — updated after every SEC filing.`
- **H1:** `Hedge Fund Holdings & 13F Tracker`
- **H2/H3 outline:**
  - H2 What hedge funds are buying and selling this quarter
    - H3 Most-bought stocks (net new + adds)
    - H3 Most-sold stocks (exits + trims)
    - H3 Highest-conviction consensus picks
  - H2 Top hedge fund managers by track record
    - H3 Ranked by 1Y / 3Y / 5Y portfolio return
    - H3 Ranked by TipRanks manager Smart Score
  - H2 Explore individual hedge fund portfolios
  - H2 Hedge fund ownership of trending stocks
  - H2 How TipRanks scores hedge fund managers (methodology)
  - H2 Filing calendar & next 13F deadline
  - H2 FAQ (what is a 13F, filing lag, limitations, how often we update)
- **Recommended modules:**
  - Quarter selector (Q2 2026 default) + "as of" freshness badge
  - Manager leaderboard table with TipRanks track-record % and portfolio value
  - "Buys vs. sells" heatmap tile (aggregated across tracked funds)
  - Consensus ticker table (# funds holding, net share change, avg. cost basis where inferrable)
  - Watchlist-style "follow this manager" toggle
- **Interactive components:**
  - Multi-select filter: sector, market cap, manager AUM band, position size %
  - Sort on every column; sticky header on scroll
  - "Compare 2 managers" side-by-side portfolio drawer
  - Ticker hover-card showing Smart Score + analyst consensus + last insider trade (uses existing TipRanks widgets)
- **Visual/data components:**
  - Sankey of "sector rotation this quarter" across all tracked funds
  - Bar+line combo: aggregated hedge fund equity exposure vs. S&P 500 quarterly
  - Per-manager sparkline of portfolio value across the last 8 quarters
- **Schema opportunities:** `Dataset` schema for the holdings tables, `ItemList` for the top-managers leaderboard, `FAQPage` for the 13F FAQ, `BreadcrumbList` for the manager child pages, `Organization` for named fund entities.
- **Internal linking strategy:**
  - Hub links out to every `/hedge-funds/<manager>` child + every `/stocks/<ticker>/hedge-fund-activity` tab.
  - Every `/stocks/<ticker>` page cross-links its "Hedge Fund Activity" tab into this hub.
  - Insider Trades and Analyst Ratings hubs each get a "See what hedge funds think" module linking here.
  - Blog posts about smart-money trends embed the top-managers table as a canonical citation link.

## 4. Differentiation vs. Competitors

### StockAnalysis.com
- **What they do:** Institutional ownership by ticker (holders list, % held, quarterly change). Clean tables.
- **Where they're weak:** No manager-level entity pages, no track-record scoring, no cross-fund aggregation, no "what's being bought right now."
- **How TipRanks beats them:** Ships a manager entity layer with accuracy scoring and cross-fund aggregation — StockAnalysis is a ticker-first view; TipRanks is both ticker- and manager-first.
- **Above the fold on TipRanks:** manager leaderboard sorted by track record, plus the current-quarter "most bought" tile.

### Barchart.com
- **What they do:** 13F filings search and per-fund holdings snapshots, buried under a data-heavy nav.
- **Where they're weak:** No performance scoring per manager, hostile UX for retail, no consensus/aggregation view, gated on legacy paywall.
- **How TipRanks beats them:** Product-led surface — a retail investor gets a usable answer in under 10 seconds without knowing what a 13F is; Barchart makes you go find it.
- **Above the fold on TipRanks:** plain-English framing ("Here's what hedge funds bought last quarter") + one primary CTA.

### MarketBeat.com
- **What they do:** Institutional ownership pages and a "hedge fund tracker" list; heavy on ads, thin on data depth.
- **Where they're weak:** Little to no per-manager performance context, no cross-manager consensus, ad-clutter that suppresses trust and dwell time.
- **How TipRanks beats them:** Cleaner data density, proprietary manager Smart Score, and a track-record layer that MarketBeat can't reproduce without building its own accuracy corpus.
- **Above the fold on TipRanks:** manager Smart Score column and portfolio return-vs-S&P delta.

## 5. Conversion Strategy
- Free tier: latest quarter's aggregated buys/sells table + top-25 managers with track-record %.
- Premium wall: full manager list, downloadable holdings CSV, historical quarter-over-quarter deltas, and "follow this manager" alerts.
- Sticky right-rail CTA: "Get alerts when Buffett/Burry/Ackman files" — fires the paywall on click.
- Inline upgrade hook on every locked column with a one-line why ("Premium unlocks 5-year manager track record").
- Trust: methodology drawer explaining how manager track record is computed, sample size, and filing-lag disclosure.
- Social proof band: "Tracking 8,400+ 13F filers · Updated within 24h of SEC posting."
- Engagement: "Add manager to portfolio" and "Compare to my holdings" — both require a free account, seeding the funnel.
- Exit-intent: offer a free weekly "Smart Money Digest" email — top 3 buys and sells across tracked funds.

## 6. Editorial Guidance
- Tone: confident, plain-English, no jargon-first sentences ("A 13F filing is…" always comes before "13F filing").
- Depth: methodology page and per-manager bio pages carry the E-E-A-T load; the hub itself stays data-forward.
- Freshness: hub updated within 24h of each SEC filing; homepage "as of" badge is non-negotiable and drives freshness signals.
- Freshness cadence: quarterly deep-refresh (post 13F deadline: Feb 14 / May 15 / Aug 14 / Nov 14), weekly aggregate recomputation.
- E-E-A-T signals: named author on methodology page, links to SEC EDGAR source filings, timestamped data, TipRanks analyst team byline.
- Editorial companion pieces: quarterly recap articles ("What hedge funds bought in Q3 2026") that internal-link back to the hub as the canonical data source.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Head term + massive long-tail (per manager, per ticker × hedge-fund-activity); competitors are weak on entity coverage. |
| Business upside | 5 | Hedge-fund data is a top-quartile Premium conversion driver historically; retail investors pay to "copy smart money." |
| UX complexity | 3 | Filters, sortable tables, and manager drawers are patterns the site already uses; the Sankey/sector-rotation viz is the only new component. |
| Engineering complexity | 4 | 13F ingestion + normalization + accuracy scoring is real infra; if the pipeline exists, the surface is a wrapper; if not, this is a quarter of work. |
| Recommended rollout speed | 4 | Ship the hub + manager pages in a 4–6 week sprint against the next 13F deadline (Nov 14, 2026); ticker-tab expansion in a follow-up. |
