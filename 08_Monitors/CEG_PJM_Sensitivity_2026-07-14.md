---
tags: [monitor, catalyst-prep, pjm, sensitivity]
ticker: CEG
event: PJM 2028/29 BRA results
event_date: 2026-07-14
prepared: 2026-07-07
status: STAGED — companion to [[PJM_Execution_Prep_2026-07-14]] (the <$270 branch)
---

# CEG — PJM-Leg Downside Sensitivity (staged 2026-07-07)

> Pre-computed math for the worst branch: **what does a weak 2028/29 BRA print actually cost CEG's $385 PT?** Built so Wednesday morning is arithmetic, not improvisation. Companion to [[PJM_Execution_Prep_2026-07-14]]; anchors from [[CEG_DCF_v1.xlsx]] (14x exit multiple) and [[Catalyst Playbooks]] §7.

---

## 1. The anchor math

- Playbook ratio: **each +$50/MW-day ≈ +$400M annual EBITDA for CEG** → implies ~21.9 GW of cleared PJM capacity ($400M ÷ ($50 × 365)).
- Value per EBITDA dollar: the DCF uses a **14x exit multiple**; live IPP forward multiples run ~10–12x. Use a 10–14x band.
- Share count: ~313M (mkt cap ~$76B at $242.26).
- Baseline embedded in estimates: prior BRA prints — $269.92 (2026/27) and **$333.44 (2027/28, cap-clearing)**. Note the asymmetric baseline: consensus 2028+ estimates likely embed something *between* those, so a $270 print is a mild negative vs. the $333 anchor even though it sits at the branch boundary.

## 2. Sensitivity table (sustained, curve-level repricing — the worst-case read)

Per −$25/MW-day *if the market treats the print as the new permanent clearing level*:
−$200M EBITDA × 10–14x = $2.0–2.8B EV ≈ **−$6.40 to −$8.90/share ≈ −1.7% to −2.3% of the $385 PT.**

| 2028/29 print | Δ vs $269.92 | Δ EBITDA (annual) | PT support impact (10–14x) | % of $385 PT |
|---|---|---|---|---|
| **$325+ (cap)** | +$55 | **+$440M** | **+$14 to +$20/sh** | +4–5% → supports PT raise |
| $295 | +$25 | +$200M | +$6 to +$9/sh | +2% |
| $270 (prior) | ~0 | ~0 | ~0 | branch boundary |
| $245 | −$25 | −$200M | −$6 to −$9/sh | −2% |
| $220 | −$50 | −$400M | −$13 to −$18/sh | −3 to −5% |
| $195 | −$75 | −$600M | −$19 to −$27/sh | −5 to −7% |

**The punchline: the >15% PT-support drop that triggers the downgrade branch requires roughly a −$165 to −$230/MW-day sustained repricing — i.e., a clearing print near $40–105/MW-day, the pre-2024 world.** No plausible single print gets there. Mechanically, even $195 costs CEG mid-single-digit % of PT support.

## 3. What this means for the <$270 branch

1. **A weak print is a narrative event, not an arithmetic event.** CEG's $385 PT rests mostly on the nuclear PPA repricing (Microsoft/Meta 20-year deals), the PTC floor ($15/MWh through 2032), and Calpine accretion — none of which a BRA print touches. Capacity payments are one revenue layer of several.
2. **So the re-underwrite must answer WHY it cleared low, not just how low:** (a) big new supply cleared (queue reform working faster than the reserve-margin thesis assumes → genuine thesis dent — this is the one that matters); (b) demand-forecast revision by PJM (data-center load pushed out → read-through to the whole power tier); (c) technical/one-off (cap mechanics, RMR treatment, LDA quirks → noise). Only (a) or (b) sustained justifies touching the rating.
3. **Price risk ≠ PT risk.** CEG at $242 is 10% above the $220 bear; a weak print plus this tape could push the *stock* through $220 even though the *PT support* moves ~2–5%. If that happens, the bear-floor protocol (MU-style: formal re-underwrite, no reflexive exit) governs — the $220 bear was built on thesis-break scenarios (adverse FERC co-location ruling, Calpine <$1.5B, capacity factor <90%), not on one auction print.
4. **NRG:** the $400M/$50 ratio is CEG-specific. NRG is ERCOT/retail-heavy with smaller PJM merchant leverage; treat a weak print as a smaller fundamental event for NRG but the same narrative event. Quantify NRG's PJM MW at the Aug 4 print (verification item).

## 4. Pre-commitments for the weak-print path (completes the ratified branch)

- Print $245–270: log a no-action confirmation with the table above cited. No PT change on arithmetic this small.
- Print $220–245: re-underwrite within 2 sessions focused on cause (a)/(b)/(c); PT haircut capped at the table's arithmetic unless cause (a) confirmed.
- Print <$220 or cause (a) confirmed: full PJM-leg rebuild in the DCF (the model's To-Do already lists the sum-of-parts build — do it then); rating decision follows the rebuilt numbers.
- Any print + CEG closes <$220: bear-floor protocol fires in parallel (separate from the auction logic).

*Sources: ratio and baselines from [[Catalyst Playbooks]] §7 (ratified 6/23, corrected 7/2); multiple band from CEG_DCF_v1 (14x exit) and live IPP comps; share count from 7/7 market cap. The 21.9 GW implied capacity is derived from the playbook ratio — verify against actual CEG cleared MW when PJM publishes auction detail.*
