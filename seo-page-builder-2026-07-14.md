# TipRanks SEO Page Builder — 2026-07-14

**Selected opportunity:** `earnings calendar`
**Why today:** Q2 2026 earnings season officially opens this week (JPMorgan, Wells Fargo, Citi report 7/14–7/15; Goldman, Morgan Stanley, BofA 7/16–7/17). Search demand for "earnings calendar," "earnings this week," and "stocks reporting earnings today" spikes 3–4× above baseline during the first two weeks of a quarterly cycle. This is the highest-intent window of the year to acquire ranking, backlinks, and habitual return visits.

---

## 1. Page Thesis

The TipRanks Earnings Calendar should be the single most decision-useful earnings page on the open web: not just *when* companies report, but *what to do about it* — beat/miss probability, analyst-implied move, options-implied move, Smart Score at report time, insider selling in the trailing 30 days, and hedge-fund positioning delta. It targets active retail traders, dividend-focused investors, and options traders who currently juggle 3–4 sites (Yahoo for the list, Barchart for implied move, MarketBeat for the beat rate, Seeking Alpha for the take). Winning this SERP is a habitual-return keyword — users check it 4–8× per week during earnings season — which compounds brand familiarity and drives conversion into Premium alerts (pre/post-earnings analyst rating changes, insider filings, Smart Score shifts).

## 2. Search Intent Breakdown

- **Primary intent:** "Show me a filterable, dated list of upcoming earnings reports with time-of-day and consensus EPS/revenue."
- **Secondary intent:** "Help me decide whether to hold, hedge, or trade a specific name through its report" — needs analyst confidence, historical surprise rate, implied move, insider signal.
- **What users really want:** A next-24-hours + this-week + next-week view they can trust, with one-click drill-through to each ticker's earnings history and TipRanks Smart Score at report time.
- **What makes them bounce:** Slow loads, stale/incorrect dates (worst offense on this keyword), no BMO/AMC time, list-only pages with no context, aggressive paywall before they see even one row.

## 3. 10x Page Blueprint

**Page type:** Product-led data hub (calendar template) — not a blog. `/earnings-calendar/` at the root with dated sub-URLs `/earnings-calendar/2026-07-14/` and ticker-scoped `/stocks/aapl/earnings/`.

**Title tag (60 chars):** `Earnings Calendar — Consensus, Beat Odds & Implied Move | TipRanks`

**Meta description (155 chars):** `Every company reporting this week with consensus EPS, analyst-implied move, Smart Score, insider activity and hedge-fund flow. Updated in real time.`

**H1:** `Earnings Calendar`

**H2 / H3 outline:**
- H2: Reporting Today (BMO / AMC / During Market split)
  - H3: Confirmed vs. Estimated dates
- H2: This Week's Earnings Highlights
  - H3: Mega-cap reports (>$100B mkt cap)
  - H3: High-conviction names by Smart Score
  - H3: Biggest analyst-implied moves
- H2: Next Week & Upcoming (next 30 days)
- H2: Yesterday's Results — Beats, Misses, Guidance Cuts
- H2: How to Read an Earnings Report on TipRanks
  - H3: What the Smart Score means at earnings
  - H3: Reading implied move vs. historical realized move
- H2: FAQ (schema-eligible)

**Recommended modules:**
- Top-of-page calendar strip (Today / Tomorrow / This Week / Next Week — pill selector, no reload)
- Master data table (default sort: market cap desc among today's reporters)
- "Movers to watch tonight" AMC card (top 5 by implied move × Smart Score)
- Post-close results ticker (auto-refreshes 4:05pm–5:00pm ET during earnings season)
- Portfolio overlay banner: "3 of your holdings report this week" (logged-in users)
- Sector heatmap for the current week

**Interactive components:**
- Column-configurable data table (users pick which of ~18 columns to show, saved to profile)
- Filters: market cap, sector, index membership (S&P 500 / Nasdaq 100 / Russell 2000), confirmed vs. estimated, Smart Score ≥ 7, has insider buying trailing 30d
- Calendar/list toggle
- "Add to my earnings watchlist" per-row (bell icon → free tier gets email morning-of, premium gets real-time push)
- ICS export ("Add to Google Calendar")
- Historical earnings drill-through modal (last 8 quarters: est vs. actual EPS, actual revenue, 1-day % move) without page navigation

**Visual / data components (TipRanks-only above the fold):**
- **Smart Score at report time** column (proprietary, 1–10)
- **Analyst-implied move** (calculated from current consensus PT vs. current price)
- **Historical beat rate** (trailing 8 quarters, ours is more granular than MarketBeat's)
- **Insider net activity trailing 30d** (buying / selling / neutral — clickable to filings)
- **Hedge-fund positioning delta** (last 13F: adds / trims / no change) — this is our moat
- **Analyst confidence trend** (rating upgrades minus downgrades trailing 90d)

**Schema opportunities:**
- `Event` schema per row (Event.name = "AAPL Q3 2026 Earnings Release", startDate, eventStatus)
- `BreadcrumbList`
- `FAQPage` on the H2 FAQ
- `Dataset` schema on the master table (helps for Google Dataset Search + AI Overviews citation)
- Per-ticker sub-page: `FinancialProduct` + `Event` combination

**Internal linking strategy:**
- Row-level: ticker → `/stocks/<ticker>/forecast`, `/stocks/<ticker>/earnings`, `/stocks/<ticker>/insider-trading`
- Sidebar/cross-links: Analyst Ratings hub, Insider Trading hub, Hedge Fund Trades hub, Smart Score explainer, Options Activity (if applicable)
- Contextual anchors in the "How to read" H2 pointing to Smart Score methodology (E-E-A-T signal)
- Outbound to the *sector* earnings landing page (e.g., "Bank earnings this week") — build these as programmatic sub-hubs

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast, minimal earnings calendar with EPS estimates, market cap, time.
- *Weakness:* Data-only — no forward view (implied move, analyst signal, insider signal). Zero personalization. No alerts.
- *How TipRanks beats them:* Layer Smart Score, hedge-fund delta, and analyst-implied move on the same fast table; add per-row bell alerts (their biggest miss for return traffic).

**Barchart.com**
- *What they do:* Deep tables, weekly earnings-calendar PDF, options-implied move column.
- *Weakness:* UI is dense/dated; navigation is dev-only friendly; premium wall is aggressive and appears before any real value shown; no analyst-track-record dimension.
- *How TipRanks beats them:* Modern UI with the same data density behind progressive disclosure; keep the *analyst-implied* move (from our tracked-accuracy analyst PTs) free — differentiated data Barchart cannot replicate.

**MarketBeat.com**
- *What they do:* Earnings calendar with consensus estimates, beat/miss history, and heavy email-list capture.
- *Weakness:* Content-farm feel; ad density; historical beat-rate methodology isn't transparent; no hedge-fund or insider integration on the calendar itself.
- *How TipRanks beats them:* Transparent methodology page for every score; combine beat rate with *analyst-track-record accuracy*; integrate insider + hedge-fund lens directly in the calendar row.

**What TipRanks data goes above the fold (in order):**
1. Ticker + company + BMO/AMC + confirmed/estimated
2. Consensus EPS + revenue
3. **Smart Score** (badge, 1–10, color-coded)
4. **Analyst-implied move %** (from tracked-accuracy analyst PTs)
5. **Insider net 30d** (arrow + $)
6. **Hedge-fund delta last 13F** (arrow + count)
7. Historical beat rate (8Q)

## 5. Conversion Strategy

- **Free tier hook:** Full calendar visible + 1 free "earnings alert" bell per user per week (logged-in, no CC) — turns a browse into an account signup.
- **CTA placement:** Sticky top-right "Get earnings alerts" pill for logged-out; contextual bell in every row post-login; end-of-table "See tomorrow's implied movers" card (soft upsell).
- **Free vs. premium boundary:** Free = calendar, consensus, historical beat rate, one alert. Premium = unlimited real-time alerts, pre-earnings Smart Score changes, live analyst rating changes, options-flow overlay, "AI earnings preview" per ticker.
- **Upgrade hooks:** After 3rd alert set → soft upgrade modal; when user opens a stock the day of its report → "See TipRanks' AI-generated earnings preview" (premium teaser with 1 free preview/week).
- **Trust elements above the fold:** "Data verified by TipRanks — 15+ years of tracked analyst accuracy" + last-updated timestamp + count of analysts/insider filings powering the page.
- **Engagement modules:** Post-close results banner (returns users at 4:05pm ET), morning "who's reporting today" email (free trigger for calendar signup), portfolio overlay if logged in.
- **Habit loop:** Bell alerts + morning email + post-close banner = 3 daily touchpoints during earnings season.
- **Anti-bounce:** Never gate the first row; never modal-interrupt within 15 seconds; keep the calendar's initial paint under 1.2s LCP.

## 6. Editorial Guidance

- **Tone:** Data-first, calm, decision-oriented — not hypey. No "top gainers" clickbait framing.
- **Depth:** Every metric label is a tooltip linking to its methodology page (Smart Score, implied move, beat rate) — required for E-E-A-T.
- **Freshness frequency:** Consensus estimates refreshed every 15 min during market hours; confirmed/estimated report dates refreshed 3×/day; historical results updated within 5 min of a company release. Publish an updated "This week in earnings" preview post every Sunday 6pm ET.
- **E-E-A-T signals:** Named methodology page authors (financial analysts with credentials), transparent data sources (SEC EDGAR for insider, 13F filings for HF, tracked analyst PTs), last-updated timestamp on every module, corrections log.
- **Human-added editorial layer:** One "TipRanks take" paragraph per mega-cap report (AAPL, MSFT, NVDA, etc.) — 100 words, written by a named editor, published morning-of-report. This is the AI-Overview citation bait.
- **Deprecate:** Any 2023–2024 "top earnings stocks to buy" listicles that cannibalize this hub — 301 into the calendar or into per-ticker earnings pages.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Head term with 4× seasonal spike; strong AI Overview surface; Dataset schema opportunity; Barchart/MarketBeat both beatable on UX. |
| Business upside | 5 | Highest-return habit keyword we own; direct feed into Premium alerts; earnings alerts are the #1 stated reason free users upgrade. |
| UX complexity | 4 | Column-configurable table, drill-through modal, sticky filters, saved views, portfolio overlay. Not trivial but a known pattern. |
| Engineering complexity | 4 | Real-time consensus refresh, alert infra (email + push), Event/Dataset schema generation per row, WebSocket-driven post-close ticker, ICS export. Alert infra is the pacing item. |
| Recommended rollout speed | **5 — ship a v1 within 3 weeks to catch Q2 tail + Q3 opener (mid-Oct)** | Phase 1 (3 wk): calendar + Smart Score + analyst-implied move + free bell alert + Event/Dataset schema. Phase 2 (6 wk): insider + hedge-fund columns, drill-through modal, portfolio overlay. Phase 3 (10 wk): AI earnings previews, options-flow overlay. Do not wait for phase 3 to launch — the SEO clock is running. |

---

**Owner recommendations for next 72 hours:**
1. Reserve the URL `/earnings-calendar/` and set up Event + Dataset schema in staging today.
2. Audit and 301 stale earnings listicles this week (Semrush → filter `url_contains:earnings` `pos:11–30`).
3. Ship a v0 "Reporting Today" widget on the TipRanks homepage this week — earn a rank signal from a high-authority page while the full hub is under build.
4. Brief content team on the Sunday-evening weekly-earnings-preview cadence starting 2026-07-19.
