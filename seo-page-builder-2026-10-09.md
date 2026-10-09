# SEO Page Builder — 2026-10-09

**Opportunity selected:** `earnings calendar`
**Rotation rationale:** Q3 2026 earnings season kicks off this week (big banks report Oct 14–18). Search volume for "earnings calendar," "earnings this week," and "earnings today" peaks the first two weeks of each quarter. Shipping/refreshing this page now captures the full 6–8 week earnings surge and compounds into Q4 2026 reporting (Jan–Feb 2027).
**Target cluster:** earnings calendar / earnings this week / earnings today / upcoming earnings / earnings schedule / earnings date <ticker>

---

## 1. Page Thesis

TipRanks' Earnings Calendar should be the single most actionable earnings page on the open web — not a passive list of dates, but a decision surface that fuses Wall Street's upcoming numbers with TipRanks' proprietary signals (Smart Score, analyst consensus accuracy, hedge-fund positioning, insider buys into the print) so traders can walk away knowing *which* reports to position for, not just *when* they drop. It serves active self-directed traders, swing/options traders, and the "earnings-season-only" retail investor who treats every quarter as a stock-picking event. It deserves to rank because competitors treat the calendar as a date table — TipRanks can turn it into a pre-earnings intelligence hub. It converts because every row is a doorway into a premium-gated signal: EPS surprise probability, pre-earnings insider activity, options-implied move vs. historical, and the Smart Score trajectory into the print.

## 2. Search Intent Breakdown

- **Primary intent:** "What companies report earnings today / this week?" — users want a scannable, filterable, time-ordered list with ticker, date, time (BMO/AMC), and consensus EPS/revenue.
- **Secondary intent:** "Should I trade this earnings print?" — expectations vs. whisper, options-implied move, prior-quarter beat/miss, analyst revisions in the last 7 days.
- **What users really want:** An edge. Not just dates — a view of which reports are mispriced, which have insider conviction, which hedge funds added into, and which analysts (with proven track records) have raised targets going in.
- **What makes them bounce:** Walls of unfiltered tickers with no sector/market-cap/importance filter; stale data that still shows last quarter after reports have printed; no "my watchlist" overlay; interstitial subscription prompts before the user sees a single data point.

## 3. 10x Page Blueprint

**Page type:** Dynamic product/data page (calendar hub) with daily, weekly, and per-ticker sub-pages — not a blog post. Hub + spoke template with programmatic SEO at the ticker level (`/earnings/<TICKER>`).

**Title tag:** `Earnings Calendar 2026: Companies Reporting This Week with EPS Estimates | TipRanks` (58 chars + brand)

**Meta description:** `Track every upcoming earnings report with analyst consensus, Smart Score, insider activity, and hedge-fund positioning going into the print. Updated every market minute.` (164 chars)

**H1:** `Earnings Calendar — Upcoming Reports with Analyst & Insider Signals`

**H2 / H3 outline:**
- H2: Earnings This Week — [Oct 13 – Oct 17, 2026]
  - H3: Monday — Pre-Market Reports
  - H3: Monday — After-Hours Reports
  - (repeat Tue–Fri)
- H2: Today's Highest-Conviction Earnings (Smart Score ≥ 8 + Hedge Fund Buy Signal)
- H2: Earnings Beat/Miss Probability — How We Score Each Print
- H2: This Season's Biggest Expected Movers (Options-Implied Move ≥ 8%)
- H2: Pre-Earnings Insider Buys (Last 90 Days)
- H2: Analyst Revisions Into the Print (Last 7 Days)
- H2: Earnings Calendar by Sector
- H2: Earnings Calendar by Market Cap (Mega / Large / Mid / Small)
- H2: International Earnings Calendar (UK, EU, Canada, Asia)
- H2: Economic Calendar — Macro Events Alongside Earnings
- H2: How to Trade Earnings Season — TipRanks Framework
- H2: FAQ

**Recommended modules:**
1. Day-selector pill row (Today / Tomorrow / This Week / Next Week / Custom range) — sticky
2. Multi-filter rail (Sector, Market Cap, Smart Score ≥ X, Analyst Consensus = Strong Buy, Has Insider Buys, In My Watchlist, Country)
3. Primary earnings table (sortable, dense-vs-comfortable toggle)
4. "Conviction stack" card per row — Smart Score dial + hedge fund net flow arrow + insider buy badge + analyst revision delta
5. Pre-earnings expectations panel (consensus EPS, consensus revenue, whisper number, prior-quarter beat %)
6. Options-implied move vs. historical realized move (bar comparison)
7. "What TipRanks' top analysts say" — filter to analysts in the top decile of track record for this ticker
8. Hedge Fund Trend module — net buy/sell among 13F filers in the last quarter
9. Insider Transactions ticker-tape (uninformative "Form 4 sell for taxes" filtered out)
10. Post-earnings replay (collapsible) — yesterday's reporters: actual vs. consensus, after-hours move, Smart Score change
11. Export to CSV / Add to Google Calendar / Push Alert (gated to signed-in users)

**Interactive components:**
- Server-rendered, hydrated filter state (shareable via URL params — critical for internal linking and backlinks)
- Row-expand drawer with full pre-earnings dossier (no page jump)
- "Alert me when <TICKER> reports" one-click subscribe
- Watchlist overlay (highlight rows in watchlist, pin to top)
- Dark/light theme-aware chart glyphs
- "Compare this quarter vs. last 4" sparkline per row

**Visual/data components:**
- Smart Score dial (0–10) rendered inline per row — a visual that no competitor has
- Analyst consensus pie (Buy/Hold/Sell counts) at ticker expand
- Options-implied-move dumbbell chart
- Hedge fund net-flow sparkline (last 4 quarters of 13F deltas)
- Historical earnings surprise scatter (expected vs. actual, last 8 quarters)

**Schema opportunities:**
- `BreadcrumbList`
- `FAQPage` for the How-to-trade-earnings FAQ
- `ItemList` for the earnings table (date, ticker, name)
- `Event` schema per earnings report (name, startDate, organizer) — this is where competitors fail; use `Event` + `FinancialProduct` to try for enhanced SERP treatment
- `HowTo` for the trade-earnings framework
- `Dataset` schema for the full calendar table (bids for Google Dataset Search inclusion)
- `Organization` with sameAs to Smart Score, analyst score, hedge fund methodology pages

**Internal linking strategy:**
- Every ticker row → `/stocks/<TICKER>/earnings` (ticker-specific earnings history page)
- Every ticker → `/stocks/<TICKER>/forecast` (analyst forecast page)
- Sector filter → `/sector/<SECTOR>/earnings`
- "Top analysts covering <TICKER>" → analyst leaderboard page
- "Hedge funds holding <TICKER>" → `/hedge-funds/stock/<TICKER>`
- "Insider trades at <TICKER>" → `/stocks/<TICKER>/insider-trading`
- Smart Score glossary tooltip → Smart Score methodology page (E-E-A-T anchor)
- Comparison modules → `/compare/<TICKER_A>-vs-<TICKER_B>` for the two biggest reporters each day
- Up-funnel: homepage, stock screener, analyst leaderboard
- Down-funnel: dividend calendar, IPO calendar, ex-dividend calendar (sibling pages)

## 4. Differentiation vs. Competitors

### StockAnalysis.com
- **What they do:** Clean, fast earnings calendar table with date, time, EPS estimate, prior EPS, market cap, and a tiny earnings-chart column. Minimalist, loved by power users.
- **Where they're weak:** No proprietary signal layer — purely passive data. No analyst track-record filter, no insider overlay, no hedge-fund context, no "which of these are high-conviction." No account-level personalization (no watchlist overlay).
- **How TipRanks beats them:** Match their speed and density, then add the Conviction Stack (Smart Score + insider + hedge fund + analyst revisions). Keep the minimalist default view, but offer a one-click "Pro view" that layers signals on top. Beat them on freshness: real-time estimate revisions, not daily snapshots.
- **Above the fold at TipRanks:** Day pills, filter rail, primary table with Smart Score dial + Analyst Consensus badge + Insider Buy flag already visible in each row — no clicks to see edge.

### Barchart.com
- **What they do:** Dense, trader-focused earnings calendar with options-implied move, expected move, and a lot of columns. Strong for options traders.
- **Where they're weak:** UI is cluttered and dated; filtering is clunky; mobile UX is poor; no fundamental or sentiment layer beyond analyst estimate; no track-record weighting on analysts; aggressive paywall/upsell interstitials.
- **How TipRanks beats them:** Keep Barchart's options-implied-move data (match or exceed) while adding fundamental conviction (Smart Score, hedge fund flow, insider). Modernize UX: fewer columns by default, drawer expand for depth. Transparent pricing and no mid-session paywall slaps.
- **Above the fold at TipRanks:** Options-implied move vs. historical realized move dumbbell, right next to Smart Score — a view neither competitor offers in one place.

### MarketBeat.com
- **What they do:** Earnings calendar with EPS estimate, revenue estimate, and some analyst context. Heavy on SEO content and email capture.
- **Where they're weak:** Interstitial popups and email-gate everything; stale UI; weak filtering; mostly re-serves consensus data without a proprietary edge; low-quality content modules padded for SEO.
- **How TipRanks beats them:** Lead with proprietary data (Smart Score, analyst track-record accuracy, hedge-fund 13F deltas) that MarketBeat cannot replicate. Strip the popups — show the data first, convert through usefulness. Programmatically generate `/earnings/<TICKER>` pages that outclass MarketBeat's thin per-ticker pages with full forecast + insider + hedge fund + Smart Score history.
- **Above the fold at TipRanks:** Hedge Fund Trend arrow and Insider Buy badge per row — TipRanks' structural moat, invisible to MarketBeat.

**The structural edge:** StockAnalysis has the cleanest UX, Barchart has the deepest options data, MarketBeat has the SEO volume. None has analyst track-record scoring, Smart Score, hedge-fund flow, and insider transactions all in one row. That is TipRanks' only-we-have-this card — play it on every row, every page.

## 5. Conversion Strategy

- Free tier shows Smart Score as a locked 0–10 dial with the number blurred until signed in (one-click signup, no credit card) — creates visible value before conversion ask.
- Smart Score numeric reveal, hedge fund net-flow sparkline, and insider buy badge gate behind free account; options-implied move, 7-day analyst revisions, and whisper number gate behind Premium / Plus.
- Row-level "Unlock full pre-earnings dossier" CTA at the drawer expand, not as a page-level interstitial — intent-aligned, not interruptive.
- Trust elements above the fold: "Data updates every market minute," analyst count tracked, track-record methodology link, press mentions row (Bloomberg, Yahoo Finance, CNBC co-marketing where available).
- Watchlist CTA ("Save <TICKER> to watchlist for earnings alerts") after a user has hovered/expanded 2+ rows — behavior-triggered, not time-triggered.
- Premium upgrade hook: at the top of the Pre-Earnings Insider Buys and Analyst Revisions modules, show the first 3 rows free, blur rows 4–20 with a "See all 47 insider buys" unlock card.
- Email capture via "Earnings Season Daily" — one email at 7:30 AM ET on every reporting day, listing top-5 Smart Score reporters that session. Lower-friction than account signup for first-time visitors.
- Sticky footer bar on mobile: "Markets open in 2h 14m — see today's 12 top-conviction reports" with a free account CTA.

## 6. Editorial Guidance

- Tone: Trader-direct, numbers-first, zero fluff. Short sentences. No "In today's volatile market…" openers.
- Depth: Every claim backed by a data component on the same page. If a module says "insider buys are elevated," the module shows the transactions.
- Freshness: Calendar table auto-refreshes server-side every 60s during market hours; editorial copy around the page (how-to section, FAQ) rewritten every quarter at the start of earnings season (second week of Jan/Apr/Jul/Oct). Date-stamp the page with "Last updated" visible.
- E-E-A-T signals: Byline for the Methodology sections from a named TipRanks data lead with LinkedIn link; link to Smart Score, analyst score, and hedge fund methodology pages from every page in the cluster; cite data provenance (SEC filings, 13Fs, Form 4s, analyst house notes).
- Internal subject-matter authority: Interlink to TipRanks' Analyst Leaderboard and Top-Rated Analysts pages — proves track-record scoring is real, not marketing.
- Avoid: Padded intros, "What is earnings season?" paragraphs at the top (push to end as FAQ for schema), stock tips disguised as neutral commentary, superlatives without supporting numbers.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | High-volume evergreen cluster; recurring seasonal spikes 4x/year; programmatic ticker-level expansion yields thousands of long-tail pages. |
| Business upside | 5 | Earnings season is TipRanks' highest-intent window; traders actively looking for an edge are the ideal premium-conversion cohort. |
| UX complexity | 3 | Table + filter rail + drawer expand is well-trodden territory; Smart Score dial and conviction stack are the design-system challenges. |
| Engineering complexity | 4 | Real-time consensus updates, 13F delta pipeline, insider-transaction classification (filter out tax-withholding sells), options-implied-move feed, and per-ticker programmatic page generation at scale. Watchlist overlay needs auth state. |
| Recommended rollout speed | 5 | Ship core calendar + Smart Score dial + sector/market-cap filter in 2 weeks to catch Q3 2026 season. Insider + hedge-fund + analyst-revision modules in week 3–4. Options-implied-move and programmatic ticker pages in week 5–8. |

**One-line directive to the squad:** Ship a passive earnings calendar in 2 weeks and layer the TipRanks moat on top before Q4 2026 reports in January — do not wait for the full build to launch.
