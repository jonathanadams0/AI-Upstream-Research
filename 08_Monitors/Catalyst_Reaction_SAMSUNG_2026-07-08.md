---
date: 2026-07-08
catalyst: Samsung Q2 2026 Preliminary Flash
playbook_section: "§3 — Samsung Q2 Full Earnings (pre-event note)"
event_type: macro_input
direct_position: false
affected_names: [LRCX, AMAT, ASML, MU, ENTG]
status: pre-signal_only  # Full capex decision table fires at Jul 30–31 full report
generated_by: catalyst-execution loop
---

# Catalyst Reaction — Samsung Q2 Preliminary Flash

**Date resolved:** July 7, 2026 (KST evening / US Tuesday morning)
**Playbook ref:** §3 Samsung Q2 Full Earnings — pre-event note (flash monitoring)
**Next gate:** Samsung Q2 Full Report with capex guidance — ~July 30–31

---

## Actual Result vs. Watch Metrics

| Watch Metric | Playbook asks | Actual | Available? |
|---|---|---|---|
| DS division OP recovery QoQ | "Strong flash = positive WFE read-through" | Company-wide OP **~₩89.4T (record; 19× YoY increase)** — DS/memory is the primary driver | Partial: company-wide only; segment split in full report |
| DS division revenue | Not specified in flash | Revenue **more than doubled to a record** (total company) | Company-wide only |
| DS capex guidance | **Not in preliminary flash** | n/a — capex is the full-report item (~Jul 30–31) | NOT YET AVAILABLE |
| HBM vs NAND mix commentary | Not in flash | n/a | NOT YET AVAILABLE |
| Samsung vs SK Hynix HBM share commentary | Not in flash | n/a | NOT YET AVAILABLE |

**Assessment:** The preliminary flash is a **strong** top-line signal — a 19× YoY OP surge is the largest in Samsung's history and materially ahead of the ~₩15T estimate many consensus models carried. Revenue more than doubling confirms the memory cycle is at or near peak economics. The DS division is the direct driver (MX/consumer devices do not compound 19× in one year).

The **capex decision branches** in §3 (DS capex maintained vs. cut thresholds) **cannot fire yet** — capex guidance appears only in the full Q2 report July 30–31.

---

## Branch Matched

**Pre-event flash read (§3 pre-event note):**

> "Watch the flash for whether DS division OP recovers QoQ — a **strong DS flash** is a positive read-through to WFE demand."

→ **STRONG DS FLASH** branch engaged.

**Implication:** Positive pre-signal for WFE demand. Confirms the capex-cycle is still expanding into Q2. Does NOT yet fire any of the §3 decision branches (those require capex ₩ guidance from the full report).

**Market reaction (important context — not a playbook branch):**
KOSPI fell ~8% on July 7 (second circuit-breaker event in months); Samsung stock fell ~7%; MU, LRCX, ASML all sold off sharply. The market framing: "good results are already priced in; now comes the AI hardware rotation." This is a **sentiment/reflexivity event**, not a fundamental trigger. The playbook branches run on fundamental inputs (capex ₩, DS OP QoQ), not on stock price action.

---

## Pre-Committed Action (this run)

**No immediate portfolio action required** — the Samsung preliminary flash is a monitoring input, not a decision-tree trigger. Capex decision branches fire at the July 30–31 full report.

**However, three flags are armed for the next sessions:**

1. **LRCX watch-status elevation pending SK Hynix (Jul 24):** If SK Hynix Q2 (§2) shows capex cut >10% vs prior guidance, the playbook says "elevate LRCX to watch status." The Samsung flash doesn't itself trigger this, but the sector tone entering SK Hynix has shifted materially.

2. **MU bear-case discrepancy — flag for Jonathan:** The 7/7 Decisions Log entry ("Bear-case touch — no rating change, PT $1,500") is inconsistent with the MU.md frontmatter (rating: Hold, PT: $1,200, bear: $800, last_updated: 2026-07-07). Either a downgrade was executed on 7/7 without a corresponding Decisions Log entry, or the company file was updated in error. **This gap must be reconciled before MU current price ($938.38) is assessed against the correct bear floor.**

   - If bear is $800 (per file): MU at $938 = 17% above bear → manageable
   - If bear is $900 (per 6/25 log entry / playbook §10): MU at $938 = 4.2% above bear → near-breach territory

3. **ASML entering Q2 print at $1,747:** Only $17 above the stale PT of $1,730. The July 15 print is a PT-reset event (per §4 ratification notes). The chip-sector selloff has done the market's work of re-pricing; the question at the print is now whether EUV ≥60 fires the "reassess Hold toward at-market" branch.

---

## Draft Decisions Log Entry

> This entry covers the Samsung Q2 flash as a macro-input event. No rating or PT change; no execution. Log for record-keeping and sequencing.

| Date | Ticker | Decision | Price @ Decision | PT | Methodology | One-line reasoning | Score |
|---|---|---|---|---|---|---|---|
| 2026-07-08 | SAMSUNG (macro) | **Preliminary flash — strong DS signal; capex decision gated Jul 30–31** | n/a (no position) | n/a | Catalyst Playbook §3 macro input | ₩89.4T Q2 OP (19× YoY record); revenue >2× to record. Flash pre-event note fires "positive WFE read-through." Full capex table (±15% thresholds) gates on full report. Market sold off 7–8% (KOSPI/Samsung) on rotation; treat as sentiment, not fundamental. No action; LRCX/AMAT/ASML confirmation pending Jul 30–31. | Open — gated |

---

## Appendix: Current Prices vs. Playbook Marks (July 8 AM)

| Name | Rating | PT | Bear | Current | vs PT | vs Bear |
|---|---|---|---|---|---|---|
| MU | **Hold*** | **$1,200*** | **$800*** | $938.38 | −22% | +17% |
| LRCX | Buy | $450 | $200 | $326.13 | −27% | +63% |
| ASML | Hold | $1,730 (stale) | n/a (unset) | $1,747.28 | +1% (at stale PT) | — |
| GEV | Buy | $1,200 | n/a | $1,077.08 | −10% | — |
| CEG | Buy | $385 | $220 | $239.71 | −38% | +9% |
| NRG | Buy | $185 | $110 | $138.01 | −25% | +25% |
| VST | Buy | $230 | ~$105 (re-underwrite pending) | $155.73 | −32% | +48% |
| AVGO | Buy | $560 | $350** | $370.78 | −34% | +6% |

*MU rating/PT discrepancy flagged above — file shows Hold/$1,200 but 7/7 log entry shows Buy/$1,500 with "no rating change." Reconciliation required.
**AVGO bear trigger: close <$360 on thesis-negative catalyst (per 7/7 log). Today's price $370.78 = +3% above trigger.

---

## Next Catalyst Gates

| Date | Event | Playbook § | Status |
|---|---|---|---|
| Jul 14 | PJM 2028/29 BRA results | §7 | Armed — CEG/NRG add sizes ratified 7/7 |
| Jul 15 | ASML Q2 | §4 | PT-reset event; all branches trigger PT action |
| Jul 24 | SK Hynix Q2 | §2 | Macro input; LRCX watch-status trigger if capex cut >10% |
| Jul 29 | LRCX Q4 FY2026 | §6 | Revenue vs $6.6B guide; Q1 FY2027 guide gating item |
| Jul 30–31 | Samsung Q2 Full Report | §3 | **Capex decision branches fire here** |
