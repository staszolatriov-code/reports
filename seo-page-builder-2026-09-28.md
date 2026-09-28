# SEO Page Builder — 2026-09-28

**Selected opportunity cluster:** Earnings Calendar
**Primary head term:** `earnings calendar`
**Supporting terms:** `earnings this week`, `earnings today`, `next week earnings`, `Q3 earnings calendar 2026`, `[TICKER] earnings date`, `earnings whisper`, `after hours earnings`, `pre-market earnings`

**Why today:** Q3 2026 earnings season kicks off the week of Oct 13 (big banks, then mega-caps late October). Search demand for "earnings calendar" and "earnings this week" is entering its steepest 90-day ramp of the year. Every day between now and Nov 10 is a high-CTR window; a strong hub shipped this week compounds through the entire cycle.

---

## 1. Page Thesis

The TipRanks Earnings Calendar is the anchor hub for one of the most predictable, recurring intent surges in retail finance: traders and investors trying to answer "who reports when, and does it matter to me?" The page targets active retail investors, options traders, and news-driven momentum traders in the 24-hour window before/after a print. It deserves to rank because competitors ship a flat table — TipRanks can ship a decision surface layered with analyst consensus, Smart Score, historical beat/miss rates, price-target moves post-print, and hedge-fund positioning going in. It converts because users arrive with a *specific ticker in mind* and a *time-boxed question*, which is the highest-purchase-intent state in finance search.

## 2. Search Intent Breakdown

- **Primary intent:** "Show me a scannable list of upcoming earnings this week/today, sortable, with the tickers I care about surfaced first."
- **Secondary intent:** "For each report, tell me whether to expect a beat, how the stock usually reacts, and what the smart money is doing."
- **What users really want:** A go/no-go decision on holding, buying, or trading options around the print — not a data table.
- **What makes them bounce:** Login walls before the calendar renders, no consensus estimate visible above the fold, no way to filter to "my watchlist / S&P 500 / large-cap only," stale historical data, and interstitial ads on mobile.

## 3. 10x Page Blueprint

**Page type:** Interactive product hub (calendar + data grid + entity detail drawer). Not an article.

**Title tag:** `Earnings Calendar 2026 — This Week's Earnings, Estimates & Smart Score | TipRanks` (68 chars)

**Meta description:** `Track every upcoming earnings report with analyst consensus, historical beat rates, Smart Score, and hedge fund positioning. Filter by date, sector, or watchlist — before and after the bell.` (203 chars)

**H1:** `Earnings Calendar`

**H2 / H3 outline:**
- H2: This Week's Earnings (default view)
  - H3: Today (Before Market Open / After Market Close split)
  - H3: Tomorrow
  - H3: Rest of week
- H2: Highest-Impact Reports This Week (curated: mega-caps + high-volatility names)
- H2: Filter & Customize
  - H3: By sector / market cap / index membership
  - H3: My Watchlist earnings
- H2: How to Read an Earnings Report (evergreen explainer, collapsible)
- H2: Last Week's Earnings Recap (beats, misses, biggest post-print moves)
- H2: Next Week / Next Month Preview
- H2: FAQ (12–15 questions, FAQPage schema)

**Recommended modules:**
- **Above-fold calendar grid** — sortable columns: Ticker, Company, Time (BMO/AMC), EPS Estimate, Revenue Estimate, Smart Score, Analyst Consensus, Historical Beat Rate (last 8 qtrs), Avg 1-Day Move.
- **Ticker detail drawer** — slides out on row click without navigation: consensus estimate, whisper, last-4-quarter EPS actual vs est chart, top hedge fund adds/trims last quarter, insider transactions in the 90 days pre-print, analyst target price changes in the last 30 days.
- **"Smart Money Signal" badge** — proprietary composite flag when Smart Score ≥ 8 AND hedge fund activity is net-buying AND analyst PT was raised in last 14 days.
- **Post-print module** — auto-populates within 15 min of the release with beat/miss deltas and Smart Score delta.
- **Options implied move** — pre-print (premium teaser: locked past a 3-ticker/day cap).
- **Watchlist overlay** — logged-out users see 3 free ticker slots.

**Interactive components:**
- Date range chip picker (Today / This Week / Next Week / Custom)
- Sector multi-select
- Market-cap slider
- Beat-rate threshold filter
- CSV export (premium)
- Calendar sync (Google/Outlook .ics — free, drives return visits)

**Visual/data components:**
- Sparkline: EPS actual vs est last 8 quarters (inline in each row on hover)
- Heat-strip: sector-level earnings density by day-of-week
- Stat tiles above fold: `X companies report this week` / `Y% beat rate last quarter` / `Top expected mover: TICKER`

**Schema opportunities:**
- `FAQPage` for the FAQ section
- `Event` schema per earnings report (name, startDate, organizer=company, description with consensus estimate) — under-indexed by competitors, real SERP feature opportunity
- `Dataset` on the calendar itself
- `BreadcrumbList`
- `SoftwareApplication` for the interactive tool

**Internal linking strategy:**
- Every ticker row → `/stocks/[ticker]/earnings` (dedicated earnings history page — build if missing)
- "Smart Score" tooltip → `/tools/smart-score` explainer
- "Analyst Consensus" column → `/stocks/[ticker]/forecast`
- "Hedge Fund Activity" badge → `/stocks/[ticker]/hedge-fund-activity`
- Sector chips → sector earnings sub-pages (`/earnings-calendar/technology`)
- Footer: link to `/dividend-calendar`, `/ipo-calendar`, `/economic-calendar` — reciprocal hub linking
- Blog: every earnings preview/recap article deep-links back to the ticker row's anchor

## 4. Differentiation vs. Competitors

**StockAnalysis.com** — Ships a clean, fast, minimalist earnings calendar table. Weak on: no proprietary signal, no hedge-fund/insider overlay, no post-print delta, no options implied move, no historical beat context in-row. **TipRanks wins by:** putting Smart Score + Analyst Consensus + Beat Rate above the fold in the same row, so the user makes a decision without clicking. Data above the fold: Smart Score badge, Analyst Consensus rating, Historical Beat %.

**Barchart.com** — Deep data but UI is dense and dated; requires a paid account for most useful filters (implied move, whisper). Weak on: mobile experience is punishing, no "smart money" narrative layer, buried behind login. **TipRanks wins by:** clean mobile-first grid, free-tier utility that's genuinely useful (3 watchlist slots, .ics export), and a narrative "Smart Money Signal" tag that Barchart cannot match without our analyst/hedge-fund data. Data above the fold: hedge fund net activity indicator, Smart Money Signal badge.

**MarketBeat.com** — Strong on SEO real estate for the head term but the page is ad-heavy, thin on proprietary data, and leans on "consensus" without a track-record layer. Weak on: analyst quality (all analysts weighted equally), no post-print recap, mobile ads crush LCP. **TipRanks wins by:** analyst track-record accuracy (only 5-star analyst consensus shown as a secondary column), post-print recap module, and a materially cleaner mobile experience. Data above the fold: 5-star analyst consensus, analyst PT change last 30 days.

## 5. Conversion Strategy

- **CTA placement:** Sticky right-rail "Unlock Full Calendar Data" card, plus in-drawer soft prompts when a locked column (implied move, full hedge fund detail) is hovered.
- **Free vs. premium boundary:** Free = full calendar list, consensus, Smart Score badge (yes/no visibility), historical beat rate, 3 watchlist slots, .ics export. Premium = implied move, whisper number, full hedge-fund detail per ticker, unlimited watchlist, alerts, CSV export.
- **Upgrade hook #1:** "Get alerted 1 hour before a Smart Score 9+ stock reports" — high-relevance, time-bound.
- **Upgrade hook #2:** Post-print "You called it" / "You missed it" moments — email the free user the day after a report they viewed pre-print, with the outcome + a CTA to see it live next time.
- **Trust elements:** Show "Data updated X min ago" timestamp; link every consensus number to its source-analyst distribution; show TipRanks' own hit-rate on Smart Score 9+ names heading into earnings ("Smart Score 9+ names beat consensus 71% of the time over last 4 quarters" — refresh quarterly).
- **Engagement modules:** Watchlist add/remove without account creation (localStorage), account nudge only after 2nd add.
- **Return-visit hook:** .ics calendar sync — users add their watchlist earnings to Google Calendar and come back for every event.
- **Anti-bounce move:** Do not gate the base table. Ever. Every competitor gates something; being the only ungated option is the moat.

## 6. Editorial Guidance

- **Tone:** Utility-first, no hype, no "buy this stock now." Treat the reader as a decision-maker who is short on time.
- **Depth:** Above the fold is scannable in 5 seconds; drawers hold the depth. Explainer content is collapsible and evergreen, not padding.
- **Freshness frequency:** Calendar data refreshes intraday; page-level "This Week / Next Week" copy refreshes every Monday 6:00 ET; recap module auto-populates; "How to Read" evergreen block reviewed quarterly.
- **E-E-A-T signal — Experience:** Bylined weekly recap post from a TipRanks markets editor with named author, photo, and credentials.
- **E-E-A-T signal — Expertise:** Methodology page linked from every Smart Score / Analyst Consensus tooltip explaining how the score is computed and validated.
- **E-E-A-T signal — Trust:** Data-source citations (SEC filings, company IR) in the footer; last-updated timestamps at row level.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Head term with 250k+ monthly US searches, seasonal spike Oct–Nov, all three named competitors rank shallow with weak proprietary layers. |
| Business upside | 5 | Highest-intent recurring surface in the funnel; each earnings season is a natural re-engagement trigger. Direct line to premium via implied-move and alerts hooks. |
| UX complexity | 4 | Filter grid + drawer + post-print module + watchlist state is non-trivial; must nail mobile. Save v2 (options implied move) for phase two. |
| Engineering complexity | 4 | Real-time post-print ingestion, watchlist persistence, .ics generation, and Event schema per-row need coordinated backend. Reuse existing ticker/earnings data services. |
| Recommended rollout speed | 5 | Ship v1 (calendar + Smart Score column + drawer + .ics) before Oct 12. Phase v2 (implied move, alerts, sector sub-pages) by Nov 1. Missing this earnings season costs a full quarter of compounding SEO. |

---

*Prepared 2026-09-28 for the TipRanks SEO + product-led growth workstream.*
