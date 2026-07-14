---
tags: [monitor, catalyst-reaction, pjm]
tickers: [CEG, NRG, VST]
event: PJM 2028/2029 BRA clearing price
event_date: 2026-07-14
run_time: 2026-07-14 evening (pjm-2028-29-bra-execution scheduled task; supersedes the PENDING draft from the earlier run)
status: RESOLVED — print confirmed, add branch EXECUTED
branch_matched: ">$325 cap-clearing (print AT the $325 cap)"
action: EXECUTED — +2% CEG and +2% NRG added at official 7/14 closes
---

# PJM 2028/2029 BRA — Catalyst Reaction (EXECUTED)

> **Supersedes the PENDING draft written by the earlier automated run** (results had not yet posted). One correction to that draft: it labeled CEG $257.57 / NRG $139.48 / VST $158.12 as "July 14 closes" — those were the **July 13** closes. Official **July 14** closes (FMP, 4:00pm ET timestamps): **CEG $256.43 (−0.4%), NRG $138.36 (−0.8%), VST $158.43 (+0.2%)**. Execution below uses the correct 7/14 closes.

---

## 1. The print

**$325.00/MW-day (UCAP), at the FERC-approved cap, for the entire PJM footprint** — a single RTO-wide price; no zonal/LDA outliers in the press release (detailed BRA report to follow on pjm.com). The 2.5% decline vs the 2027/28 print ($333.44) is entirely the lower cap, not softer demand. **Third consecutive auction clearing at the collar cap.**

Key auction facts ([PJM press release, 7/14](https://www.prnewswire.com/news-releases/pjm-capacity-auction-procures-138-318-mw-of-generation-resources-as-work-continues-to-address-growing-electricity-demand-302825613.html)):

- 138,318 MW UCAP procured (+3,733 MW vs 2027/28); total auction value $16.4B.
- **6,831 MW short of the reliability requirement** — second consecutive RTO-wide shortfall vs the 1-in-10 standard (prior ~6,500 MW). PJM will seek FERC approval for a special **Backstop Procurement in September**.
- Only **525 MW UCAP of new generation/uprates cleared** — the capacity increase came from accreditation changes and coal→gas conversions, not new build. Supply response remains anemic.
- Forecast peak load +~2,000 MW vs the prior auction; large data-center loads again cited in the load forecast.
- Reserve margin 14.7%. Next BRA (2029/30) in December.

## 2. Branch match

Playbook §7 (corrected 7/2) is explicit: *"Price cap ~$325/MW-day ≈ the '>$325 add branch' threshold below, so a cap-clearing print fires the add branch at the cap itself."* Print cleared **at** the cap → **add branch fires**. Pre-ratified by Jonathan 7/7 ([[Decisions Log]]): +2% each CEG and NRG at the 7/14 close, funded from cash; VST no-add on any branch.

## 3. Execution (official 7/14 closes)

| Name | 7/14 close | Add | Shares added | New position | New cost | Effective wt |
|---|---|---|---|---|---|---|
| **CEG** | $256.43 | +2% ($2,000) | **7.7994** | 33.6289 sh | $8,500 | 8.5% |
| **NRG** | $138.36 | +2% ($2,000) | **14.4550** | 64.4704 sh | $8,500 | 8.5% |
| **VST** | $158.43 | **no add** (ratified: asym ~1.1x) | — | 27.3560 sh | $4,000 | 4% |

Cash: $15,812 − $4,000 = **$11,812 (11.8% of the $100k model)** — above the >10% floor staged for the Jul 15–Aug 13 gauntlet. (The PENDING draft's "below the cash floor" worry was arithmetic error — 11.8% > 10%.) Power-complex exposure stays ≤ ~26% of book as staged.

The closes predate the after-4pm release; the muted session is the "partly priced" case the 7/13 refresh flagged (CEG +2.5% Monday read as anticipation). Per prep: the add is committed on the *print*, not the reaction. Wednesday's open gives the first market read.

## 4. Sanity checks (prep §4/§6)

- **CEG $256.43 vs $220 bear floor: +16.6% — no bear-floor protocol.** Cushion improved from 9.2% at 7/7 staging.
- Delivery-year check ✓ — this is the **2028/29** BRA ($333.44 was 2027/28).
- Asymmetry at execution: CEG +50% to PT / −14.2% to bear ≈ **3.5x**; NRG +34% / −20.3% ≈ **1.7x** — both clear the 1.5x bar ✓.
- Sensitivity note ([[CEG_PJM_Sensitivity_2026-07-14]]) not needed — strong-print branch.

## 5. Thesis read + PT revisit (QUEUED — needs a decision, not mechanical)

A third consecutive cap-clearing print **with a widening reliability shortfall and near-zero new build clearing** confirms the structural reserve-margin thesis on every axis — and adds a catalyst the playbook didn't have: the September Backstop Procurement (separate, additive procurement mechanism; see the Inside Lines 7/1 context in the superseded draft, preserved in git history — net read mildly positive CEG, neutral-to-watch NRG/VST on curtailment-rights design).

Branch says "revisit CEG/NRG PTs upward." Arithmetic from the sensitivity note: $325 vs the $269.92 baseline = +$440M annual EBITDA → **+$14 to +$20/sh of CEG PT support (~$400–405 case vs the current $385)**. Caveat from the same note: consensus likely already embeds something between $270 and $333, so incremental support vs expectations is smaller. **PT revisit was not pre-ratified with numbers — queued for Jonathan / next session rather than executed tonight.** NRG PT revisit additionally needs its PJM cleared-MW quantified (verification item; Aug 4 print).

VST: the print half-satisfies the best row of its Aug 7 Q2 branch ("Cogentrix closes **+ PJM cleared >$325**" → consider T1) — Cogentrix close status is now the live variable.

## 6. Follow-ups

1. **CEG/NRG PT revisit decision** — next session (arithmetic in §5).
2. Add **PJM Backstop Procurement (September)** to [[Catalyst Playbooks]] as a dated entry when the FERC filing lands.
3. Verify CEG/NRG cleared MW against the detailed BRA report when posted (checks the 21.9 GW implied figure in the sensitivity note).
4. Update CEG/NRG/VST company notes' PJM sections + `current_price` (left for tomorrow's 7am catalyst-execution run).
5. Diarize the 2029/30 BRA (December) when PJM confirms the date — last collared auction context.

---

*Sources: [PJM press release 7/14/2026](https://www.prnewswire.com/news-releases/pjm-capacity-auction-procures-138-318-mw-of-generation-resources-as-work-continues-to-address-growing-electricity-demand-302825613.html) · closes via FMP batch quote (4:00pm ET 7/14 timestamps) · [[Catalyst Playbooks]] §7 (ratified 6/23, corrected 7/2) · [[PJM_Execution_Prep_2026-07-14]] (staging + 7/13 refresh) · [[Decisions Log]] 7/7 (add size ratified).*
