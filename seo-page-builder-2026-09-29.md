# SEO Page Builder — 2026-09-29

**Cluster selected:** Earnings Calendar
**Rationale for today:** Q3 2026 earnings season kicks off in ~10 days (big banks report the week of Oct 12). Search volume for "earnings calendar," "earnings this week," and ticker-specific "when does X report" queries is climbing daily. This is the peak build/refresh window — a superior earnings hub captured now compounds through four earnings weeks and re-ranks stronger every subsequent quarter.

---

## 1. Page Thesis

TipRanks Earnings Calendar is the fastest, most decision-ready earnings hub on the internet — a live, filterable calendar where every scheduled report is instantly enriched with the three things retail traders actually want before a print: **analyst consensus vs. Smart Score**, **hedge fund positioning delta last quarter**, and **insider buying/selling in the 90 days into the print**. It targets active retail traders, options players, and long-term investors who plan trades around earnings weeks. It deserves to rank because competitors show *when* companies report but hide the *edge signals* behind paywalls or omit them entirely. It converts because the free tier gets the calendar hooked, and every "why is this stock a Buy?" click funnels into Smart Score and Premium.

## 2. Search Intent Breakdown

- **Primary intent:** Find a specific company's earnings date OR see what's reporting this week/day (transactional-informational hybrid — user is planning a trade).
- **Secondary intent:** Assess whether an upcoming print is likely to beat, based on analyst revisions, insider activity, and hedge fund flow.
- **What users really want:** A single screen that answers "should I hold, buy, sell, or trade this earnings?" — not just a date and an EPS estimate.
- **What makes them bounce:** Static tables, no filter for market cap / sector / country, EPS estimates without context, gated data on the first row they try to click, and slow-loading calendars that don't remember their timezone.

## 3. 10x Page Blueprint

- **Page type:** Interactive data hub (calendar app) with SEO-optimized daily/weekly sub-pages (`/earnings-calendar/2026-10-13`, `/earnings-calendar/this-week`).
- **Title tag:** `Earnings Calendar 2026 — This Week's Earnings Reports, Estimates & Smart Score | TipRanks`
- **Meta description:** `Live earnings calendar with analyst estimates, Smart Score, hedge fund activity, and insider trades for every reporting company. Filter by sector, market cap, or country. Free.`
- **H1:** `Earnings Calendar — Every Report, Every Signal`
- **H2/H3 outline:**
  - H2: This Week's Biggest Earnings (H3: Mega-cap · Highest expected move · Analyst upgrades into print)
  - H2: Full Calendar (H3: Filters — date, sector, market cap, country, index membership, Smart Score band)
  - H2: Pre-Earnings Signals (H3: Analyst revisions last 30 days · Insider buying/selling · Hedge fund position changes)
  - H2: Historical Beat/Miss Rates by Company
  - H2: Earnings Season Overview (H3: Sector heatmap · Aggregate beat rate · Guidance sentiment)
  - H2: How to Trade Earnings (short, evergreen educational — 300 words, linked to deeper guides)
  - H2: FAQ (When does earnings season start? How reliable are estimates? What is a whisper number? Does Smart Score predict earnings surprises?)
- **Recommended modules:**
  - Live-updating calendar grid (day/week/month toggle, BMO/AMC tags)
  - Per-row inline expansion: Smart Score, analyst consensus, price target, insider trades (90d), hedge fund Δ (last 13F)
  - "Expected Move" column derived from options IV — differentiator vs. everyone
  - Portfolio integration: "3 stocks in your portfolio report this week" (logged-in hook)
  - Watchlist earnings alerts (email + push)
- **Interactive components:** Multi-select filters, savable filter presets, CSV export (Premium), calendar sync (.ics for Google/Apple), sortable columns, sparkline for last 8 quarters beat/miss.
- **Visual/data components:** Sector heatmap of the week, "surprise history" mini-bar chart per row, hedge fund flow chevron (▲ accumulating / ▼ trimming), Smart Score dial.
- **Schema opportunities:** `Event` schema for each earnings date (name, startDate, location=virtual, organizer=company), `FAQPage` schema for the FAQ block, `Dataset` schema for the calendar itself, `BreadcrumbList`, `Organization` for TipRanks.
- **Internal linking strategy:**
  - Every ticker row → individual stock forecast page, analyst ratings page, insider trades page, hedge fund holdings page
  - Sector filter → sector overview pages
  - "How to trade earnings" → TipRanks Academy / options tools
  - Featured cross-links: Smart Score explainer, Top Analyst leaderboard, Earnings Whispers vs. Consensus explainer
  - Calendar → Dividend Calendar, IPO Calendar, Economic Calendar (hub cluster)

## 4. Differentiation vs. Competitors

**StockAnalysis.com** — Clean earnings calendar with EPS estimates and revenue estimates, sortable. **Weak:** No analyst rating context on the row, no insider or hedge fund overlay, no expected-move data, no personalization. **TipRanks beats them by:** Layering Smart Score, analyst consensus & price target, insider 90-day net, and hedge fund 13F Δ into every row, above the fold, with a live "expected move" from options IV.

**Barchart.com** — Deep, professional earnings calendar with options-implied move and pre/post historical price reactions. **Weak:** Cluttered legacy UI, most valuable columns (implied move, whisper) locked behind Barchart Premier, weak on analyst track-record credibility (no per-analyst star ratings). **TipRanks beats them by:** Cleaner mobile-first UI, **Top Analyst-weighted** consensus (not raw average), free Smart Score, and free 90-day insider net — the three things Barchart charges for.

**MarketBeat.com** — Strong SEO on ticker + "earnings date" long-tail queries, decent calendar. **Weak:** Ad-heavy, thin per-row data, no interactive filtering beyond date, editorial content leans generic, no hedge fund overlay. **TipRanks beats them by:** Faster page, real filters, uncluttered UX, and the four proprietary signals (Smart Score, analyst track record, hedge fund activity, insider trades) MarketBeat literally does not have.

**Above the fold on the TipRanks calendar row:** Ticker · Company · Report time (BMO/AMC) · Expected move % · Smart Score · Analyst consensus · Hedge fund Δ · Insider net (90d). No competitor shows all seven.

## 5. Conversion Strategy

- Sticky top CTA during earnings weeks: "Get pre-earnings alerts for your watchlist" → email capture (free) → nurture to Premium.
- Free tier: full calendar + Smart Score visible + top-3 analyst consensus + basic insider net.
- Premium boundary: full analyst list with individual star ratings, complete 13F hedge fund breakdown, options-implied move history, CSV export, unlimited watchlist earnings alerts, pre-market earnings AI summary.
- Inline upgrade hooks on each row: click hedge fund Δ chevron → soft paywall preview → "See all 47 funds holding NVDA (Premium)."
- Trust elements above the fold: "Data trusted by 5M+ investors," "Track record scored on 200,000+ analyst calls," verified S-1/13F/10-Q source labels.
- Engagement modules: user comments/sentiment poll per company ("Will AAPL beat?"), streaks for daily calendar visits, "beat prediction" leaderboard (gamified retention).
- Post-earnings hook: automated "Earnings recap" email 2 hours after each print for logged-in users with the ticker on watchlist — drives daily re-engagement.
- AI feature promo: "Ask TipRanks AI: Is NVDA likely to beat?" button on every row → Premium teaser after 3 free queries/day.

## 6. Editorial Guidance

- Tone: confident, analytical, trader-native. Use terms like "consensus revision," "positioning delta," "implied move" — no hand-holding, but every jargon term links to a one-sentence tooltip.
- Depth: calendar rows are data-dense but scannable; supporting evergreen content ("How to trade earnings," "What is a whisper number?") is 600–900 words with real examples from recent quarters.
- Freshness frequency: calendar refreshes every 15 minutes during market hours; estimates and analyst revisions daily; the `/earnings-calendar/this-week` slug regenerates weekly; historical beat/miss data updated within 30 minutes of each print.
- E-E-A-T signals: byline on all editorial content by named TipRanks analysts with credentials; cite SEC 8-K/10-Q sources on estimate blocks; expose analyst star ratings and lifetime accuracy % on every consensus figure.
- Show data provenance: "Estimates from 34 analysts, weighted by 3-year track record" hover on the consensus number.
- Never publish a rumored/unconfirmed date without a "Confirmed by company" vs. "Estimated based on historical pattern" flag.

## 7. Build Priority

| Dimension | Rating (1–5) | Notes |
|---|---|---|
| SEO upside | 5 | Massive evergreen + 4× annual spike; head term "earnings calendar" plus long-tail "[ticker] earnings date" captures millions of sessions/quarter. |
| Business upside | 5 | Highest-intent audience of any TipRanks page — people planning trades this week convert on Premium at 2–3× baseline. |
| UX complexity | 4 | Live data, filters, per-row expansion, timezone handling, mobile parity — non-trivial but well-scoped. |
| Engineering complexity | 4 | Requires reliable earnings-date feed, options IV integration for implied move, real-time recompute of hedge fund Δ; leverages existing TipRanks data pipes for Smart Score/analyst/insider. |
| Recommended rollout speed | 5 | **Ship v1 within 10 days** to catch Q3 2026 earnings season kickoff (Oct 12 week). v1 = calendar + Smart Score + analyst consensus + insider net + basic filters. v2 (hedge fund Δ, implied move, alerts) within 30 days before mid-earnings-season peak. |
