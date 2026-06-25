---
tags: [dashboard]
last_updated: 2026-06-23
---

# Hold PT Watch — Holds At or Above Their Price Target

> **Why this exists.** Every closed decision to date is a conservative Hold the market overran to the upside (GEV $440, FCEL $18, INTC $120 — see [[Decisions Log]] Lessons #1 and #3). The recurring failure is letting a *static fair-value PT* sit unchallenged on a name with a live catalyst. This note surfaces the next candidates for that error: **Hold-rated names trading within 5% of, or above, their PT.** When a name lands here it needs an explicit decision — reset the PT to a defensible base case, or justify the Hold as an active lean against momentum. It is not a default.

> **Read alongside:** [[Decisions Log]] (Rule 6: scoring a Hold; Lesson #3) · [[Catalyst Playbooks]] (ASML is a ratified PT-reset event) · [[Verification Worklist]] (KLAC/ASML/SMNEY flags).

---

## Live query (frontmatter-driven)

```dataview
TABLE WITHOUT ID
  file.link AS "Name",
  ticker AS "Ticker",
  price_target AS "PT",
  current_price AS "Price",
  round((current_price - price_target) / price_target * 100, 1) AS "% vs PT"
FROM "03_Companies"
WHERE rating = "Hold" AND price_target AND current_price AND current_price >= price_target * 0.95
SORT (current_price - price_target) / price_target DESC
```

> ⚠️ **This query has two blind spots — the static table below is the curated truth:**
> 1. **KLAC won't appear.** Its frontmatter PT is still the **pre-split $1,950** while the price is ~$259, so the ratio reads hugely negative and the filter skips it. In split-adjusted terms (~$244) the stock is *above* PT. Fix the KLAC PT to resolve this.
> 2. **Stale/missing `current_price`.** Frontmatter prices lag the live tape (refreshed Fridays); SMNEY has no `current_price` field at all. Don't trust the query for timing — use it to catch *new* entrants.

---

## Curated snapshot — as of 2026-06-23 closes

| Ticker | Rating | PT | Price (6/23) | vs PT | The decision owed | Gating event |
|---|---|---|---|---|---|---|
| **SNDK** | Hold | $2,000 | ~$2,260 | **+13%** | Reset PT to reflect actual earnings power ($5.95B rev / $3.62B NI per qtr) **or** treat the Hold as a trim signal. Add zone ($1,600–1,800) never triggered. | Q4 FY2026 earnings ~Aug 13 |
| **ASML** | Hold | $1,730 | ~$1,927 | **+11%** | PT is stale below a 52-wk-high price. Ratified as a **PT-reset event** in [[Catalyst Playbooks]] — branches drive an explicit PT decision, not "no action." | Q2 print ~Jul 16 |
| **KLAC** | Hold | $1,950 ⚠️ pre-split | ~$259 | **~+6% vs split-adj.** | Frontmatter PT is pre-split (~8:1). Restate PT to a post-split basis (~$244 prior → above market); resolve Under Review. | Next earnings + 10-K (Verification Worklist #6) |
| **SMNEY** | Hold | $175 | well above | **above** | PT $175 is stale (SMERY P/E ~81x; mkt cap ~$168B). Rebuild on the corrected SE financials. | SE FY2025 annual report (Verification Worklist #8) |
| **ENTG** | Hold | — (under review) | ~$168 | **above last PT $155** | Downgraded Buy→Hold 6/18, PT pulled pending a Q2 model. Build the model and set a real PT. | Q2 filings / model build |
| **TSEM** | Hold | $285 | ~$283 | **−0.8% (at PT)** | Lesson #3 flags this as "the next Hold to test." Decide the lean before it breaks above. | Next earnings |

*Prices: 6/23 official closes per [[Decisions Log]] where available; SNDK from the 6/23 intraday monitor. Treat as approximate.*

---

## How to use this note

1. **At each weekly refresh / quarterly review:** re-run the live query, then reconcile against this table (it catches what the query misses).
2. **When a name lands here:** open a dated [[Decisions Log]] entry. Either (a) reset the PT to a defensible base case and log the methodology, or (b) keep the Hold and write the one-line reason it's an active lean against momentum.
3. **PT resets gated to a print** (ASML Jul 16, SNDK Aug 13) are tracked in [[Catalyst Playbooks]] — clear them there when the event lands.
4. **Retire a row** once its PT is reset or its rating changes.
