# SEO Page Builder — Earnings Calendar

**Date:** 2026-07-13
**Cluster:** Earnings Calendar (`earnings calendar`, `earnings this week`, `earnings today`, `after hours earnings`, `pre market earnings`, `AAPL earnings date`, `Q2 earnings calendar`)
**Why today:** Q2 2026 earnings season opens this week — the four largest US banks (JPM, WFC, C, BAC) report Mon–Wed, followed by GS, MS, and NFLX. Search interest for "earnings calendar" and "earnings this week" spikes 3–4× above baseline for the next 6 weeks. Building the hub now captures the entire season's compounding demand and re-ranks four more times per year on evergreen momentum.

---

## 1. Page Thesis

The TipRanks Earnings Calendar is a **live, filterable, forecast-aware event hub** that answers three questions in one screen: *who reports today/this week*, *what does Wall Street expect*, and *what happened the last time they reported*. It serves active retail investors and swing traders who make position decisions on a 24–72 hour horizon around earnings prints. It deserves to rank because it fuses three assets no competitor combines above the fold — analyst consensus with **track-record-weighted accuracy scores**, Smart Score at time of report, and last-quarter EPS surprise history. It converts because every row is a doorway into a per-ticker earnings page whose paywalled surface (analyst-accuracy-weighted forecast, insider trades in the 30 days prior, hedge fund positioning delta) is exactly what a trader needs before the bell.

## 2. Search Intent Breakdown

- **Primary:** transactional — "what reports today/this week, at what time, what's the consensus" → the user wants a scannable table right now.
- **Secondary:** research — "history of beats/misses, expected move, post-earnings drift" → power users filtering by market cap, sector, confirmed vs. unconfirmed.
- **What users really want:** an edge — which reports are *actually* worth trading, not just a chronological list. Whose analysts have been right? Are insiders buying into the print?
- **What makes them bounce:** cramped tables, no pre-market vs. after-hours split, static "consensus EPS" with no context on analyst accuracy, forced login before seeing a single row, no way to set an alert.

## 3. 10x Page Blueprint

**Page type:** Product-led data hub (calendar template) with programmatic sub-pages per date, week, sector, and ticker.

**Title tag:** `Earnings Calendar 2026 — This Week's Reports, Consensus & Track Record | TipRanks`

**Meta description:** `Live earnings calendar with EPS/revenue estimates weighted by analyst track record, Smart Score at report date, insider trades, and historical surprise. Filter by date, sector, market cap.`

**H1:** `Earnings Calendar — Track Every Report With Analyst Accuracy Scores`

**H2 / H3 outline:**
- H2 *This Week's Earnings (Jul 13–17, 2026)* — pinned sticky filter bar
  - H3 Monday · Tuesday · Wednesday · Thursday · Friday tabs
  - H3 Pre-Market · After-Hours · During Session toggles
- H2 *Today's Confirmed Reports* — hero table
- H2 *Highest-Impact Reports This Week* — Smart-Score-ranked top 10
- H2 *Beat History Leaders* — tickers with ≥8 consecutive beats
- H2 *What the Top-Rated Analysts Expect* — track-record-weighted consensus block
- H2 *Insider & Hedge Fund Activity Ahead of Earnings*
- H2 *How to Read an Earnings Report* — evergreen explainer (short, linkable)
- H2 *Upcoming Weeks* — next 4 weeks, links to `/earnings-calendar/week-of-YYYY-MM-DD`
- H2 *Earnings Calendar FAQ*

**Recommended modules:**
1. Sticky filter bar (date range, market cap, sector, index membership, confirmed-only, expected-move ≥ X%).
2. Live "reports in next 60 min" ticker strip during market hours.
3. Row-level Smart Score badge + track-record-weighted EPS estimate + last-4-quarter surprise sparkline.
4. Hover card on any ticker: last print reaction (1-day %, 5-day drift), top analyst most recent take.
5. Free vs. Premium toggle showing what upgrading unlocks (dim rows, don't hide them).
6. Sector heat strip: aggregate beat rate this week by GICS sector.
7. Post-earnings recap module that back-fills after the print with the actual number vs. consensus vs. TipRanks-weighted consensus (proves the weighting works — this is the moat).

**Interactive components:**
- Column sort on every metric (expected move, consensus EPS, Smart Score, analyst accuracy).
- Watchlist add-from-row (one click).
- Email/push alert for "notify me the morning of AAPL's report."
- CSV export (premium).
- ICS calendar subscription URL, per-user, personalized to their watchlist.

**Visual/data components:**
- Consensus vs. TipRanks weighted-consensus delta chip on every row (green when weighted > street, red when below) — instantly readable edge.
- 4-quarter surprise sparkline inline.
- Analyst-accuracy dial (0–100) beside consensus EPS.
- Sector heat strip (12 GICS blocks) at top.
- Implied-move gauge from options.

**Schema opportunities:**
- `Event` schema per ticker+date (name, startDate, organizer=company, eventStatus).
- `FinancialProduct` on ticker rows.
- `FAQPage` on the FAQ block.
- `BreadcrumbList` for `/earnings-calendar` → `/earnings-calendar/2026-07-14` → `/earnings-calendar/AAPL/2026-07-31`.
- `ItemList` on the hero table.
- `Dataset` on the historical surprise data.

**Internal linking strategy:**
- Every ticker row → its `/stocks/<ticker>/earnings` page.
- Every sector chip → `/earnings-calendar/sector/<sector>`.
- Hub → dividend calendar, IPO calendar, economic calendar (sibling event hubs; cross-link with contextual anchor text, not a generic footer).
- Post-earnings recap rows → the ticker's forecast page and Smart Score page.
- Every top-analyst mention → their `/experts/analysts/<slug>` profile page (drives topical authority for analyst pages simultaneously).

## 4. Differentiation vs. Competitors

### StockAnalysis.com — `/earnings-calendar/`
- **What they do:** Clean, fast, minimalist table — date, ticker, EPS estimate, revenue estimate, time.
- **Where they're weak:** No analyst-track-record weighting. No Smart Score. No expected-move column. No historical beat/miss context on the row. No sector/market-cap filters visible above the fold. No alerting. Consensus is just an average — dumb weighting.
- **How TipRanks beats them:** Same clean scannability, but each row carries the *edge layer* — weighted consensus, accuracy dial, surprise sparkline, insider chip. We answer "should I care?" not just "when is it?"
- **Above the fold:** track-record-weighted consensus delta chip + 4-quarter surprise sparkline on every row.

### Barchart.com — `/stocks/earnings/`
- **What they do:** Dense, feature-rich table with EPS, revenue, whisper number, time, market cap. Options-oriented users.
- **Where they're weak:** Overwhelming UI, aggressive interstitials and login walls, weak sector filtering, no analyst credibility layer, whisper number without a stated methodology, poor mobile.
- **How TipRanks beats them:** Match the data density where it matters (implied move, whisper-equivalent = TipRanks weighted consensus with a *disclosed* methodology), but with modern UX, no interstitial, mobile-first, and a credibility story ("weighted by analyst track record" is a defensible whisper substitute).
- **Above the fold:** implied-move gauge from options + TipRanks weighted consensus, labeled with methodology tooltip.

### MarketBeat.com — `/earnings/`
- **What they do:** Long-form, SEO-heavy pages per ticker earnings event with lots of contextual text; strong on ranking for `AAPL earnings date` long-tail queries.
- **Where they're weak:** Interstitials and email-gate walls, thin data density on the hub itself, consensus quality is basic, no proprietary composite, weak filtering, ad-heavy layout.
- **How TipRanks beats them:** Beat them at their own long-tail game — programmatic per-ticker earnings pages powered by Smart Score, analyst-track-record consensus, insider window, hedge fund delta, and last-print reaction. Kill the interstitial pattern; free surface is generous, premium is clearly worth it.
- **Above the fold:** Smart Score badge + hedge fund delta chip on the per-ticker earnings page, contextual paragraph auto-generated from live data (matches MarketBeat's content depth without their staleness).

## 5. Conversion Strategy

- **Free tier surface (must be generous):** current week's calendar, consensus EPS/rev, expected move, last quarter beat/miss, 3 rows of top-analyst consensus per ticker. Enough to be the reference nobody else needs.
- **Premium boundary:** track-record-weighted consensus *number* (not just the direction chip), full analyst list with accuracy scores, insider trade detail in the 30-day window, hedge fund positioning delta, CSV export, watchlist alerts >5 tickers.
- **Primary CTA placement:** inline "Unlock weighted consensus" chip on every row (contextual, not sidebar), plus a soft sticky footer bar during market hours only.
- **Upgrade hook #1 — proof, then paywall:** post-earnings recap module publicly shows the historical accuracy of TipRanks weighted consensus vs. street on past reports. Then paywall the *forward* number. Users buy the future because they saw the past worked.
- **Upgrade hook #2 — alerts:** free users get 3 earnings alerts, premium gets unlimited + pre-market prep email 60 min before open on report days.
- **Trust elements:** methodology tooltip on every proprietary metric; analyst accuracy scores link to that analyst's full track record; "Last updated: 30 sec ago" timestamp; source attribution for every EPS estimate.
- **Engagement modules:** save filter presets, ICS calendar subscription (sticky habit — the URL keeps refreshing forever), one-click add all this week's mega-caps to a watchlist.
- **Post-print re-engagement:** if a logged-in free user viewed a ticker pre-earnings, email them the recap the morning after with a "see what the top analysts are saying now" CTA into the paywalled updated forecast.

## 6. Editorial Guidance

- **Tone:** analytical, neutral, second-person where appropriate ("here's what to watch"). Never breathless.
- **Depth:** the hub itself is data-first with a short evergreen explainer at the bottom (400–600 words on how to read earnings). Per-ticker earnings pages get an auto-generated 200-word context paragraph refreshed hourly.
- **Freshness cadence:** data every 30 seconds during market hours; editorial "Earnings Week Preview" published every Sunday evening and internally linked from the hub; per-ticker page regenerated within 5 min of print.
- **E-E-A-T signals:** byline preview posts to TipRanks analyst team with credentials; methodology page linked from every proprietary metric; disclose data provider and update cadence; every analyst named is a real, verifiable person with a track record page; SEC-filing citations on insider/hedge fund modules.
- **Quality bar:** if the weighted consensus is unavailable or the number of covering analysts is <3, show a clearly labeled "insufficient coverage" state rather than a misleading average.
- **Evergreen assets:** "How to read an earnings report," "What is EPS surprise," "Pre-market vs. after-hours earnings" — each 600–900 words, internally linked from the hub, targeting supporting long-tail queries without diluting the hub itself.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Head term with 4× seasonal spikes, huge long-tail (`<TICKER> earnings date` × 8,000 tickers), event schema competitive advantage, minimal quality competition on the weighted-consensus angle. |
| Business upside | 5 | Highest-intent moment in the retail investor lifecycle — pre-earnings research maps directly to premium features (analyst accuracy, insider window, hedge fund delta). Alerts create sticky habit → retention. |
| UX complexity | 3 | Table + filters + hover cards is well-trodden; the novelty is the weighted-consensus chip and post-print recap loop, both isolated components. |
| Engineering complexity | 4 | Live data at 30s cadence, analyst-weighting job, per-ticker page generation at scale, ICS feed per user, alert pipeline, post-print recap back-fill job. Real infra, but reuses existing analyst-accuracy pipeline. |
| Recommended rollout speed | 5 | Ship the hub + top 500 tickers' per-earnings pages before Aug 1 to capture Q2 tail (biotech/retail report late July–mid Aug). Programmatic long-tail and alerts in a fast-follow within 3 weeks. Don't wait for Q3 — the compounding starts now. |
