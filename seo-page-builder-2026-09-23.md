# TipRanks SEO Page Builder — 2026-09-23

**Selected opportunity cluster:** `earnings calendar`
**Why today:** Q3 2026 earnings season begins in ~3 weeks (banks lead the week of Oct 12). "Earnings calendar," "who reports this week," and ticker-level "when does X report earnings" queries spike now and hold elevated volume through mid-November. This is a recurring, high-intent hub with clear conversion paths into portfolio, alerts, and premium.

---

## 1. Page Thesis

The Earnings Calendar hub is TipRanks' evergreen booking system for the market's most predictable volatility event. It serves active traders, options players, and long-term shareholders who need to know *when* a company reports and — uniquely — *what smart money, analysts, and insiders are doing into the print*. It deserves to rank because it fuses four proprietary datasets (analyst track-record accuracy, Smart Score, hedge fund 13F deltas, insider transactions) onto a single date-driven surface competitors treat as a flat table. It converts because every row is a live pre-earnings decision that begs for alerts, watchlists, and Premium-gated confidence signals.

## 2. Search Intent Breakdown

- **Primary intent:** "Show me a filterable list of companies reporting on X date/week" — transactional-informational, dominated by traders scoping the week ahead.
- **Secondary intent:** Ticker-level "when does AAPL report earnings" + "what analysts expect" — pulls a large long-tail cluster into the hub via child pages.
- **What users really want:** An edge — not just the date. They want EPS estimates, beat/miss history, options-implied moves, analyst revisions, hedge fund positioning, and post-earnings drift patterns *before* the print.
- **What makes them bounce:** Stale dates (worst offense), unconfirmed vs. confirmed dates unlabeled, missing pre-market/after-hours timing, no filtering by market cap/sector/index, and login walls on the calendar itself.

## 3. 10x Page Blueprint

- **Page type:** Product-led data hub (parent) → per-day and per-ticker earnings pages (children). Not a blog.
- **Title tag:** `Earnings Calendar 2026 — Analyst Estimates, Smart Score & Hedge Fund Moves | TipRanks`
- **Meta description:** `Live earnings calendar with confirmed report dates, EPS & revenue estimates, analyst accuracy scores, Smart Score, insider trades, and hedge fund positioning. Filter by week, sector, market cap, or index.`
- **H1:** `Earnings Calendar`
- **H2/H3 outline:**
  - H2: This Week's Earnings Highlights (auto-curated: top-5 by market cap + top-5 by pre-earnings analyst revisions)
    - H3: Most-Watched Reports This Week
    - H3: Biggest Analyst Upgrades/Downgrades Into Earnings
    - H3: Notable Insider & Hedge Fund Activity Into Earnings
  - H2: Full Earnings Calendar (interactive table — the core module)
  - H2: Earnings by Date (Today / Tomorrow / This Week / Next Week / By Month)
  - H2: Earnings by Sector & Index (S&P 500, Nasdaq-100, Russell 2000, sector splits)
  - H2: Earnings Movers & Post-Earnings Drift Tracker
  - H2: How to Read an Earnings Report with TipRanks Data
  - H2: FAQ (schema-eligible: BMO vs. AMC, confirmed vs. estimated, whisper number, why dates change)
- **Recommended modules:**
  1. Interactive calendar table (default view: this week, BMO/AMC split, sortable columns).
  2. "Smart Money Into Earnings" panel — hedge fund 13F delta + insider buy/sell in the last 90 days per ticker.
  3. Analyst Consensus & Accuracy strip — consensus EPS/rev, but weighted by analyst track-record score (unique TipRanks data).
  4. Post-earnings drift heatmap — 1-day, 5-day, 30-day median return after last 8 prints.
  5. Options-implied move (Premium gate).
  6. AI Earnings Preview — TipRanks AI synthesis of the sell-side notes, guidance history, and management tone (Premium teaser + full behind gate).
  7. Alert bar — "Get notified before [Ticker] reports" (email + push, free trigger).
- **Interactive components:**
  - Filters: date range, index membership, sector, market cap, exchange, Smart Score ≥8, has-buy-rating consensus, has-recent-hedge-fund-buying.
  - Column toggles: reveal Smart Score, analyst accuracy, hedge fund delta, insider net, options-implied move.
  - "Add to My Calendar" (Google/Outlook .ics export) — sticky feature that competitors don't nail.
  - Pin-to-watchlist inline action on every row (auth-gated but low-friction).
- **Visual/data components:**
  - Sparkline of last 8-quarter beat/miss vs. estimates in each row.
  - Color-coded Smart Score chip.
  - Miniature analyst consensus donut (Buy/Hold/Sell).
  - Sector heatmap for the current week.
- **Schema opportunities:**
  - `Event` schema per confirmed earnings date (EarningsEvent variant).
  - `FinancialProduct`/`Corporation` schema per ticker child page.
  - `FAQPage` for the FAQ section.
  - `BreadcrumbList` (Home > Stocks > Earnings Calendar > [Week] > [Ticker]).
  - `ItemList` for the weekly table.
- **Internal linking strategy:**
  - Every row deep-links to the ticker's Earnings tab, Smart Score page, Hedge Fund holders page, Insider Trades page, and Analyst Forecast page.
  - Hub links out to Stock Screener (pre-filtered "Reporting this week + Smart Score ≥8"), Analyst Ratings hub, Insider Trading hub, and Hedge Fund Holdings hub.
  - Child ticker earnings pages link back to the calendar week they belong to (breadcrumb + "See other reports this week").
  - Editorial "Earnings Preview" articles link into their ticker's calendar row and vice versa.

## 4. Differentiation vs. Competitors

**StockAnalysis.com**
- *What they do:* Clean, fast earnings calendar with EPS estimates, market cap, sector filter, and a simple confirmed/estimated flag.
- *Where they're weak:* No analyst-quality weighting, no hedge fund/insider overlay, no post-earnings drift data, no alerting, thin child pages, no AI preview.
- *How TipRanks beats them:* Fuse analyst accuracy + Smart Score + smart-money overlay into the same row. Where StockAnalysis shows "consensus EPS $2.14," TipRanks shows "$2.14 (based on 24 analysts; top-quartile analysts weighted $2.19)."
- *Above the fold:* Track-record-weighted consensus, Smart Score chip, and a "Smart Money into this print" pill (net insider $ + hedge fund delta) — none of which StockAnalysis has.

**Barchart.com**
- *What they do:* Deep data density — implied volatility, options activity, technicals — attached to earnings dates. Traders love the raw data.
- *Where they're weak:* Cluttered UX, paywall gates a lot of the useful columns, no fundamental narrative, no analyst reputation layer, weak mobile experience.
- *How TipRanks beats them:* Match Barchart's data ambition but with cleaner defaults and a fundamental+sentiment layer they lack. Free tier shows more decision-useful signal (analyst accuracy, Smart Score, insider net) than Barchart's free tier.
- *Above the fold:* Options-implied move *paired* with track-record-weighted analyst target — the trader-plus-fundamentals combo Barchart never presents together.

**MarketBeat.com**
- *What they do:* Broad calendar with strong SEO on ticker-level "when does X report" pages; heavy on aggregated news snippets.
- *Where they're weak:* Ad-heavy, low data density per row, no proprietary signal, no meaningful smart-money layer, generic content.
- *How TipRanks beats them:* Own the "smart money into earnings" narrative MarketBeat can't manufacture (they have no 13F pipeline, no analyst track-record scoring). Cleaner UX and faster loads.
- *Above the fold:* Hedge Fund 13F delta (last quarter) + Insider net-buy in last 90 days per row — a data column MarketBeat literally cannot produce.

## 5. Conversion Strategy

- **Free-tier hooks (above the fold):** Confirmed date, BMO/AMC, consensus EPS/rev, Smart Score chip, analyst consensus donut — enough signal to build trust.
- **Premium boundary:** Track-record-weighted consensus, options-implied move, AI Earnings Preview, post-earnings drift history beyond last 2 quarters, hedge fund 13F delta beyond top-line count.
- **Contextual upgrade hook:** On row hover/expand, show a locked "Top-analyst weighted estimate: $X.XX" with a one-click Premium trial CTA — offer is *specific* to the row the user is already researching.
- **Alert CTA (free, auth-gated):** "Notify me before [Ticker] reports" — captures email + creates account, funneling into portfolio.
- **Watchlist CTA:** Every row has a one-click "Add to My Earnings Watchlist" — becomes the retention loop (weekly digest email of upcoming reports on their list).
- **Trust elements:** "Data updated [timestamp]," source badges (company IR, consensus provider), analyst track-record links, methodology tooltip on Smart Score, and a visible "confirmed by company" vs. "estimated" flag on every date.
- **Engagement modules:** Post-earnings recap emails to users who watched a ticker into its print — high open-rate, low-cost re-engagement.
- **Portfolio tie-in:** If the user has a portfolio, surface "3 of your holdings report this week" banner above the calendar — the strongest single conversion pull we can build.

## 6. Editorial Guidance

- **Tone:** Analyst-grade, plainspoken, decision-oriented. No hype, no clickbait. Traders and long-term investors both need to feel it's built for their workflow.
- **Depth:** The hub is data-first; editorial lives in child previews and post-earnings recaps. Each preview is 400–600 words, structured (setup → estimates → smart money → risk).
- **Freshness frequency:** Calendar table refreshes intraday for confirmed dates and consensus revisions. Child previews written 3–5 days ahead of print; recaps within 90 minutes of report.
- **E-E-A-T signals:** Bylined analyst previews with credentials and track-record links; methodology page for Smart Score and analyst accuracy; visible "last verified" timestamps; company IR source citations.
- **Consistency:** Use the same table schema and column naming across hub, child, and ticker Earnings tabs — the interface should feel like one product, not three.
- **Recap loop:** Every recap links back to its own preview and to the ticker's next scheduled report — closes the editorial-to-data flywheel.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Massive recurring-intent cluster; parent hub + hundreds of child pages; seasonal traffic peaks every quarter. Existing competitor pages are beatable on data depth. |
| Business upside | 5 | Every pre-earnings decision maps to a Premium hook (implied move, weighted consensus, AI preview); strong alert/watchlist capture funnel; portfolio tie-in is the single best cross-sell trigger we have. |
| UX complexity | 4 | The table is complex — filters, column toggles, inline actions, mobile parity, alert flow, .ics export. Needs a real design pass, not a reskin. |
| Engineering complexity | 4 | Data plumbing is the real cost: confirmed/estimated date normalization, track-record-weighted consensus computation, 13F delta joins per ticker, options-implied move feed, scheduled cache invalidation on IR updates. Reuse existing analyst/hedge fund/insider pipelines where possible. |
| Recommended rollout speed | 5 | Ship the hub + this-week/next-week views + top-100 ticker child pages before Oct 12 (bank earnings kickoff). Follow with sector/index cuts and full ticker coverage by Oct 20. AI Earnings Preview can gate behind a Phase 2 flag if the model isn't production-ready. |

---

**Rollout note:** Because Q3 earnings starts mid-October, the SEO window to earn rankings for "earnings calendar this week" is closing. Ship a minimum-viable hub + top-100 child pages by Oct 5, then iterate.
