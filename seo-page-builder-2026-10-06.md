# SEO Page Builder — 2026-10-06

**Cluster selected today:** `earnings calendar`
**Why today:** Q3 2026 earnings season kicks off this week (big banks report Fri–Mon). Earnings calendar queries spike +40–70% in the five trading days before season opens, and the SERP is currently dominated by thin, non-interactive calendars. Prime window to ship or re-rank a 10x page before volume peaks.

---

## 1. Page Thesis

A product-led, real-time **Earnings Calendar** that is not a static table but a signal-rich workspace: every ticker row is instrumented with TipRanks' Smart Score, analyst consensus, EPS surprise history, hedge-fund 13F deltas, insider trades in the 30 days pre-report, and expected-move pricing. Target users are self-directed retail traders and premium-curious power users scouting earnings plays this week. It deserves to rank because no competitor combines a filterable calendar with proprietary conviction signals. It converts because every ticker row is a dozen micro-upgrade moments to Premium (full history, pre-earnings AI brief, portfolio alerts).

## 2. Search Intent Breakdown

- **Primary intent:** Transactional/navigational — "which companies report earnings this week/today and what should I watch?"
- **Secondary intent:** Research — EPS/revenue estimates, expected move, time of day (BMO/AMC), confirmed-vs-estimated date.
- **What users really want:** A ranked, filterable list that tells them *which* earnings matter and *why*, not an undifferentiated 400-row dump.
- **What makes them bounce:** Date-only tables with no estimates, pop-up email gates, slow-loading SPAs, no filtering by market cap or sector, mobile tables that overflow.

## 3. 10x Page Blueprint

- **Page type:** Interactive data hub (calendar + dynamic table) with sub-templates for weekly/daily/per-ticker.
- **Title tag:** `Earnings Calendar — This Week's Reports, EPS Estimates & Smart Score | TipRanks`
- **Meta description:** `Live earnings calendar with EPS estimates, analyst consensus, Smart Score, insider trades, and hedge fund activity before every report. Filter by date, sector, or market cap.`
- **H1:** `Earnings Calendar: Who's Reporting This Week`
- **H2/H3 outline:**
  - H2: Today's Earnings (BMO / AMC split)
  - H2: This Week at a Glance (heatmap by day)
  - H2: Confirmed vs. Estimated Dates — How to Read the Calendar
  - H3: Pre-Earnings Signals That Matter
  - H2: Top 10 Watched Earnings This Week (Smart Score + volume filter)
  - H2: Earnings Season Spotlight — Sector Previews
  - H2: FAQ (confirmed dates, after-hours moves, EPS vs. revenue)
- **Recommended modules:**
  1. Date picker + segmented control (Today / This Week / Next Week / Custom)
  2. Multi-filter bar: sector, market cap, Smart Score band, has-options, country
  3. Row-level inline expand: 5-quarter EPS surprise bars, revenue trend, analyst consensus pill
  4. "Pre-Earnings Watchlist" one-click add (free-tier hook)
  5. Expected move module (powered by options IV; Premium hook)
  6. Hedge fund + insider delta column (14-day lookback)
  7. AI Pre-Earnings Brief button per ticker (gated / limited free previews)
- **Interactive components:** Sticky column headers, column sort, saved filter presets, CSV export (Premium), one-click add-to-portfolio, dark-mode toggle, timezone selector.
- **Visual/data components:** Mini EPS-surprise sparkline per row, Smart Score colored pill (red→green 1–10), confidence badge, market-move expected-range bar.
- **Schema opportunities:** `ItemList` for the calendar table, `FinancialProduct` per ticker row, `FAQPage`, `BreadcrumbList`, `Event` schema for each earnings release (date, time, participant = Organization/ticker).
- **Internal linking strategy:**
  - Each ticker row → `/stocks/<ticker>/earnings`
  - Sector preview blocks → sector hub pages
  - "Smart Score explained" inline tooltip → Smart Score methodology page
  - Analyst column → analyst ratings page for that ticker
  - "Hedge fund delta" → hedge fund activity page
  - Breadcrumb: Home → Tools → Earnings Calendar
  - Footer: Earnings Whispers glossary, Price Target Tracker, Insider Trades hub (cross-cluster equity flow)

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast weekly earnings table with EPS/revenue estimates and surprise.
- *Weakness:* No conviction layer, no analyst/insider overlay, no AI brief, limited filters, no portfolio integration.
- *How TipRanks beats them:* Add Smart Score + consensus + insider/HF delta columns above the fold; keep load speed parity.
- *Above the fold on TipRanks:* Smart Score pill, analyst consensus, pre-earnings insider trade count.

**Barchart.com**
- *What they do:* Dense, feature-rich calendar with options data; strong for pros.
- *Weakness:* Information overload, dated UI, aggressive paywalls, poor mobile, no proprietary conviction score.
- *How TipRanks beats them:* Cleaner IA, mobile-first row expansion, proprietary Smart Score replaces the "which do I actually watch?" guesswork.
- *Above the fold:* Expected-move range bar beside each ticker (matches Barchart's options strength but visualized).

**MarketBeat.com**
- *What they do:* Earnings calendar + heavy email-capture, consensus beat/miss history.
- *Weakness:* SEO-stuffed boilerplate, interstitial email gates, no interactive filtering, little proprietary data.
- *How TipRanks beats them:* No interstitials, deeper proprietary signals (Smart Score, hedge fund, bloggers), AI pre-earnings brief.
- *Above the fold:* 5-quarter EPS surprise sparkline (visual beat/miss) beside the ticker — faster to read than MarketBeat's paragraphs.

## 5. Conversion Strategy

- Sticky CTA bar after 1,000ms dwell: "Get the Pre-Earnings AI Brief — free trial"
- Free tier: full calendar, Smart Score pill, 3 ticker row-expands per day
- Premium boundary: unlimited row expands, options expected-move, AI brief, CSV export, alert rules
- Upgrade hook: "Watchlist alerts for earnings surprises" on add-to-watchlist click
- Trust elements: analyst accuracy badges, "Data as of HH:MM ET", source attribution per field, SEC EDGAR link
- Engagement: save filter preset (requires free account); email a weekly digest (free account hook)
- Social proof row: "Watched by 12,443 investors this week" per high-interest ticker
- Exit intent (desktop only, mobile avoids it): one-tap "email me this week's top 10 earnings"

## 6. Editorial Guidance

- Tone: analyst-grade, calm, factual; no hype language, no "could skyrocket"
- Depth: evergreen scaffolding (how to read, confirmed vs. estimated, what moves stocks post-earnings) with dated weekly spotlight blocks
- Freshness frequency: calendar auto-refreshes every 15 min during market hours; editorial "spotlight" updated every Sunday night and Wednesday morning
- E-E-A-T: byline from in-house markets editor, methodology links to TipRanks' accuracy methodology, dated "last reviewed" per editorial block
- Transparency: note which fields are consensus vs. proprietary, link each estimate source
- Accessibility: all data readable without hover (focus states, screen-reader labels on sparklines, contrast-tested dark mode)

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume evergreen cluster, SERP currently thin; recurring seasonal spikes 4x/year |
| Business upside | 5 | Every row is a Premium upgrade surface; aligns with portfolio alerts product |
| UX complexity | 4 | Dense table + filters + inline expand + mobile parity is non-trivial |
| Engineering complexity | 4 | Live data refresh, options expected-move, AI brief caching, schema at scale |
| Recommended rollout speed | 5 | Ship MVP (calendar + Smart Score + filters) within 2 weeks to catch Q3 season; iterate on AI brief and expected-move modules through November |

---

*Prepared 2026-10-06 for the TipRanks SEO program.*
