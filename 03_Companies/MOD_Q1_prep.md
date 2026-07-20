# MOD Q1 FY2027 Earnings Prep
**Date:** 2026-07-20 | **Expected report:** ~2026-07-29 (per frontmatter) — **Bigdata.com tearsheet confirms 2026-07-30** (Q1 2027 earnings call); 1-day discrepancy, flagged below.

> **Fiscal quarter note:** Modine's fiscal year runs April–March, so the quarter reporting in late July 2026 (covering Apr–Jun 2026) is **Q1 FY2027**, not calendar Q2 — confirmed via Bigdata.com's `earnings_calendar` (title "Q1 2027"). MOD.md's own catalyst language ("Watch FY2026 Q1 print closely") is stale/ambiguous on this point; the confirmed label is used here.

---

## Setup

| Item | Value |
|---|---|
| Rating / PT | Buy / $355 |
| Current price | $229.20 |
| Conviction | High |
| Thesis (one-line) | Modine is one of the few publicly traded pure-plays on data center thermal management at scale, with a purpose-built cooling segment growing into AI hyperscaler demand while its legacy climate & HVAC businesses fund the transition and compress perceived risk. |

---

## Invalidation Trigger

**Thesis Invalidation Tracker row (`00_Dashboard/Portfolio Summary.md`):** "Sell Trigger: Data center revenue growth decelerates below 20% YoY for 2 quarters | Monitor Via: Quarterly segment revenue." (Last checked 2026-06-04.)

**What in this print would fire it — and which confirming quarter this would be:** The most recent data center segment growth figures recorded in the vault are **+218% YoY** (Portfolio Summary Model Portfolio table, row 14, as of 2026-06-04) and **+225% YoY** (MOD.md §Valuation "Key Metric"). Both are far above the 20% threshold, and no prior quarter in the vault shows growth below 20%. **This means if Q1 FY2027 data center revenue growth prints below 20% YoY, it would be the FIRST of the two required consecutive confirming quarters — not sufficient on its own to fire the sell trigger, but a major escalation that would require flagging watch status ahead of the next print** (per the 2-quarter design of this trigger).

---

## 3 Questions This Print Must Answer

1. **Does management provide a quantified data center segment revenue/backlog disclosure**, and does the YoY growth rate stay comfortably above 20% — MOD.md §8 Catalysts specifically flags this as the top near-term catalyst ("Quarterly earnings with data center segment disclosure... Watch [Q1] print closely")?
2. **Is there any single-customer concentration disclosure showing one customer >40% of revenue with an order reduction** (Bear Case §10 Trigger #2)?
3. **Does management raise FY2027 EBITDA margin guidance** (Catalysts §8, would confirm the mix-shift thesis) **or finally disclose the exact PT (Performance Technologies) vs. CIS segment revenue split**, which remains an open [VERIFY] item throughout §4 Business Overview and §7 Valuation?

---

## Consensus Expectations

**Confirmed report date (Bigdata.com tearsheet, retrieved 2026-07-20):** 2026-07-30 (Q1 2027 earnings call) — **differs from frontmatter `next_earnings` (2026-07-29) by 1 day.** Flagging for correction; not edited here per task constraints.

**Consensus (pull from terminal):** not retrievable via available tools as of this run for the Q1 FY2027 print itself. Bigdata.com's `analyst_estimates` feed (rp_entity_id E114F4) has no record for the quarter ending ~June 2026 — its earliest available record is labeled FY2026 fiscal period 3 (period ending 2026-09-30: mean revenue ~$964.6M, mean EPS ~$1.76, 6 analysts), which appears to correspond to the quarter *after* this print.

No management guidance for this specific quarter is quoted in MOD.md (its Valuation section is explicitly marked "SCREENING MODE — placeholder"), so no substitute figure is available either.

---

## Playbook Check

No existing Catalyst Playbooks entry for MOD. Since it's Buy-rated, the following is a **drafted** playbook-style outcome table based on MOD.md's Thesis, Bear Case, and Catalysts sections — all numeric thresholds are DRAFT and unratified:

| Outcome | Read | Action (DRAFT) |
|---|---|---|
| DC segment revenue growth **DRAFT: ≥50% YoY** + margin guidance raised | Bull case intact; mix-shift accelerating ahead of plan | DRAFT: Reiterate Buy; consider moving PT toward the $450 bull scenario in MOD.md §Valuation |
| DC segment revenue growth **DRAFT: 20–50% YoY**, EBITDA margin roughly stable (~13–15%) | In-line; thesis intact, deceleration from the +218–225% run-rate but still well clear of the trigger | DRAFT: Confirm PT $355; no action |
| DC segment revenue growth **DRAFT: <20% YoY** | First leg of the 2-quarter sell trigger firing (see Invalidation Trigger above) | DRAFT: Do not downgrade yet; elevate to watch status; hard checkpoint at next print — a second sub-20% quarter fires the sell trigger |
| Single customer disclosed **DRAFT: >40%** of revenue with an order reduction | Concentration risk materializing (Bear Case Trigger #2) | DRAFT: Re-underwrite immediately |

---

## Data Sources

- `03_Companies/MOD.md` (frontmatter; §2 Thesis; §7 Valuation; §8 Catalysts; §10 Bear Case)
- `00_Dashboard/Portfolio Summary.md` (Thesis Invalidation Tracker row; Model Portfolio table row 14)
- Bigdata.com company tearsheet (rp_entity_id E114F4), sections `analyst_estimates` + `earnings_calendar`, retrieved 2026-07-20

---

**Powered by [Bigdata.com](https://bigdata.com)**

*For informational purposes only. Not investment advice.*
