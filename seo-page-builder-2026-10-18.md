# SEO Page Builder — 2026-10-18

**Cluster:** Earnings Calendar
**Why today:** Peak Q3 2026 earnings season (banks reported last week; mega-caps and consumer names cluster across the next three weeks). Search volume for `earnings calendar`, `earnings this week`, and ticker-level `[ticker] earnings date` is at the quarterly high. This is the moment to ship a 10x calendar — users are returning daily, not once.

---

## 1. Page Thesis

An earnings calendar is the second-most-visited data page on any serious finance site during a reporting season — people check it the way they check weather. The page is for retail investors and active traders who want to know *what's reporting, when, what's expected, and what to do about it* — not just a list of names on a date. It deserves to rank because incumbents treat earnings as a passive date table and skip TipRanks' unique context (analyst consensus accuracy, Smart Score at report time, insider/hedge-fund positioning into the print). It converts because every row is a doorway into a stock page, and every stock page has a premium wall.

## 2. Search Intent Breakdown

- **Primary intent (navigational-informational):** "Who reports this week / today / before open?" — a time-filtered list with company, ticker, time of day, EPS consensus.
- **Secondary intent (preparation):** "What should I expect from this print?" — consensus beat/miss history, options-implied move, analyst sentiment going in.
- **What users really want:** Not a table. A triage tool — filter by watchlist, market cap, sector, confirmed vs. estimated date, and surface *which prints matter to me*.
- **What makes them bounce:** Static date tables with no times (BMO/AMC), no estimates, stale data, interstitials, no mobile filtering, and dead ticker links that go to a thin stub rather than a real stock hub.

## 3. 10x Page Blueprint

- **Page type:** Interactive data hub (calendar + grid) with persistent URL state for date, filter, and view mode. Programmatic sub-pages for `/earnings-calendar/[date]`, `/earnings-calendar/this-week`, `/earnings-calendar/[sector]`, and `/stocks/[ticker]/earnings`.
- **Title tag:** `Earnings Calendar — This Week's Earnings Reports & Expectations | TipRanks`
- **Meta description:** `Track every company reporting earnings this week with analyst consensus, Smart Score, options-implied moves, and hedge fund positioning. Filter by date, sector, or your watchlist.`
- **H1:** `Earnings Calendar: This Week's Reports With Analyst Expectations`
- **H2 / H3 outline:**
  - H2 `Earnings This Week` (default view, Mon–Fri strip with BMO/AMC lanes)
    - H3 `Today's Confirmed Reports`
    - H3 `Pre-Market (BMO)` / `After-Hours (AMC)`
  - H2 `Highest-Impact Reports` (ranked by market cap × implied move × analyst-coverage breadth)
  - H2 `What Analysts Expect` (consensus EPS, revenue, YoY, surprise history — the "going-in" view)
  - H2 `Smart Score Into Earnings` (TipRanks composite as of print)
  - H2 `Hedge Fund & Insider Activity Before the Print` (positioning in the quarter leading up)
  - H2 `Options-Implied Move vs. Historical Move`
  - H2 `My Watchlist Earnings` (gated: logged-in module)
  - H2 `Last Week's Results` (beat/miss recap, auto-generated)
  - H2 `How to Use the Earnings Calendar` (brief; FAQ-shaped for SGE/AIO)
  - H2 `FAQ` (BMO vs AMC, confirmed vs estimated, where estimates come from, how Smart Score factors earnings)
- **Recommended modules:**
  - Date strip (±14 days, keyboard-navigable, URL-stateful)
  - Row-level mini-card on hover: EPS/rev consensus, last 4 surprises sparkline, Smart Score, analyst count, insider last 90d, hedge-fund delta last 13F
  - "Confirmed vs. estimated date" badge with source timestamp
  - Watchlist overlay (free account gate → premium for alerts)
  - Sector / market-cap / country / exchange filters
  - "Download .ics" for individual tickers (sticky, high-intent)
- **Interactive components:**
  - Server-rendered table with client-side filter/sort for crawlability
  - "Only my watchlist" toggle (sign-in CTA for anonymous users)
  - Earnings-day countdown on each row during active week
  - Pre/post-print toggle: before the print → expectations; after → actuals vs. estimate
- **Visual/data components:**
  - Beat/miss history sparkline (8 quarters)
  - Options-implied move gauge vs. 8-quarter realized-move average
  - Smart Score gauge (TipRanks proprietary) with sub-component breakdown on hover
  - Analyst track-record accuracy badge next to consensus (TipRanks' moat)
- **Schema opportunities:**
  - `ItemList` for the day's reports
  - `Event` schema per ticker/date (name, startDate with timezone, performer=Company)
  - `FAQPage` for the FAQ block
  - `BreadcrumbList` for date and sector sub-pages
  - `FinancialProduct` + `Organization` links on ticker rows
- **Internal linking strategy:**
  - Every ticker row links to `/stocks/[ticker]` and the dedicated `/stocks/[ticker]/earnings` sub-hub
  - Date pages cross-link to `/stocks/[ticker]/forecast` (analyst), `/stocks/[ticker]/hedge-fund-activity`, `/stocks/[ticker]/insider-trading`, `/stocks/[ticker]/smart-score`
  - Sector-filtered views link to `/stocks/sector/[sector]/earnings` and sector screeners
  - "Dividend payers reporting this week" cross-link into `/dividends` hub
  - Compare module: pick two tickers reporting same day → `/compare/[a]-vs-[b]`

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- What they do: Clean, fast earnings calendar table with EPS/revenue consensus. Minimal visual noise. Strong UX.
- Where they're weak: No proprietary signal going into the print, no analyst-accuracy weighting, no hedge-fund or insider overlay, no watchlist personalization at scale, limited post-print narrative.
- How TipRanks beats them: Add the *why it matters* layer — Smart Score, analyst track-record-weighted consensus (not just raw mean), hedge-fund positioning delta, insider trading in the 90 days before the print.
- Above the fold: Smart Score + analyst-accuracy-weighted consensus beat/miss probability for the top 5 highest-impact reports today.

**Barchart.com**
- What they do: Dense, feature-rich calendar with options data, implied moves, and historical surprise. Power-user depth.
- Where they're weak: Interface is cluttered and ad-heavy; mobile experience is poor; no proprietary composite; implied-move data is behind inconsistent paywalls; no social/sentiment overlay; data freshness varies by row.
- How TipRanks beats them: Match Barchart's data depth (implied move, surprise history) but surface it cleanly with Smart Score as the anchor signal; add blogger/expert sentiment and insider activity Barchart lacks; superior mobile.
- Above the fold: Clean "highest-impact today" ranked grid with Smart Score, implied move, and hedge-fund delta — the three things Barchart buries.

**MarketBeat.com**
- What they do: Earnings calendar bundled with heavy email-capture CTAs and analyst-rating-change feeds.
- Where they're weak: Table is thin on actual data per row; aggressive pop-ups; analyst coverage lacks accuracy weighting; no proprietary score; no hedge-fund 13F integration; content frequently reads AI-generated and stale.
- How TipRanks beats them: Real data per row instead of an email trap; analysts have *track records*, not just names; original Smart Score; genuine hedge-fund and insider data.
- Above the fold: A usable product, not a lead form. Analyst-accuracy-weighted consensus and Smart Score visible without an email handoff.

## 5. Conversion Strategy

- Free: full week view, consensus EPS/revenue, Smart Score snapshot, last-quarter surprise. Premium: multi-week forward view, watchlist earnings alerts (push + email), analyst-accuracy-weighted consensus with full history, options-implied-move historical overlay, hedge-fund positioning timeline.
- Sticky right-rail CTA on desktop: "Alert me when [stocks on screen] report" — logged-out users prompted to sign up free; logged-in free users prompted to upgrade for alerts beyond 3 tickers.
- In-row upgrade hook on the "Analyst Accuracy-Weighted Consensus" column: free users see the headline consensus; premium users see the weighted number and top-3 most-accurate analysts' individual estimates.
- Trust elements above the fold: "Analyst track records verified across 500K+ ratings," source and timestamp on every data point, "Confirmed by company IR" badge where applicable.
- Post-print engagement module: after the market closes on report day, auto-swap row to "beat/miss, reaction, revised consensus" — brings users back the next morning.
- Watchlist capture: anonymous visitors see a "Add [ticker] to free watchlist" prompt after 30s or on second row-expansion.
- Email: free weekly "Earnings Week Ahead" digest personalized to watchlist; premium: morning-of alerts with pre-print brief.
- Avoid: interstitials, modal pop-ups, email-wall before any data. The MarketBeat tax.

## 6. Editorial Guidance

- Tone: analytical, calm, data-first. No hype language, no "stocks to buy before earnings." Users here are preparing, not being sold.
- Depth: short expectation summaries (60–100 words) auto-generated per high-impact ticker from TipRanks' own analyst, insider, and hedge-fund data — with a human editor reviewing the top 20 names each week.
- Freshness: data refreshes intraday (consensus, confirmed-date status); editorial pre-print briefs refresh daily during peak weeks; post-print recap within 30 minutes of release.
- E-E-A-T: byline every editorial brief with a TipRanks analyst or editor whose track record is itself a TipRanks page; link to the author's methodology; cite primary sources (company IR, SEC filings) with timestamps; show the "last updated" timestamp on every row.
- Avoid syndicated/scraped copy — this is where MarketBeat loses on E-E-A-T.
- Internal author/entity schema with `sameAs` to the TipRanks author profile; `Review`/`Rating` schema where an editorial brief includes a Smart Score snapshot.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Peak seasonal volume; evergreen weekly refresh; strong internal link hub into every ticker page; schema-rich. |
| Business upside | 5 | High-return-visit page during 4–6 weeks per quarter; direct funnel into watchlist (free→premium alert gate). |
| UX complexity | 4 | Date-stateful URL, logged-in watchlist overlay, pre/post-print row swap, hover micro-cards all need design + motion polish. |
| Engineering complexity | 4 | Confirmed-vs-estimated date pipeline, intraday consensus refresh, options-implied-move data integration, per-ticker Event schema at scale, i18n for timezones. |
| Recommended rollout speed | 4 | Ship core calendar + Smart Score + analyst-weighted consensus in 3 weeks to catch late Q3 / Q4 season; layer watchlist alerts, options-implied module, and post-print auto-swap in weeks 4–8. |
