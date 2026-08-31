# Competitor Watchdog — 2026-08-31

## MarketBeat.com

### 1. Summary of What Changed

- **ETF Screener** (`/ratingsdb/etf-screener/`) is live and filterable by asset class, benchmark, fund family, category, focus, region, and dividend yield — a full-featured landing page for ETF-related queries.
- **Dividend ETFs List** (`/dividends/etfs/`) ranks the 100 largest dividend ETFs by AUM — a high-intent page for income investors.
- **Dividend Screener** (`/dividends/screener/`) blends analyst rating rank (scored 0–4.00) with dividend yield/payout ratio — this is a product-SEO page combining two high-volume query clusters.
- **Earnings Calendar** (`/earnings/latest/`) continues indexing individual earnings call transcripts per company per quarter, creating a long-tail content moat.
- **Audio listening** for stock articles rolled out — UX/engagement signal, increases dwell time, reduces bounce.
- **All Access feature comparison page** (`/subscribe/all-access/#feature-comparison`) is being actively merchandised; premium positioning around analyst ratings and real-time alerts.
- Active syndication of dividend and ETF content to Yahoo Finance and Nasdaq.com, building external authority signals.

### 2. Why It Matters

MarketBeat is compounding a **product-led SEO moat**: every screener page is also a conversion funnel entry. Blending analyst ratings into dividend screener results is smart — it steals users searching for both analyst data AND income stocks. The earnings transcript strategy (per-ticker, per-quarter pages) builds enormous long-tail index coverage that compounds quarterly. Audio on articles boosts engagement signals that Google rewards.

### 3. Threat Level

| Finding | Threat Level |
|---|---|
| Dividend Screener with analyst rating ranking | **High** — directly competes with TipRanks' analyst-rated dividend pages |
| ETF Screener + Dividend ETFs list | **Medium** — growing ETF coverage TipRanks is lighter on |
| Earnings transcript long-tail content | **High** — high-volume, low-competition query cluster |
| Yahoo Finance / Nasdaq syndication | **Medium** — authority building from high-DA domains |
| Audio on articles (engagement UX) | **Low** — indirect SEO signal, but signals product investment |

### 4. Recommended Response

- **Build now**: A TipRanks dividend screener that surfaces analyst-rated dividend stocks — combining SmartScore with yield/payout data. MarketBeat's version is this combined product; TipRanks has the analyst data edge.
- **Build now**: Earnings transcript pages per ticker — even thin transcripts with structured data capture long-tail queries MarketBeat is vacuuming up.
- **Improve template**: ETF pages — ensure TipRanks ETF coverage (holdings, analyst exposure, ratings) is deeper than MarketBeat's screener output.
- **Strengthen internal linking**: Connect analyst ratings pages → dividend data → screener → conversion; MarketBeat's funnel architecture is tighter than it appears.

---

## StockAnalysis.com

### 1. Summary of What Changed

- **ETF Reverse Lookup Tool** (`/tools/etf-reverse-lookup/`) is a new standalone page: enter a ticker, see every ETF that holds it. Supported by a dedicated tutorial page for SEO/UX depth.
- **Fundamental Chart out of beta**, now globally available with two new indicator categories: *Forecasted* (S&P Global consensus estimates) and *Analyst Ratings* (3 years of daily price target + rating history). This is a direct attack on TipRanks' core value proposition.
- **Volume Alerts** extended to all logged-in users (previously gated) — registration conversion hook; reduces barrier to email capture.
- **Sharpe Ratio + Sortino Ratio** added across stock screener, ETF/mutual fund screeners, tables, and watchlist — targeting quant-oriented users and advisor-grade queries.
- **Top Analysts page** migrated to server-side pagination — faster TTFB, better Core Web Vitals.
- **Mobile app launched** on iOS App Store ("Stock Analysis: Stocks & Funds") — new acquisition channel outside organic search.
- 8.96M visits/month as of October 2025; growing.

### 2. Why It Matters

StockAnalysis adding **3 years of daily analyst rating history** into a free chart tool is a direct, product-level attack on TipRanks' paid differentiation. Users searching "analyst price target history [ticker]" may now land on StockAnalysis and get the data for free. The ETF Reverse Lookup fills a specific high-intent query ("which ETFs hold [stock]?") with a clean, free tool — TipRanks has weaker coverage here. Adding Sharpe/Sortino to screeners pulls in professional/advisor users who previously would have paid for Bloomberg or FactSet. The mobile app creates a new retention loop outside Google entirely.

### 3. Threat Level

| Finding | Threat Level |
|---|---|
| Analyst Ratings history in Fundamental Chart (free) | **Critical** — undermines TipRanks' core analyst data moat |
| ETF Reverse Lookup Tool (new page/query cluster) | **High** — captures a query type TipRanks doesn't own |
| Sharpe/Sortino in screener (quant metrics) | **Medium** — pulls professional user segment |
| Volume alerts gated removal (conversion hook) | **Medium** — email capture at scale, weakens TipRanks free-tier differentiation |
| Mobile app launch | **Medium** — long-term retention threat outside SEO channel |

### 4. Recommended Response

- **Respond immediately**: Audit TipRanks' analyst rating history depth vs. StockAnalysis Fundamental Chart. If TipRanks' free tier shows less data, this is a conversion threat. Consider making 1-year analyst rating history free with a clear upgrade prompt for 3+ years.
- **Build new page**: ETF Reverse Lookup equivalent — "ETFs holding [TICKER]" page template. TipRanks' analyst coverage of ETF constituents makes this page richer than StockAnalysis's version.
- **Add product modules**: Quant/risk metrics (Sharpe, Sortino, Beta, volatility) to stock pages and screener — the sophistication gap is closing fast.
- **Improve conversion hooks**: If volume alerts are now free on StockAnalysis, TipRanks' alert system should have a clear free tier with a visible upgrade path visible on first visit.
- **Monitor**: Mobile app growth — watch for mobile-specific ranking signals and consider TipRanks app retention improvements.

---

## Cross-Competitor Signals

Both MarketBeat and StockAnalysis are converging on the same strategy: **making analyst data infrastructure free at the surface, and monetizing depth**. MarketBeat blends analyst ratings into screeners. StockAnalysis puts 3-year analyst history into charts. This compresses the space TipRanks traditionally owns — premium analyst intelligence — into the free tier of commoditized tools.

Both are also expanding ETF coverage aggressively (screeners, lists, reverse lookups, dividend ETFs), signaling that ETF-related queries are a high-growth content vector neither has fully won.

**Strategic implication for TipRanks**: The moat is no longer just having analyst data — it's the quality, exclusivity, and actionability of that data (Smart Score, consensus models, hedge fund data, insider tracking). These need to be the first thing a user sees on any page, not buried in a premium paywall. Surface differentiation; let depth drive upgrades.

---

## Priority Action List

1. **[CRITICAL — This Week]** Audit analyst price target history depth on TipRanks free tier vs. StockAnalysis Fundamental Chart. Define a free/paid split that retains the moat without giving away the store.

2. **[HIGH — This Week]** Brief the product/content team on building an **"ETFs holding [TICKER]"** page template. This query cluster is unowned by TipRanks and being captured by StockAnalysis. TipRanks analyst coverage of holdings makes this a natural, differentiated fit.

3. **[HIGH — This Week]** Launch or prioritize a **combined Dividend + Analyst Rating Screener** page. MarketBeat already has this. TipRanks has better analyst data; this is a winnable page.

4. **[MEDIUM — Next Sprint]** Begin publishing **per-ticker earnings call transcript** pages. MarketBeat is indexing these at scale, building long-tail moat. TipRanks' earnings data is strong; wrapping it in indexable content captures adjacent queries.

5. **[MEDIUM — Next Sprint]** Add **Sharpe Ratio, Sortino Ratio, and Beta** as screener filters. StockAnalysis is pulling professional/advisor users with quant metrics. This segment converts to paid plans at higher rates.
