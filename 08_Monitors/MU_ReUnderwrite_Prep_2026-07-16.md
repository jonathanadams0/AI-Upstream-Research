---
date: 2026-07-16
ticker: MU
type: reunderwrite_prep
status: STAGED — fires only on close <$900
protocol_source: Decisions Log 2026-07-07 ("Bear-case touch — re-underwrite protocol armed")
prior_reunderwrite: 2026-07-07 (MU.md §6 — Buy→Hold, PT $1,500→$1,200, bear $900→$800)
tags: [monitor, reunderwrite, MU]
---

# MU Re-underwrite Prep — Staged for 2026-07-16 Close

> **Gate: this checklist executes ONLY if MU's official close (FMP settled quote, 16:00 ET) is below $900.** Intraday breach does not fire it (7/15 precedent: dayLow $873.63, close $904.28 → NOT FIRED). At 10:28 CDT MU is $862.83 — $37 below the floor.

## Step 0 — Close verification

- [ ] Official close: $______ (confirm settled quote + market closed)
- [ ] If ≥$900: log a close-check note (NOT FIRED, 4th consecutive session inside 4% of trigger), stop here
- [ ] If <$900: protocol FIRES — schedule full re-underwrite next session, complete steps 1–5

## Step 1 — Anchor to fundamentals, not the tape (per 7/7 pre-commitment)

The protocol explicitly requires anchoring to HBM fundamentals. Nearest hard datapoint: **SK Hynix Q2 print, July 24.** If the re-underwrite runs before then, mark conclusions provisional pending that print.

## Step 2 — Original bear-thesis triggers (all must be re-checked, none fired as of 7/16 AM)

| Trigger | Test | Status 7/16 AM |
|---|---|---|
| 2 sequential GM declines | Q3 84.9% → Q4 guide ~86%; need two down quarters | Not fired (next datapoint: Q4 FY26 print ~Sept 25) |
| HBM4 slip | Ramp 2x faster than HBM3E; >$1B shipped | Not fired |
| China restriction | 8-K disclosing new restriction | Not fired — **CXMT $8.6B IPO is competitive supply pressure, NOT a restriction. Do not conflate.** |

## Step 3 — What's new since the 7/7 re-underwrite (evaluate each)

1. **CXMT $8.6B STAR Market IPO, lists July 27** — funds Chinese DRAM capacity expansion. Directly feeds the supply-overshoot leg of the $800 bear scenario (which assumed SK Hynix/Samsung ASP pressure; add CXMT). Question: does state-funded Chinese capacity pull the H1 FY2027 down-cycle scenario forward?
2. **TSMC Q2 (7/16)** — beat, record profit; selloff is expectations-reset, not demand deterioration. Neutral-to-positive for AI-memory demand.
3. **Qualcomm/Harman automotive supply agreements (7/16)** — constructive, small vs data center mix.
4. **SK Hynix ADR unwind + HBM4-weakness chatter (7/15)** — assess against actual Jul 24 print, not headlines.
5. **Barron's "3 Reasons Micron Keeps Falling" (7/16)** — read, log arguments vs bear case.

## Step 4 — Decision framework

- Bear $800 = ~$114 NTM EPS × 7x (two-triggers-fired scenario). Test: has evidence moved probability of that scenario materially since 7/7?
- **Do-not-add stands regardless of outcome** (7/7: "no new capital ... regardless of intraday pullbacks").
- **No autonomous rating change** — outcomes are: (a) reaffirm Hold/$1,200/$800; (b) flag PT or bear revision for Jonathan's ratification; (c) escalate if a trigger has actually fired.
- Re-upgrade checkpoint remains Q4 FY2026 (~Sept 25): revenue ≥$49B, GM ≥85%, no China restriction.

## Step 5 — Paper trail

- [ ] Decisions Log entry (update the Open 7/7 protocol row — fired/not fired, disposition)
- [ ] MU.md changelog entry + `last_updated`
- [ ] If provisional: calendar the July 24 SK Hynix print as the completion datapoint

---

*Prices and bear-case distances only — no position data included.*
