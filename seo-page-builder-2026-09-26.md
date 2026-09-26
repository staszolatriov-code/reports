# TipRanks SEO Page Builder — 2026-09-26

**Selected cluster:** `earnings calendar`
**Why today:** Q3 2026 earnings season begins ~Oct 14 (JPM/WFC/C typically lead). Search volume for "earnings calendar," "earnings this week," and single-ticker "AAPL earnings date" spikes 3–4x from late September through late October. This is the pre-season traffic ramp — the two-week window where the page needs to already be indexed, cached, and structured, not still being built.

---

## 1. Page Thesis

TipRanks' Earnings Calendar should be the single most decision-useful pre-earnings page on the open web: not just *when* companies report, but *what to expect and how to trade around it* — analyst consensus vs. Smart Score, revision momentum in the last 7/30 days, hedge fund positioning changes into the print, insider selling clusters, and historical post-earnings drift. It targets active retail traders, options traders, and pre-market news readers who currently jump between MarketBeat's calendar, Yahoo Finance's list, and a broker screen. It deserves to rank because competitors ship a bare table; TipRanks can ship a table where every row is a mini-thesis. It converts because "next earnings" is the highest-intent, most repeat-visited surface on any finance site — a natural Premium wedge (unlimited filters, alert automation, full history).

## 2. Search Intent Breakdown

- **Primary intent:** "When does [X] report?" and "who reports this week?" — dated, factual, need scannable table
- **Secondary intent:** "How is [X] expected to do?" — EPS/revenue consensus, whisper number, options-implied move, Smart Score trend
- **What users really want:** an actionable pre-earnings scorecard per name — is the Street raising or cutting numbers, are hedge funds adding, are insiders selling, has the stock already run
- **What makes them bounce:** login walls before the table renders, missing tickers, dates that don't match confirmed press releases, no timezone control, no "this week / next week / today AMC/BMO" filter

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (hub + auto-generated per-ticker earnings pages + per-day landing pages)
- **Title tag:** `Earnings Calendar 2026 — This Week's Earnings Reports | TipRanks`
- **Meta description:** `Full earnings calendar with analyst consensus EPS, Smart Score, hedge fund activity, and post-earnings drift for every company reporting this week. Free.`
- **H1:** `Earnings Calendar`
- **H2/H3 outline:**
  - H2: Earnings This Week (default view, US market)
    - H3: Monday / Tuesday / Wednesday / Thursday / Friday tabs
  - H2: Highlighted Reports (curated 6–10 tickers with the biggest expected moves)
  - H2: Filter the Calendar (sector, market cap, exchange, Smart Score, analyst rating, expected move)
  - H2: How to Read This Calendar (consensus, whisper, implied move, drift)
  - H2: Next Week's Earnings
  - H2: Earnings Season Overview (Q3 2026 tracker: % reported, beat rate, revision index)
  - H2: FAQ (BMO vs AMC, confirmed vs estimated dates, why dates change)
- **Recommended modules:**
  - Sticky day-filter tabs with count badges (e.g., "Tue • 47")
  - Row-level expandable drawer: 30/90-day price chart, last 4 quarters' beat/miss, revision heatmap, top 3 analyst calls, hedge fund Δ shares, insider Δ$
  - "Set Alert" inline CTA on every row (email/push)
  - Confidence flag: `Confirmed` (from company IR) vs `Estimated`
  - Currency + timezone toggles
- **Interactive components:**
  - Column-sortable table (market cap, expected move, Smart Score, analyst consensus, days to report)
  - Multi-select ticker watchlist filter ("show only my watchlist")
  - Options-implied move calculator (from ATM straddle) inline in the row drawer
  - Compare-two-companies chip inside a sector cluster
- **Visual/data components:**
  - Post-earnings drift sparkline (last 8 quarters, +1D/+5D return)
  - Revision heatmap tile (EPS estimate delta last 7/30/90d)
  - Smart Score gauge
  - Hedge Fund Signal chip (Positive / Very Positive / Negative)
  - Insider Δ over trailing 90 days
- **Schema opportunities:**
  - `Event` schema per row with `startDate`, `name`, `organizer` (company), `about` (earnings call)
  - `Dataset` schema on the hub
  - `BreadcrumbList` and `FAQPage` for the FAQ block
  - `ItemList` for the "This Week" curated table so Google can surface a rich list
- **Internal linking strategy:**
  - Every ticker row → deep-linked to `/stocks/{ticker}/earnings` (per-ticker earnings history page)
  - Sector chips → sector earnings pages (e.g., `/earnings-calendar/technology`)
  - "See analyst forecasts" → analyst ratings page for that ticker
  - "See hedge fund activity" → 13F holdings page for that ticker
  - Contextual link inside the FAQ to the Smart Score explainer
  - Homepage, stock overview, and screener all link "Next earnings: Oct 30" chip → this page filtered to that ticker

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, minimal earnings calendar table with date, EPS estimate, revenue estimate, market cap.
- *Where they're weak:* No analyst-side signal, no positioning data, no expected move, no per-row drawer, no alerts, no historical drift.
- *How TipRanks beats them:* Every row carries Smart Score, Hedge Fund Signal, insider Δ, analyst consensus with track-record-weighted accuracy — the difference between a schedule and a scoresheet.
- *Above the fold:* Confirmed count, biggest expected movers, Smart Score column visible before scroll.

**Barchart.com**
- *What they do:* Deep data table with pre-market EPS, revenue est., surprise history; skews to power users; heavy interstitials.
- *Where they're weak:* Slow, ad-cluttered, gated columns, dated UX, no positioning data (13F/insiders not native), weak mobile.
- *How TipRanks beats them:* Same data density minus the ad wall, plus proprietary Smart Score + hedge fund + insider + expert sentiment layered in — one page instead of five tabs.
- *Above the fold:* Fast-loading table with sortable columns, no login required, "Confirmed" badges from IR filings.

**MarketBeat.com**
- *What they do:* SEO-forward earnings calendar with heavy internal linking, per-ticker earnings pages, email alerts as the wedge.
- *Where they're weak:* Shallow analytics — consensus and last-quarter EPS but no positioning, no drift chart, template feel across tickers.
- *How TipRanks beats them:* Match MarketBeat's link depth and alert flow, then dominate on data quality — track-record-weighted analyst accuracy, real 13F deltas, insider clusters — plus AI-generated pre-earnings summary per ticker.
- *Above the fold:* AI Earnings Preview card (2 sentences) for the top 5 names of the week — nothing MarketBeat can match without an equivalent AI stack.

## 5. Conversion Strategy

- Free tier: current week's calendar, top 3 sortable columns, one saved filter, one email alert
- Premium wedge: unlimited alerts, full history drawer beyond 4 quarters, revision heatmap, options-implied move, watchlist-only filter, sector deep pages, CSV export
- Sticky "Set Earnings Alerts" CTA in the right rail (visible on scroll, personalized copy: "You're watching NVDA — get alerted 24h before its Oct 30 report")
- Inline upgrade prompt when a user hits the 3rd row-drawer open in a session (soft), or attempts a 2nd alert (hard)
- Trust: "Confirmed via IR" badge with source link, "Updated 2 min ago" timestamp, analyst count and track-record accuracy on every consensus number
- AI Earnings Preview card requires free account (email capture) — the highest-converting hook of the page
- "Add to Google Calendar / Outlook" for any row — free but requires account, drives repeat visits
- Post-earnings recap email auto-sent to alert subscribers — the loop that makes Premium sticky

## 6. Editorial Guidance

- Tone: professional-neutral, no hype, no "MUST BUY" copy — this is a decision surface, not a sell sheet
- Depth: numbers-first; every claim ties to a data point with a hover source; prose limited to the FAQ, the AI preview card, and the season overview
- Freshness: date-modified stamp visible; calendar auto-refreshes date confirmations 4x daily against IR filings; consensus refreshes hourly during market hours; AI previews regenerate 24h before each print
- E-E-A-T: named "Data methodology" link explaining consensus construction and Smart Score, author byline on any editorial commentary (season overview), source citations to company IR pages for confirmed dates, visible last-updated timestamp
- Never: quietly show "estimated" dates as "confirmed" — this is the #1 trust killer on earnings calendars and where competitors lose users
- Never: paywall the current-week table — kills SEO and the free-to-paid funnel starts with the row drawer, not the row itself

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume, evergreen, seasonal 3–4x spikes; MarketBeat currently owns it and is beatable on data depth |
| Business upside | 5 | Highest-intent surface on the site for alert subscriptions — natural Premium wedge and re-visit engine |
| UX complexity | 4 | Row-drawer, filters, timezone, alerts, and per-ticker deep-link all need to feel instant; mobile is the hard part |
| Engineering complexity | 4 | IR-confirmation pipeline, consensus refresh, options-implied move calc, alert delivery infra, per-ticker page auto-generation |
| Recommended rollout speed | 5 | Ship the hub + top-500 per-ticker earnings pages within 2 weeks to catch Q3 season; iterate drawer + AI preview during the season |

---

*Prepared 2026-09-26 · TipRanks SEO Page Builder*
