---
tags: [monitor, pjm, power, CEG, NRG, VST]
run_date: 2026-07-01
catalyst: PJM Capacity Auction (2028/2029 delivery year)
status: IN PROGRESS — results expected July 14, 2026
---

# PJM Monitor — July 1, 2026

> **No playbook catalyst resolved in the last 24 hours.** This note documents two material PJM-related developments that affect the active CEG / NRG / VST decision tree.

---

## 1. PJM 2028/2029 BRA — In Progress

**Status:** Offer window opened June 30, 2026 (yesterday). Bids close July 7; results posted July 14 after 4pm ET.

**Playbook note correction:** The [[Catalyst Playbooks]] entry §7 labels this auction "(2027/2028 delivery year)" — this appears to be a typo. The 2027/2028 BRA already cleared **December 17, 2025 at $333.44/MW-day** (the FERC price cap; ~$121,705/MW-year). The vault's "~July 2026" date correctly points to the **2028/2029 BRA**, which is now confirmed as the active event.

**Price cap for 2028/2029 BRA:** ~$325/MW-day (approximately equal to the playbook's ">$325 add branch" threshold). In 2027/2028, the auction hit the cap because the RTO fell short of its reliability requirement for the first time; without the cap, it would have cleared at ~$194k/MW-year (+60%). Supply/demand conditions are similar heading into 2028/2029.

**Watch for July 14:** Whether the clearing price exceeds $325/MW-day:

| Outcome | Branch | Pre-committed action |
|---|---|---|
| **> $325/MW-day** | Structural tightening confirmed | **Add to CEG and NRG** (upsize one tier); revisit PTs; VST add only if bear re-underwrite complete |
| **$270–$325** | In-line | No action; confirm PTs unchanged |
| **< $270** | Reserve-margin thesis weakening | Re-underwrite PJM leg within 1 week |

**Set a calendar reminder for July 14, 4pm ET.**

---

## 2. DOE PJM Power Emergency — July 1–3, 2026

**Event:** On June 30, the DOE issued an emergency order under Federal Power Act Section 202(c) authorizing PJM Interconnection to:
- Waive environmental emission limits for generation plants
- Curtail large industrial loads including co-located data centers

**Trigger:** PJM is forecasting 166,304 MW peak demand on July 2, which would break the all-time PJM record (165,563 MW, 2006). Heat index forecasts ~95°F+. Emergency orders take effect 11:59pm July 1 and expire 11:59pm July 3.

**This is NOT a playbook catalyst.** There is no pre-committed decision tree for a DOE Section 202(c) order. Key read-throughs for covered names:

- **CEG ($248.37, −$10.95 today):** Nuclear fleet runs baseload regardless; emergency does not materially affect output. The real-time energy price spike during peak hours benefits the small portion of output sold into spot markets. The data-center co-location curtailment order is an important development — **check CEG's #1 invalidation condition** (FERC ruling against co-location). If FERC uses this emergency to formalize co-location curtailment rights, it reduces the value of CEG's Microsoft/other co-location agreements.
- **NRG ($146.06, −$3.05):** Gas and peaker fleet benefits directly from energy price spikes during peak hours. Emergency is operationally positive.
- **VST ($158.63, −$3.75):** ERCOT is the primary VST market (not PJM), so direct impact is limited. PJM power prices bleeding through to day-ahead market signal is marginally positive. Cogentrix (PJM-footprint CCGT acquisition) adds some exposure.

**Why are all three down today?** Likely broad market weakness (Wall St futures slipping, US-Iran tensions, rate hike expectations) rather than PJM-specific news. Nothing in the emergency order is structurally negative for the power thesis.

---

## Current Prices vs. Playbook Entries

| Ticker | Rating | PT | Bear | Price (7/1) | Upside to PT | Downside to Bear |
|---|---|---|---|---|---|---|
| CEG | Buy | $385 | $220 | $248.37 | +55% | −11% |
| NRG | Buy | $185 | $110 | $146.06 | +27% | −25% |
| VST | Buy | $230 | $105* | $158.63 | +45% | −34% |

*VST bear re-underwrite still pending per playbook §1 note — bear $105 is the ratified figure but the full re-underwrite is a pre-req for any add.

---

## Next Action

**July 14, 2026:** Check PJM.com for 2028/2029 BRA clearing price. If >$325/MW-day, execute the Add branch per [[Catalyst Playbooks]] §7 and log in [[Decisions Log]] same day. If the cap for 2028/2029 is set at $325/MW-day and the auction hits it, treat as clearing ">$325" per the spirit of the playbook.

Also monitor FERC actions around co-location policy this week given the DOE emergency context — this is CEG's #1 invalidation condition.
