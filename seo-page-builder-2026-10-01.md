# SEO Page Builder — 2026-10-01

**Selected opportunity:** Earnings Calendar
**Why today:** Q3 2026 earnings season opens next week (big banks lead on 2026-10-07/08), driving a 6-week spike in "earnings calendar", "earnings this week", and "when does [TICKER] report earnings" queries. The cluster has recurring quarterly demand and is the single highest-volume evergreen tool keyword where TipRanks still ranks behind Yahoo Finance, StockAnalysis.com, and MarketBeat.

---

## 1. Page Thesis

An investor-grade, filterable Earnings Calendar hub that answers "who reports when, and does it matter?" in one view. The target user is a self-directed investor or options trader who checks the calendar 2–4x per week during earnings season and wants not just dates, but the TipRanks edge: analyst EPS/revenue consensus, Smart Score, pre-earnings analyst revisions, hedge fund positioning changes, and historical post-earnings price moves. It deserves to rank because every incumbent (Yahoo, Nasdaq, StockAnalysis) ships a flat table — none layer proprietary signals on top of the date. It converts because the calendar is a daily habit surface: once a user builds a watchlist of upcoming reporters, we have 30+ days to upsell premium alerting on Smart Score moves and analyst revisions ahead of the print.

## 2. Search Intent Breakdown

- **Primary:** Transactional-informational — "when does company X report" / "what's reporting this week"; needs a date, time (BMO/AMC), and consensus numbers above the fold.
- **Secondary:** Opportunity-scouting — "best earnings plays this week", "stocks reporting with high short interest / Smart Score"; needs filterable screening.
- **What users really want:** A confidence read — not just the date, but *should I care?* (beat/miss history, analyst momentum into the print, implied move).
- **Bounce triggers:** Stale dates, missing after-hours tags, no ticker filter, consensus numbers hidden behind a login, slow table re-sort, no mobile-friendly day view.

## 3. 10x Page Blueprint

- **Page type:** Dynamic data hub (daily-refreshed calendar) with sub-routes for `/this-week`, `/today`, `/sp500`, and per-ticker deep links.
- **Title tag:** `Earnings Calendar 2026 — This Week's Earnings Reports & EPS Estimates | TipRanks` (58 chars; year token swaps automatically)
- **Meta description:** `Track every upcoming earnings report with analyst EPS consensus, Smart Score, hedge fund activity, and historical post-earnings moves. Updated daily.` (155 chars)
- **H1:** `Earnings Calendar — Upcoming Earnings Reports`
- **H2/H3 outline:**
  - H2: Earnings This Week (default view, Mon–Fri tabs + date picker)
  - H2: Highlighted Reporters (editorially curated: top 10 by market cap × catalyst score)
  - H2: Filter by Smart Score, Analyst Consensus Trend, Market Cap, Sector, Index
    - H3: High Smart Score reporters this week
    - H3: Analyst-upgraded ahead of earnings
    - H3: Heavy hedge fund buying before the print
  - H2: Historical Beat Rate & Post-Earnings Drift (per ticker)
  - H2: How to Read an Earnings Calendar (short, below the fold, for E-E-A-T & long-tail)
  - H2: Earnings Season Calendar — Q3 2026 Reporting Dates (seasonal anchor)
  - H2: FAQ — When do earnings get reported, BMO vs AMC, whisper numbers, confirmed vs estimated dates
- **Recommended modules:**
  - Day-strip header (Mon–Fri with report counts; swipeable on mobile)
  - Primary table: Ticker | Company | Date/Time | EPS Est | Rev Est | Smart Score | Analyst Trend (7-day arrow) | Implied Move | Last Q Beat/Miss
  - "Confirmed vs. estimated date" badge (unique vs. Yahoo which hides this)
  - Watchlist pin button on every row (free, drives sign-up)
  - Pre-earnings analyst revision sparkline (last 30 days)
- **Interactive components:**
  - Multi-select filters that update the URL (shareable deep links → backlinks)
  - "Add to Google/Apple Calendar" one-click .ics export (unique vs. all three competitors)
  - Row expand → mini-chart of last 8 quarters' post-earnings 1-day move
  - "Alert me 24h before" toggle (free: email; premium: SMS + Smart Score change)
- **Visual/data components:**
  - Heatmap: next 4 weeks × sector, cell color = aggregate Smart Score of reporters
  - Donut of this week's reporters by market cap tier
  - Beat-rate dial per ticker (last 8 quarters)
- **Schema opportunities:**
  - `ItemList` for the earnings table (each row an `Event` with `startDate`, `name`, `location: Virtual`, `organizer` = company)
  - `BreadcrumbList`, `FAQPage` on the FAQ block
  - `Dataset` schema on the historical post-earnings move table
  - `SpeakableSpecification` on the "earnings this week" summary paragraph (voice-search)
- **Internal linking strategy:**
  - Every ticker row deep-links to `/stocks/[ticker]/earnings` (per-ticker earnings history page — spin up templated children)
  - Sidebar: "Related tools" → Analyst Forecasts, Smart Score Screener, Hedge Fund Trades, Insider Trading Calendar
  - Footer rail: "Last week's biggest beats/misses" (editorial recap, updates weekly, keeps crawl frequency high)
  - Breadcrumb into `/calendars/` hub (future expansion: dividend calendar, IPO calendar, economic calendar)

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast table with date, time, EPS estimate, EPS actual. Good UX, minimal filtering.
- *Weak:* No analyst momentum, no proprietary score, no hedge fund context, no historical post-earnings move, no alerts.
- *How TipRanks beats:* Smart Score column + analyst-revision sparkline + hedge-fund-activity badge, all above the fold.
- *Above the fold:* Smart Score, 7-day analyst-revision arrow, confirmed-date badge.

**Barchart.com**
- *What they do:* Dense table, strong on options data (implied move), paywalls most filters.
- *Weak:* Cluttered UI, locks the useful columns behind Premier, no retail-friendly explainers.
- *How TipRanks beats:* Keep the implied-move signal free, add Smart Score & analyst trend, cleaner mobile view, free watchlist pinning.
- *Above the fold:* Implied move (free) + Smart Score + "Add to calendar".

**MarketBeat.com**
- *What they do:* SEO-optimized calendar pages, heavy ad load, strong per-ticker earnings sub-pages, email upsell.
- *Weak:* Ad-saturated, slow LCP, analyst coverage summarized not scored, no composite signal.
- *How TipRanks beats:* Faster LCP (<1.8s target), composite Smart Score vs. their list-of-analysts approach, and expert/blogger sentiment (unique).
- *Above the fold:* Smart Score, expert sentiment %, hedge-fund-buying-before-earnings badge.

## 5. Conversion Strategy

- Primary CTA ("Pin to watchlist") on every row — free, requires account, converts anonymous → registered.
- Secondary CTA ("Alert me before this prints") — free tier = email 24h out; premium hook = SMS + Smart Score change + analyst revision alert.
- Free vs. premium line: full calendar, EPS consensus, Smart Score, last-quarter beat/miss are **free**; multi-quarter beat history, pre-earnings insider & hedge-fund delta, and real-time alert bundle are **premium**.
- Above-the-fold trust strip: "Tracking 8,400+ US-listed companies • Analyst track records audited since 2009 • 180M+ data points".
- "This week's TipRanks-flagged plays" editorial module anchored by analyst and Smart Score — proof the proprietary data finds the movers.
- Soft-gate the historical post-earnings drift chart after 2 ticker expansions in a session → sign-up wall (not paywall).
- Premium upgrade modal triggered on 3rd alert set-up, offering 7-day free trial of Premium.
- Exit-intent on mobile: "Get this week's earnings in your inbox every Sunday" → captures email even on bounce.

## 6. Editorial Guidance

- Tone: pragmatic, trader-literate, zero hype. Short declarative sentences. Numbers before adjectives.
- Depth: data-first with a 180–220-word explainer block below the fold for long-tail queries ("what time do earnings come out", "BMO vs AMC meaning") — not a 2,000-word SEO essay.
- Freshness: calendar table re-renders daily at 06:00 ET; "last updated" timestamp visible; weekly editorial recap of biggest beats/misses pushes a fresh crawl signal every Monday.
- E-E-A-T: byline the weekly recap to a named TipRanks analyst with linked bio; link methodology for Smart Score and analyst-track-record scoring; cite SEC filing dates for confirmed earnings.
- Author schema (`Person` with `jobTitle`, `sameAs` to LinkedIn) on the recap post; `Organization` schema with `foundingDate`, `award`, and press-mention `sameAs` on the hub.
- Avoid: speculative "stocks that will beat earnings" clickbait — this cluster is one Google Helpful Content hit away from a demotion, and competitors like MarketBeat already carry that penalty surface area.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Evergreen + quarterly surge; top 3 cluster by non-brand volume; TipRanks currently ranks p2–p3 for most head terms. |
| Business upside | 5 | Daily-habit surface, perfect wedge for alerting upsell; feeds premium Smart Score and analyst-revision product moats. |
| UX complexity | 3 | Table + filters + per-row expand is standard, but mobile day-strip + .ics export + alert flows add real polish work. |
| Engineering complexity | 4 | Needs reliable confirmed-date ingestion, intraday Smart Score snapshot per ticker, scalable per-ticker child pages, schema automation. |
| Recommended rollout speed | 4 | Ship v1 (table + filters + Smart Score column + watchlist pin) within 4 weeks to catch Q3 earnings season; alerts and heatmap in v1.5 by late October. |
