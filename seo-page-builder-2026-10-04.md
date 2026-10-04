# SEO Page Builder — 2026-10-04

**Selected opportunity:** `earnings calendar`
**Why today:** Q3 2026 earnings season opens the week of Oct 12 with the big U.S. banks (JPM, WFC, C) and extends through early November with mega-cap tech. Search demand for "earnings calendar", "earnings this week", and "[ticker] earnings date" is seasonally peaking right now, and the SERP is dominated by lightweight calendar grids that under-serve users who really want to decide whether to hold, hedge, or trade around a print.

---

## 1. Page Thesis

TipRanks' Earnings Calendar should be the only earnings calendar on the web that answers *"what should I do about this print?"* instead of just *"when is this print?"*. It is for active retail investors, options traders, and dividend/portfolio holders who need to see upcoming earnings ranked by *consequence to them* — their holdings, their watchlist, the market's biggest movers — overlaid with analyst expectations, Smart Score, insider activity in the last 90 days, and historical post-earnings drift. It deserves to rank because the top-ranking competitors publish a date table and nothing else; it converts because every row is a doorway into a premium-gated "Earnings Prep" view that costs a login to open and a subscription to see in full.

## 2. Search Intent Breakdown

- **Primary intent:** find a filterable, date-sorted list of upcoming earnings reports (today, this week, next week, by sector, by market cap).
- **Secondary intent:** for a specific ticker on the calendar — EPS/revenue consensus, whisper number, prior beat/miss history, expected move from options.
- **What users really want:** a yes/no signal on *"is this earnings print likely to move my position, and in which direction is the setup leaning?"* — which no competitor currently delivers.
- **What makes them bounce:** stale dates, no pre-market vs. after-market tag, no estimates on the row, popups/registration walls before the calendar renders, and tables that cannot be sorted or filtered without a page reload.

## 3. 10x Page Blueprint

- **Page type:** Interactive data tool / evergreen landing page (not a blog post). Pure product surface with heavy internal linking.
- **Title tag:** `Earnings Calendar 2026 — This Week's Earnings Reports, Estimates & Analyst Forecasts | TipRanks`
- **Meta description:** `See every upcoming earnings report with analyst estimates, Smart Score, insider activity, and expected moves. Filter by date, sector, market cap, or your watchlist — updated in real time.`
- **H1:** `Earnings Calendar: Upcoming Earnings Reports With Analyst Forecasts`
- **H2 / H3 outline:**
  - H2 `This Week's Highest-Impact Earnings` (editorial module, auto-generated from Smart Score + market cap + options expected move)
  - H2 `Full Earnings Calendar` (the main interactive table)
    - H3 `Filter by date, sector, market cap, or your portfolio/watchlist`
    - H3 `Pre-market vs. after-market reports`
    - H3 `Confirmed vs. estimated dates`
  - H2 `How to Read an Earnings Row on TipRanks`
  - H2 `What TipRanks Shows That Other Earnings Calendars Don't`
  - H2 `Earnings Season 2026: Dates to Know` (editorial cadence block, refreshed quarterly)
  - H2 `Earnings Calendar FAQ` (schema-eligible)
- **Recommended modules:**
  - "My Earnings This Week" (logged-in users — pulls their portfolio + watchlist tickers off the full calendar).
  - "Biggest Expected Movers" (sorted by implied-move % from options chain).
  - "Smart Score vs. Street" tile per row.
  - "Analyst Price Target Change in Last 30 Days" sparkline per row.
  - "Insider Activity Last 90 Days" dot indicator per row (buy/sell net).
  - "Hedge Fund Signal" column (TipRanks' hedge fund confidence delta QoQ).
  - "Earnings Reaction History" micro-chart (last 8 quarters of 1-day post-earnings return).
- **Interactive components:**
  - Column-level filters that update the URL (sharable / crawlable states for `/earnings-calendar/this-week`, `/earnings-calendar/sector/technology`, `/earnings-calendar/sp500`).
  - Watchlist-aware highlighting (requires login — soft gate).
  - "Set an earnings alert" button on every row (email/push — email capture is the primary free-tier conversion event).
  - Sortable by: date, time (BMO/AMC), market cap, Smart Score, analyst consensus, implied move, prior quarter surprise.
- **Visual/data components:**
  - Heatmap strip at the top: next 10 trading days, intensity = aggregate market cap reporting that day.
  - Per-row "beat/miss" ribbon showing the last 4 quarters as colored dots.
  - Mini "expected move cone" chart in the row-expand drawer.
- **Schema opportunities:**
  - `ItemList` for the calendar rows (each row an `Event` subtype).
  - `FAQPage` for the FAQ H2.
  - `BreadcrumbList` back to `/earnings/`.
  - Per-ticker rows link to `FinancialProduct` / `Corporation` entities already defined on TipRanks' stock pages.
- **Internal linking strategy:**
  - Every ticker row deep-links to that stock's dedicated earnings tab (`/stocks/<ticker>/earnings`), its forecast page, and its Smart Score page.
  - Date headers link to a date-pinned archive (`/earnings-calendar/2026-10-14/`) — generates long-tail hits like *"earnings october 14 2026"*.
  - Sector filters produce canonical sector-earnings pages (`/earnings-calendar/sector/semiconductors`).
  - Cross-link to Price Target Tracker, Analyst Forecasts hub, and Insider Trading dashboard.
  - "Earnings Season 2026" editorial block links out to a *Q3 2026 Earnings Preview* longform piece and vice versa.

## 4. Differentiation vs. Competitors

### StockAnalysis.com
- **What they do:** Clean, fast earnings calendar with EPS/revenue estimates, actuals once reported, and a basic time-of-day tag.
- **Where they're weak:** No analyst-rating context on the row, no portfolio/watchlist awareness, no options-implied move, no insider signal, no post-earnings drift history. It's a well-designed read-only table.
- **How TipRanks beats them:** Every row is a decision support unit, not just a date lookup. Smart Score + 30-day target revisions + insider net + hedge fund signal + implied move are the five above-the-fold columns that StockAnalysis simply does not have.
- **Above the fold:** "This Week's Highest-Impact Earnings" ranked card deck pulling Smart Score + implied move — a module they can't replicate without TipRanks' proprietary scoring.

### Barchart.com
- **What they do:** Dense, pro-grade earnings calendar with lots of columns, estimate revisions, and options data. Powerful but intimidating.
- **Where they're weak:** UX is 2010-era: hostile paywalls on the useful columns, cluttered filters, no narrative layer, no "what should I do" interpretation, mobile experience is poor. SERP CTR suffers.
- **How TipRanks beats them:** Same data density but with Smart Score as a one-glance verdict, a mobile-first layout, and editorial "Biggest Expected Movers" context. The free tier shows *more* actionable columns than Barchart's free tier.
- **Above the fold:** Smart Score column visible to logged-out users (Barchart hides implied move behind Premier) + a sector heatmap strip.

### MarketBeat.com
- **What they do:** Earnings calendar embedded in a heavily ad-monetized newsletter funnel. Fine data, good email capture.
- **Where they're weak:** Ad-heavy LCP damages Core Web Vitals and user trust; data lacks a proprietary signal; no serious options or hedge-fund data; mobile layout shifts.
- **How TipRanks beats them:** Clean product-grade UI, meaningfully faster LCP, and signals MarketBeat cannot produce — hedge-fund QoQ delta and analyst track-record-weighted consensus. Same email-capture value prop ("alert me") but tied to a product users keep opening.
- **Above the fold:** Watchlist-filtered calendar (free with a login) + hedge-fund-flow indicator per row.

## 5. Conversion Strategy

- CTA 1 (above the fold, free): "Add to watchlist" / "Alert me before this earnings print" — email capture, no credit card.
- CTA 2 (row-expand drawer, free): "See full analyst forecast for [TICKER]" — bounces to the forecast page, which is itself a conversion funnel.
- CTA 3 (soft paywall at row 25 of 500): "See the full Smart Score + hedge-fund signal — free TipRanks account."
- CTA 4 (hard premium hook): "Earnings Prep report" — the per-ticker synthesized view (implied move + options skew + insider net + analyst track-record-weighted target) is Premium.
- Free vs. Premium boundary: dates, estimates, time-of-day, Smart Score (last 7 days), and basic beat/miss history stay free; options-implied move, hedge-fund delta, analyst *track-record-weighted* consensus, and the full "Earnings Prep" PDF export are Premium.
- Trust elements: "Updated 3 minutes ago" timestamp, analyst count behind each consensus, source attribution for options data, visible last-8-quarter accuracy of TipRanks' own earnings-move signal.
- Engagement loop: logged-in users see a "You hold 4 of this week's reporters" banner — the single highest-converting module in the design.
- Retention: on earnings day, email/push to subscribers *"[TICKER] reports after close — here's the TipRanks setup"* — brings them back to the page the day of the print.

## 6. Editorial Guidance

- Tone: calm, data-forward, decision-oriented — like a terminal, not a tabloid. Zero hype language around individual tickers.
- Depth: the calendar is the product; editorial is scaffolding. The "This Week's Highest-Impact Earnings" and "Earnings Season 2026" blocks are 150–250 words each, refreshed weekly / quarterly respectively.
- Freshness frequency: calendar data real-time; editorial callouts refreshed Sunday evening (US) and intra-week when a major company confirms a surprise date; a short "Earnings Season Preview" longform at the start of each quarter.
- E-E-A-T — Experience: show "Last 8 quarters: our implied-move signal called direction correctly X% of the time" with transparent methodology.
- E-E-A-T — Expertise & Authority: byline the quarterly preview to a named TipRanks analyst with a linked author bio page and prior published work.
- E-E-A-T — Trust: clearly disclose data vendors for options and estimates, show last-updated timestamps per row, and link methodology for Smart Score and hedge-fund signal.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume evergreen head term plus a long tail (date-pinned, sector, ticker-earnings-date) that competitors have not systematically captured. Dated-URL strategy multiplies crawlable surface. |
| Business upside | 5 | Earnings is the single most reliable intent trigger for premium conversion — users show up with a question that only TipRanks' proprietary signals can fully answer. |
| UX complexity | 3 | Table + filters + row-expand drawer is a known pattern; watchlist awareness and the implied-move cone are the only novel pieces. |
| Engineering complexity | 4 | Real-time estimates ingest, options-implied-move pipeline, watchlist join on the server, and 500+ dated/sector URL variants with proper canonicalization. |
| Recommended rollout speed | 4 | Ship v1 (table + Smart Score + estimates + watchlist) within 4 weeks to catch Q3 earnings tail; iterate hedge-fund delta, implied-move cone, and dated archives through November for Q4 preview launch.
