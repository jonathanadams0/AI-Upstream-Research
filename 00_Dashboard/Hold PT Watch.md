---
tags: [dashboard]
last_updated: 2026-07-02
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

## Curated snapshot — updated 2026-06-29

| Ticker | Rating | PT | Price (6/29 approx.) | vs PT | Status | Gating event |
|---|---|---|---|---|---|---|
| **SNDK** | Hold | $2,000 | ~$2,335 | **+16.8%** | Gated — no PT change. MU beat Q4 guide by 22%; implied SNDK Q4 EPS ~$38.4 if same beat → upgrade trigger in play (needs EPS ≥$38 + 6th NBM + Q1 FY2027 guide ≥$35). All three required. | Q4 FY2026 earnings Aug 13 |
| **ASML** | Hold | $1,730 ⚠️ stale | ~$1,841 | **+6.4%** | Gated — PT is a ratified reset event in [[Catalyst Playbooks]]. Q2 guidance €8.4–9.0B rev, 51–52% GM. Consensus $10.16B / $7.82 EPS. All branches drive PT action July 15. | Q2 print July 15 |
| **KLAC** | Hold | **$270** ✅ reset 6/29 | ~$259–277 (+7% Jun 29) | **~0–4%** | **PT reset complete.** Split 10:1 (not 8:1) confirmed June 12. Prior $1,950 ÷ 10 = $195 adj.; new PT $270 at 74x FY2026E EPS $3.66. Asym 0.09x → Hold confirmed. Stock may be at/above PT after Jun 29 move. | Next earnings (Q4 FY2026 ~Aug 2026) |
| **SMNEY** | Hold | **$38** ✅ reset 6/29 | ~$34.55 (ENR.F 157 EUR × 0.2 × 1.10) | **+10%** | **PT reset + ADR error corrected.** Prior $175 was 1:1 ADR assumption — actual 1:5 (SEC F-6 confirmed). ENR consensus €196 (~$43 SMNEY); our PT $38 (€173 ENR) conservative pending Annual Report. Asym 0.28x → Hold. | SE Annual Report items (17 in §11 of SMNEY.md) |
| **ENTG** | Hold | — (under review) | ~$176+ | **above last PT $155** | Downgraded Buy→Hold 6/18; exited T4 position 6/25 at $176.28 (+31%). PT Under Review pending Q2 FY2026 model build. Re-entry: confirmed rev growth + PT >$200 + asym ≥1.5x. | Q2 FY2026 filings (late July 2026) |
| **TSEM** | Hold | $285 | ~$283 | **−0.8%** | Watching. Lesson #3 flagged this as the "next Hold to test." Still just below PT. | Next earnings |
| **ON** | Hold | $100 | ~$88.57 | **−11.4%** | Downgraded Buy→Hold 6/29. Synaptics $7B all-stock acquisition: ~12% dilution, EPS accretive only late 2028. PT $160→$100; bear $65. Re-entry: post-close synergy proof or pullback to $70–75. | Synaptics deal close (mid-2027) |

*Prices: official closes or last-known from [[Decisions Log]]; Jun 29 KLAC estimated from +7% Jun 29 move on $258.80 base. Treat as approximate.*

---

## Untracked cohort added 2026-07-02 (full-vault review sweep)

> The 7/2 vault review ([[Vault Review 2026-07-02]]) reconciled the live query against frontmatter across all coverage and found these Holds at/near/above PT that never entered the curated table. Prices are **live intraday 7/2** (broad tape red −1–5%); several were further above PT at the 6/26 close (WDC was +21%, STX +13%). Each needs the Rule-2 decision: reset the PT or log the Hold as an active lean.

| Ticker | Rating | PT | Price (7/2 intraday) | vs PT | Status | Gating event |
|---|---|---|---|---|---|---|
| **FCEL** | Hold | **$26** ✅ reset 7/2 | $28.73 | +10% | **PT reset complete** (was $18, +60% overrun). Hold kept as explicit anti-momentum lean: Fit Energy 30MW firm < 100MW upgrade trigger; revenue still declining; rally was flows+financing. Watch for framework conversion 8-Ks. | ≥100MW firm order (event) / Q3 FY2026 Sep 1 |
| **MKSI** | Hold | **$450** ✅ reset 7/2 | $384.19 | −15% | **PT reset complete** (was $310). 35x NTM ~$12.75; street cluster $453–600. Now below PT — row retires at next refresh. Deep-dive required before Aug 5 print (EBITDA/leverage unverified). | Q2 earnings Aug 5 |
| **SCCO** | Hold | $165 | $173.59 | +5.2% | Entered the band. Low-conviction note. | Q2 earnings Jul 28 |
| **INTC** | Hold | $120 | $124.99 | +4.2% | Decision closed ✗ 6/23; PT never reset after scoring. Reset to a defensible base case or re-log the bearish lean. | Q2 earnings Jul 24 |
| **WDC** | Hold | $560 | $574.00 | +2.5% | Was **+21% above PT** at 6/26 close ($675) — today's pullback is doing the PT's job for it. Thin note (41 lines) in the strongest memory tape on record; deepen before the print. | Q4 FY2026 earnings Jul 31 |
| **CRDO** | Hold | $250 | $254.54 | +1.8% | Entered the band. | Q1 FY2027 earnings Sep 2 |
| **PWR** | Hold | $680 | $687.25 | +1.1% | Entered the band. | Q2 earnings Jul 30 |
| GLW | Hold | $210 | $210.16 | 0% | At PT exactly. | Q2 earnings Jul 24 |
| STX | Hold | $910 | $874.54 | −3.9% | Inside 5% band (was +13% above PT at 6/26 close $1,025). Thin note; same memory-tape caveat as WDC. | Q4 FY2026 earnings Jul 28 |

**Process fix adopted:** the Friday weekly refresh must reconcile the live Dataview query against this curated table — new entrants get a row the same day. This cohort sat invisible for up to two weeks because that reconciliation step wasn't explicit.

---

## How to use this note

1. **At each weekly refresh / quarterly review:** re-run the live query, then reconcile against this table (it catches what the query misses).
2. **When a name lands here:** open a dated [[Decisions Log]] entry. Either (a) reset the PT to a defensible base case and log the methodology, or (b) keep the Hold and write the one-line reason it's an active lean against momentum.
3. **PT resets gated to a print** (ASML Jul 16, SNDK Aug 13) are tracked in [[Catalyst Playbooks]] — clear them there when the event lands.
4. **Retire a row** once its PT is reset or its rating changes.
