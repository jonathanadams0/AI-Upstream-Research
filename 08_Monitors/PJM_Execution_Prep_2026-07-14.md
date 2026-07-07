---
tags: [monitor, catalyst-prep, pjm]
event: PJM 2028/29 Base Residual Auction results
event_date: 2026-07-14
prepared: 2026-07-07
status: RATIFIED — add size locked 7/7; execute after results post (~4pm ET Jul 14)
---

# PJM 2028/29 BRA — Execution Prep (staged 2026-07-07)

> Everything needed to execute [[Catalyst Playbooks]] §7 same-day. Results post on pjm.com after **4pm ET Tuesday July 14**. Bids closed July 7. Price cap ~$325/MW-day; prior (2027/28) BRA cleared **$333.44** at the then-cap; the one before cleared $269.92. This is the book's biggest pre-committed action — CEG and NRG are both T1 6.5%.

---

## 1. Where the names sit going in (7/7 intraday, AI-unwind tape)

| Name | Rating/PT | Price 7/7 | vs entry | Bear | To bear | To PT | Asym | Position |
|---|---|---|---|---|---|---|---|---|
| **CEG** | Buy/$385 | $242.26 | −3.7% | $220 | −9.2% ⚠️ | +59% | **6.4x** | T1 6.5% |
| **NRG** | Buy/$185 | $138.04 | +6.2% | $110 | −20% | +34% | 1.7x | T1 6.5% |
| **VST** | Buy/$230 | $154.73 | +5.8% | $105 (re-underwritten 6/23; frontmatter/MP $145) | −6–32% | +49% | ~1.1x | T2 4% |

The unwind has *improved* the add math vs when the playbook was ratified (CEG was $260+ then). Both CEG and NRG clear the ≥1.5x asymmetry bar at today's prices; they are Group 3 power names, so the 6/25 Group-1 guardrail does not apply.

## 2. Branch table (ratified 6/23, corrected 7/2) — with staged execution

| Clearing price | Ratified action | Staged execution (recompute shares at 7/14 close) |
|---|---|---|
| **> $325** (cap-clearing) | **Add CEG + NRG**; revisit PTs upward; log same day | Add **2% each** (see §3): CEG ~$2,000 ≈ 8.26 sh @ $242; NRG ~$2,000 ≈ 14.49 sh @ $138. Cash $15,812 → ~$11,812 (11.8%). Then PT revisit: each +$50/MW-day ≈ +$400M annual EBITDA for CEG — a $325+ print vs the $270 prior supports raising the PJM leg. |
| **$270 – $325** | No action; confirm PTs | Write the Catalyst Reaction note; confirm CEG $385 / NRG $185; no trades. |
| **< $270** | Re-underwrite PJM leg of VST/CEG within 1 week; downgrade if PT support drops >15% | ⚠️ **CEG is only 9.2% above bear going in** — a weak print + tape means the re-underwrite happens FAST (target: within 2 sessions, not 1 week). Stage the CEG DCF PJM-leg sensitivity before Jul 14 if time allows. |
| Delayed / FERC CIFP change | Check CEG #1 invalidation (FERC co-location ruling) first | No trade until checked. |

## 3. The one decision to make BEFORE results: add size

§7 says "upsize one tier," written when the add routed through VST (T2→T1). CEG/NRG are already T1 — there is no higher tier. **Staged default: +2% (one T3-increment) each**, funded from cash, taking each to 8.5% effective. Rationale: keeps total power-complex exposure ≤ ~26% of book, preserves >10% cash into the Jul 15–Aug 13 gauntlet, and respects that T1 6.5% is the framework's max *initial* weight, not a hard cap on adds. Alternative (+1% each) if the tape is still breaking down. **RATIFIED 2026-07-07 by Jonathan: +2% each. Logged in [[Decisions Log]] 7/7 — execution on Jul 14 is mechanical.**

**VST: staged NO-ADD even on a >$325 print.** The 6/23 re-underwrite is complete and survived, but asymmetry is ~1.1x — below the 1.5x bar — and §7's add was explicitly rerouted to CEG/NRG on 6/23. A cap-clearing print helps VST's Q2 print (Aug 7) instead; revisit there.

## 4. Same-day checklist (after 4pm ET Jul 14)

1. Pull clearing price (RTO-wide + relevant LDAs) from pjm.com press release.
2. Match branch → write `Catalyst_Reaction_PJM_2026-07-14.md` (the 7am catalyst-execution loop will draft this Wednesday morning if not done Tuesday — doing it Tuesday is better).
3. Decisions Log rows: one per name acted on (price at decision, branch cited, sizing math).
4. Model Portfolio: position rows + Change Log + cash reconciliation (if adds fire).
5. Update CEG/NRG/VST notes' PJM sections + `current_price`.
6. Sanity checks: CEG vs $220 bear; the 2027/28 print ($333.44) as the reference; don't confuse delivery years — this is **2028/29**.

## 5. Context worth having on screen

Each +$50/MW-day ≈ +$400M annual for CEG (playbook math). VST's own Q3'25 call floated a $329 scenario. A second consecutive cap-clearing auction would confirm the structural reserve-margin thesis (interconnection queue + data-center load growth) — that's the variant perception that justified CEG at 47% below consensus PT. Conversely, a sub-$270 print with CEG 9% above bear is the single worst combination on the July calendar — which is exactly why the re-underwrite path is staged above.

*Prices: live intraday 2026-07-07 (FMP). Recompute all share counts at the 7/14 close before executing. This note stages decisions; the Decisions Log entries on 7/14 are the record.*
