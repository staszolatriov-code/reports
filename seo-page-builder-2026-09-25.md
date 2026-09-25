# SEO Page Builder — 2026-09-25

**Cluster selected:** Earnings Calendar
**Why today:** Q3 2026 US earnings season begins in ~2.5 weeks (mid-October). Search demand for "earnings calendar", "earnings this week", "earnings today", and "companies reporting earnings" is climbing off its seasonal trough. Building/refreshing the hub now captures the ramp instead of chasing it.

---

## 1. Page Thesis

TipRanks' Earnings Calendar should be the single page a retail or semi-pro investor opens each morning during earnings season to see **who is reporting, what the Street expects, what actually happened, and whether the stock is worth owning through the print** — all in one screen. It targets active investors, options traders, and dividend/holding investors preparing for volatility around their names. It deserves to rank because incumbents (Yahoo, Nasdaq, StockAnalysis, MarketBeat) treat the calendar as a passive schedule; TipRanks can fuse it with Smart Score, analyst track record, and hedge fund/insider signals no one else has. It converts because every row is a natural drop-off into a premium-gated pre-earnings intelligence view.

## 2. Search Intent Breakdown

- **Primary intent:** filterable schedule — "who reports today / this week, at what time (BMO/AMC), with EPS and revenue consensus."
- **Secondary intent:** decide **how to trade or hold** the print — implied move, historical beat rate, analyst revisions in the last 7/30 days.
- **What users really want:** confidence to act — a shortlist of *actionable* names for tonight/tomorrow, not a 2,000-row dump.
- **What makes them bounce:** paywall on the schedule itself, stale consensus figures, missing after-hours reactions, no way to filter to *their* watchlist or portfolio, and mobile tables that require horizontal scrolling.

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (dynamic dated landing page) with programmatic day/week/ticker child pages (`/earnings-calendar`, `/earnings-calendar/2026-10-15`, `/earnings/AAPL`).
- **Title tag:** `Earnings Calendar 2026 — Today, This Week & Consensus Estimates | TipRanks`
- **Meta description:** `See every US earnings report with EPS & revenue consensus, Smart Score, analyst track records, and hedge fund activity. Filter by date, sector, market cap, or your portfolio — free.`
- **H1:** `Earnings Calendar`
- **H2/H3 outline:**
  - H2 Today's Earnings *(default view; date-picker + BMO/AMC toggle)*
  - H2 This Week's Earnings *(sub-tabs: Mon–Fri)*
  - H2 Most-Watched Reports This Week *(editorial + traffic-weighted)*
    - H3 Mega-cap prints
    - H3 High implied-move names
    - H3 Recent analyst upgrades reporting soon
  - H2 How To Read an Earnings Report *(evergreen glossary block)*
    - H3 EPS beat vs. revenue beat
    - H3 Guidance and why it moves the stock more than the print
    - H3 Whisper numbers vs. consensus
  - H2 TipRanks Pre-Earnings Signals
    - H3 Smart Score before the print
    - H3 Analyst revisions in the last 7 days
    - H3 Insider buying/selling in the last 30 days
    - H3 Hedge fund position changes last quarter
  - H2 After the Bell: Yesterday's Results & Reactions
  - H2 Earnings Season Playbook *(Q3 2026 edition, refreshed quarterly)*
  - H2 FAQ
- **Recommended modules:**
  - Sticky filter bar (date, sector, market cap, exchange, index membership, "My Watchlist", "My Portfolio").
  - Consensus row: EPS est / prior EPS / revenue est / YoY growth / historical beat rate.
  - TipRanks column set: Smart Score, Analyst Consensus (buy/hold/sell), 12-mo price target upside, top-analyst-only price target, hedge fund signal, insider signal.
  - "Confirmed vs. estimated" report-time badge.
  - After-hours / pre-market reaction chip once reported.
- **Interactive components:**
  - Column customizer + saved views (free login required — first conversion moment).
  - Watchlist overlay ("show only my tickers reporting this week").
  - Alerts: "notify me 24h before AAPL reports" (email free / push premium).
  - Implied-move calculator from options chain.
  - "Compare vs. last quarter" mini-modal per row.
- **Visual/data components:**
  - Weekly heat-strip: bar chart of # of reports per day, colored by aggregate Smart Score.
  - Per-ticker sparkline of last 8 quarters' surprise %.
  - Sector treemap for the selected week (size = market cap, color = analyst consensus).
- **Schema opportunities:**
  - `ItemList` for each dated calendar (each row → `FinancialProduct` / `Event`-shaped custom).
  - `FAQPage` on the glossary block.
  - `BreadcrumbList` across `/earnings-calendar/{date}` and `/earnings/{ticker}`.
  - `Dataset` schema on the master hub (freshness + coverage signals for AI overviews / Google Datasets).
  - `Article` + `Person` (author) on the Season Playbook.
- **Internal linking strategy:**
  - Every ticker row → `/stocks/{ticker}/earnings` (dedicated per-ticker earnings history + estimates page).
  - Sector chips → `/sectors/{sector}/earnings-calendar`.
  - Cross-link to Analyst Ratings hub, Smart Score explainer, Hedge Fund Activity hub, Insider Trades hub.
  - "Reporting next week" widget on all `/stocks/{ticker}` pages links back into the calendar for the correct dated URL (long-tail programmatic uplift).
  - Editorial articles ("What to expect from NVDA earnings") canonical-link to the calendar row's ticker earnings page.

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* clean, fast weekly calendar; EPS/rev estimates; basic filters; free.
- *Where they're weak:* no analyst quality layer, no proprietary score, no hedge fund/insider context, no per-user personalization, thin editorial.
- *How TipRanks beats them:* fuse the same clean UX with Smart Score, top-analyst-only consensus, and portfolio filtering.
- *Above the fold:* Smart Score + top-analyst price-target upside on every row.

**Barchart.com**
- *What they do:* deep pro-grade tables; options-implied move; export.
- *Where they're weak:* dense, ad-heavy, feature-gated to Premier, hostile mobile UX, no analyst *accuracy* dimension.
- *How TipRanks beats them:* keep the pro data density but ship a mobile-first design, and add analyst *track record* (not just count of ratings) — a signal Barchart structurally doesn't have.
- *Above the fold:* implied move + historical beat rate + top-analyst consensus in a single row.

**MarketBeat.com**
- *What they do:* SEO-heavy calendar with heavy email-capture; strong per-ticker earnings pages; consensus + "confirmed" badges.
- *Where they're weak:* aggressive interstitials, thin proprietary data, no hedge-fund/insider fusion on the calendar, editorial reads AI-generated.
- *How TipRanks beats them:* real analyst track-record data, hedge fund position deltas from 13F, insider transactions from Form 4 — none of which MarketBeat originates.
- *Above the fold:* hedge fund + insider signal chips next to the consensus row.

## 5. Conversion Strategy

- Free tier: full calendar, consensus, Smart Score badge, top-3 analyst consensus.
- Premium hooks: full analyst list with individual track records, unlimited watchlist alerts, options implied-move, "pre-earnings AI brief" per ticker.
- Sticky right-rail CTA card: "See the top-analyst-only price target for [row user is hovering]" → soft paywall preview.
- "Add to watchlist" as the primary CTA on every row (login wall → account creation → email capture).
- Post-print re-engagement: automatic email the morning after a watched ticker reports with the TipRanks reaction summary.
- Trust: show analyst accuracy percentiles, cite source (Form 4, 13F), timestamp every data point.
- Engagement: streak counter for logging in during earnings season; leaderboard of "most-accurate analysts this season" refreshed daily.
- Upgrade prompt is *contextual*, never modal on load — it fires on the third row expansion or on watchlist add #4 (free cap).

## 6. Editorial Guidance

- Tone: crisp, analytical, decision-oriented; assume the reader owns positions.
- Depth: hub stays scannable; ticker-level and playbook pages go deep with charts and cited data.
- Freshness: consensus refreshed intra-day; "confirmed vs. estimated" times updated hourly; Season Playbook rewritten each quarter with a visible "Updated {date}" stamp.
- E-E-A-T: named market analyst byline on the Playbook and per-mega-cap previews, with credentials and TipRanks track record; link to author page with `Person` schema.
- Cite primary sources on every data point (company IR page for confirmed dates, SEC EDGAR for 13F/Form 4, exchange feed for reactions).
- Never publish AI-only editorial on this hub; human-edited previews for the top 25 reports each week.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Evergreen high-volume head term with strong seasonal spikes 4×/yr; programmatic dated + ticker children unlock long tail. |
| Business upside | 5 | Every row is a natural upgrade moment; earnings watchers convert to premium at above-portfolio-average rates. |
| UX complexity | 4 | Dense table + filters + personalization + mobile-first is non-trivial; column customizer and saved views add scope. |
| Engineering complexity | 4 | Real-time consensus feed, confirmed-date scraping, options implied-move calc, per-user watchlist overlay, and dated URL generation for SEO. |
| Recommended rollout speed | 5 | Ship MVP (hub + today/week views + Smart Score column + watchlist filter) **before Oct 10** to catch Q3 season; layer implied-move, sector treemap, and AI briefs in the following 2–3 sprints. |

---

*Prepared 2026-09-25 for TipRanks SEO & Growth.*
