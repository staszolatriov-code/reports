# TipRanks SEO Page Builder — 2026-09-09

**Selected opportunity cluster:** `earnings calendar`
**Why today:** Q3 2026 earnings season kicks off in ~4 weeks (mid-October). Search volume for "earnings calendar" and "earnings this week" typically climbs 3–5x between mid-September and mid-November. This is the annual moment to ship (or re-ship) the page and capture the seasonal wave before competitor pages solidify their rankings for the cycle.

---

## 1. Page Thesis

An always-live earnings calendar built for the *decision*, not the download. Where competitors show a bare table of tickers and dates, TipRanks shows each upcoming earnings event pre-scored: analyst confidence, historical EPS beat rate, hedge-fund positioning heading in, and a Smart-Score-derived "expected reaction" band. Target audience is the active retail investor who already knows earnings dates matter and wants to know *which of this week's 300 reports are worth acting on*. It ranks because it satisfies a data-heavy intent with proprietary data no competitor owns, and it converts because every row is a doorway into a ticker page gated behind Premium's forecast overlays.

## 2. Search Intent Breakdown

- **Primary intent:** "What companies report earnings this week / today / next week?" — informational-with-transactional-tail.
- **Secondary intent:** "Which of these earnings actually matter / which will move?" — filtering + prioritization.
- **What users really want:** a scannable, filterable list where the *interesting* rows (mega-caps, high-beta, high short interest, high analyst confidence) surface without manual work.
- **What makes them bounce:** static tables that can't be filtered, missing time-of-day (BMO/AMC), no consensus EPS/revenue, ad-heavy layouts, and pages that force a login before showing a single date.

## 3. 10x Page Blueprint

- **Page type:** Product-led data landing page (calendar hub) + programmatic per-day and per-week sub-pages (`/earnings-calendar/2026-10-14`, `/earnings-calendar/this-week`, `/earnings-calendar/premarket`).
- **Title tag:** `Earnings Calendar 2026 — This Week's Reports, Estimates & Smart Score | TipRanks`
- **Meta description:** `Track every upcoming earnings report with consensus EPS, revenue estimates, analyst confidence, hedge-fund positioning, and TipRanks Smart Score. Filter by date, sector, market cap, or before/after the bell.`
- **H1:** `Earnings Calendar — Every Report, Pre-Scored`
- **H2 / H3 outline:**
  - H2: This Week's Earnings (default view, live table)
    - H3: Before Market Open
    - H3: After Market Close
  - H2: High-Confidence Reports This Week *(TipRanks proprietary filter)*
  - H2: Most-Watched by Hedge Funds *(proprietary)*
  - H2: Full Earnings Calendar (calendar grid, click any date)
  - H2: How TipRanks Scores an Earnings Report (E-E-A-T + methodology)
  - H2: Last Week's Beats & Misses *(retention hook + evergreen internal linking)*
  - H2: Earnings FAQ (schema-eligible)
- **Recommended modules:**
  - "Smart Filter Bar" — sector, market cap, session (BMO/AMC), analyst confidence tier, hedge-fund activity, Smart Score, options-implied move.
  - "Watchlist Overlay" — logged-in users see their tickers highlighted; free CTA to create one.
  - "Expected Move" column — options-implied straddle move alongside historical average post-earnings move.
  - "Whisper vs. Consensus" delta column.
  - "Insider activity in last 90 days" mini-icon per row (proprietary).
  - Post-earnings companion card: "How the market reacted" for yesterday's reports (retention).
- **Interactive components:**
  - Sticky day selector (Mon–Fri strip with report counts).
  - Column chooser (persist per user).
  - Row-hover mini-panel with the last four quarters' EPS actual-vs-estimate sparkline.
  - "Add to my earnings watchlist" one-click on any row.
  - Time-zone auto-detect with manual override (US ET default).
- **Visual / data components:**
  - Density heatmap: reports-per-day bars above the table so users instantly see the busy days.
  - Beat/miss sparkline per row (last 4–8 quarters).
  - Smart Score dial (color-coded 1–10).
  - Analyst rating pill (Strong Buy / Buy / Hold / Sell / Strong Sell) inline.
- **Schema opportunities:**
  - `ItemList` for the day's reports.
  - `Event` schema per earnings report (name = "AAPL Q4 2026 Earnings Report", startDate, eventStatus).
  - `FAQPage` for the FAQ block.
  - `BreadcrumbList` for date sub-pages.
  - `Dataset` schema on the hub declaring the calendar is a queryable dataset.
- **Internal linking strategy:**
  - Every ticker → forecast page, analyst-ratings page, hedge-fund-activity page (3 links per row, not one — pipes link equity into the highest-converting deep pages).
  - Date sub-pages cross-link forward/back day-by-day and to the parent week/month.
  - Sector rollups (`/earnings-calendar/technology`) link to sector heatmaps and top-ranked stock lists.
  - Editorial "Earnings Preview" articles link into the hub with anchor text = ticker + earnings date.

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, minimal earnings calendar with EPS/revenue estimates and market cap. Fast, mobile-friendly.
- *Where they're weak:* Zero proprietary signal — you get consensus and a date, nothing to rank the rows. No hedge-fund, insider, or analyst-track-record layer. No filtering by "which of these are actually worth watching."
- *How TipRanks beats them:* Pre-score every row with Smart Score, analyst confidence, and hedge-fund/insider activity. Convert a data table into a prioritized action list.
- *Above the fold:* Smart-Score-sorted "This week's high-confidence reports" strip, before the full table.

**Barchart.com**
- *What they do:* Deep data with time-of-day and consensus, but pay-walled sorting/filtering and cluttered UX with ads and upsells.
- *Where they're weak:* Free tier is intentionally crippled; interface is a Bloomberg-era grid that intimidates retail; no track-record layer on the consensus (whose estimate?).
- *How TipRanks beats them:* Full-fidelity free calendar (data is the loss-leader); premium unlocks the *forecast overlay*, not the underlying calendar. Show *which* analysts contribute to the consensus with their accuracy scores.
- *Above the fold:* Consensus EPS with an "analyst accuracy weighted" toggle unique to TipRanks.

**MarketBeat.com**
- *What they do:* Broad earnings calendar coverage with heavy SEO focus and email-capture funnels.
- *Where they're weak:* SEO-first, UX-second — pages are long-scroll ad walls with thin interactivity; data freshness lags; no proprietary sentiment layer.
- *How TipRanks beats them:* Modern app-like UX, real-time updates post-report, and the Bloggers/Financial Experts sentiment layer (unique) shown alongside each earnings row.
- *Above the fold:* Sentiment split (bullish/bearish experts on this ticker heading into earnings) — no competitor shows this.

## 5. Conversion Strategy

- **Free tier boundary:** the calendar itself, all dates, consensus EPS/revenue, Smart Score dial (visible, not the underlying breakdown). Free = the "what and when."
- **Premium boundary:** analyst-accuracy-weighted consensus, options-implied vs. historical move overlay, hedge-fund positioning delta into earnings, whisper numbers, post-earnings Smart Score change forecast. Premium = the "should I trade this."
- **In-row CTA:** "Preview →" button opens a modal Earnings Preview; free users see 3/week, then soft paywall with a "See all previews" upgrade.
- **Sticky watchlist CTA:** if signed-out, a persistent "Track earnings for your stocks" strip with one-tap Google/email signup — no credit card.
- **Post-earnings re-engagement:** yesterday's reports show actual vs. estimate with a "See what analysts are saying now" link — feeds them back into a Premium ratings page.
- **Trust elements above the fold:** "Powered by 8,500+ tracked analysts · 45M+ ratings graded for accuracy" line under the H1; small link to methodology.
- **Upgrade hook — the calendar itself is free forever.** Premium is sold on *interpretation*, not access. This removes the biggest bounce driver on competitor pages.
- **Personalization hook:** logged-in users get "Your watchlist this week" pinned to the top — makes the page feel owned and drives daily returns.

## 6. Editorial Guidance

- **Tone:** neutral, data-forward, second-person minimal; sound like a terminal, not a newsletter.
- **Depth:** every methodology claim links to a dedicated explainer (Smart Score, analyst accuracy, hedge-fund methodology) — E-E-A-T anchor.
- **Freshness frequency:** intraday for the current day's reports (post-market-close actuals within 10 minutes of release); overnight full refresh for next 8 weeks of consensus estimates; weekly manual editorial pass on the "How TipRanks Scores an Earnings Report" section.
- **Named authorship:** the methodology and preview sections carry named financial-analyst bylines with credentials and LinkedIn — feeds Person schema.
- **E-E-A-T signals:** methodology page, analyst accuracy audit report (annual), sourced data disclosures ("consensus aggregated from N brokerages"), review dates ("Data updated: 2026-09-09 14:32 ET").
- **Content velocity:** ship 2–3 short "Earnings Preview" articles per week during season, each linking back to the hub with dated URLs — these become the long-tail net for "[TICKER] earnings preview" searches.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Evergreen high-volume head term; programmatic date/sector sub-pages open thousands of long-tail queries; seasonal spike is imminent. |
| Business upside | 5 | Highest-intent audience TipRanks can address — someone checking earnings calendars is a self-identified active investor and prime Premium prospect. |
| UX complexity | 4 | Filter bar + row-hover panels + expected-move calculation + watchlist overlay is real product work, not a static table. |
| Engineering complexity | 4 | Data pipeline needs BMO/AMC classification, options-implied-move calc, near-real-time actuals ingestion, and per-user watchlist joins at page load. |
| Recommended rollout speed | 5 | Ship the MVP (calendar + Smart Score + filter bar + date sub-pages + schema) in 3 weeks to catch the Q3 wave; layer expected-move, whisper deltas, and hedge-fund positioning in a Phase 2 within the same season. |

---

## Ship-week checklist (MVP scope)

1. Hub route + date sub-pages generated for the next 90 days on build.
2. `ItemList` + `Event` + `FAQPage` schema live before submission to Search Console.
3. Filter bar with persisted state (URL params — filtered views become indexable landing pages).
4. Smart Score column + one proprietary "hedge fund activity" icon column visible free tier.
5. Ticker cells triple-link: forecast, analyst ratings, hedge-fund activity.
6. Methodology page shipped with named author and last-reviewed date.
7. Post-earnings "actual vs. estimate" fill within 10 minutes of release for S&P 500 names.
