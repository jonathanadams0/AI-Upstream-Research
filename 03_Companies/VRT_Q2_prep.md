# VRT Q2 Earnings Prep
**Date:** 2026-07-20 | **Expected report:** ~2026-07-29 (confirmed via Bigdata.com/Quartr earnings calendar — matches frontmatter `next_earnings`)

---

## Setup

| Item | Value |
|---|---|
| Rating / PT | Buy / $370.00 |
| Current price | $289.41 |
| Conviction | High |
| Thesis (one-line) | Vertiv is the dominant global supplier of thermal management, power distribution, and IT infrastructure for data centers — one of the most direct pure-play beneficiaries of hyperscaler/colo AI capex, with revenue nearly doubling in three years on structural demand that shows no sign of abating. |

*Note: [[VRT]] note body header still reads "Rating: Under Review / PT: —" (stale from an earlier draft pass) while YAML frontmatter — the source of truth per vault convention — carries Buy/$370. Flagged for cleanup; not corrected here per constraints.*

---

## Invalidation Trigger

> From the vault's Thesis Invalidation Tracker ([[Portfolio Summary]]):
> **Sell Trigger:** Order guidance cut >15% in single quarter | **Monitor Via:** Quarterly orders slide.

**What in this print would fire it:** VRT's order growth is the market's real-time proxy for AI data center capex, and management leads with the orders slide every quarter. The most recent cited figure in the vault (Q4'25) was **orders +252% YoY** (per [[Vertiv as the AI Cooling Pure-Play]] and [[Liquid Cooling Mass Adoption]]) — an extraordinary, likely unsustainable comp. The trigger fires on a >15% guided cut to orders in a single quarter, not merely a deceleration in the YoY growth rate off that base. The vault's own thesis notes flag this explicitly: expect Q2'26 YoY orders growth to look much smaller against the Q4'25/Q1'26 comps, and the market may misread normalization as demand deterioration — the actual test is whether management characterizes the change as a guidance cut versus a comp effect. Also watch the bear case's companion metric: gross margin sustained below 30% (vs. ~36% currently) would compound the read as a real thesis crack, not just noisy comps.

---

## 3 Questions This Print Must Answer

1. **Orders/bookings trajectory.** Did Q2'26 order growth (YoY and sequential book-to-bill) show a genuine deceleration versus the extraordinary +252% YoY Q4'25 base, or does the growth rate remain robust even against a tough comp? This is the single most-watched line in the release (per [[Cooling-Thermal]] sector note: "VRT orders growth and book-to-bill... best real-time AI capex signal").
2. **Gross margin durability.** Did gross margin hold at or above the ~36% level cited in the bear case, or is there evidence of the sub-30% compression trigger from competitive pricing (Schneider Electric, new liquid-cooling entrants) that the note's Bear Case explicitly flags as a rating-change condition?
3. **Verification-flag resolution.** The [[VRT]] note carries dozens of unresolved `[VERIFY]` tags (segment revenue mix, AI-linked revenue attribution %, current backlog/lead-time detail, current trading multiple, hyperscaler capex guidance cross-checks). Does the 10-Q/earnings call supply updated segment and backlog disclosure that can close any of these open items?

---

## Consensus Expectations

**Consensus (pull from terminal):** Bigdata.com's analyst-estimates feed (FMP-sourced, 12 analysts) returned forward quarterly estimates starting at **FY2026 Q3** ($3.71B revenue / $1.78 EPS mean) — the imminent **Q2 2026** quarter (the one reporting ~7/29) was **not present** in the returned dataset, likely rolled off ahead of the print. Do not treat the Q3 figures below as the Q2 consensus.

| Metric | FY2026 Q3 consensus (context only — not the reporting quarter) |
|---|---|
| Revenue | ~$3.71B (12 analysts) |
| EPS | ~$1.78 (12 analysts) |
| EBITDA | ~$528M |

**Q2 2026 consensus EPS/revenue: not retrievable via available tools as of this run.** Pull from Bloomberg/FactSet terminal before the print.

---

## Playbook Check

No existing [[Catalyst Playbooks]] entry for VRT. Buy-rated → DRAFT playbook below; all thresholds are DRAFT and unofficial.

| Outcome | Read | Action (DRAFT) |
|---|---|---|
| DRAFT: Orders growth ≥30% YoY (even off tough comp) + gross margin ≥36% + no hyperscaler capex pause disclosed | Bull — AI cooling demand still accelerating; thesis strengthening | DRAFT: Hold position; flag for PT-raise review; no add without fresh asymmetry check |
| DRAFT: Orders growth 10–30% YoY + gross margin 33–36% + backlog stable | In-line — normalization off an extraordinary base, thesis intact | DRAFT: No action; re-confirm at Q3 that deceleration is comp-driven, not demand-driven |
| DRAFT: Orders guidance cut >15% in the quarter (tracker trigger) or growth <10% YoY | Bear — approaching/at the tracked sell trigger | DRAFT: Escalate to re-underwrite; cross-check gross margin and hyperscaler commentary before any rating action |
| DRAFT: Gross margin <30% sustained (bear case condition #2) | Margin compression confirms competitive erosion, not just a comp effect | DRAFT: Rating review triggered per [[VRT]] note's explicit Bear Case change-to-Hold/Sell criteria |

---

## Data Sources

- [[VRT]] company note (frontmatter + Bear Case §9 + Catalysts §8)
- [[Portfolio Summary]] Thesis Invalidation Tracker and catalyst calendar
- [[Vertiv as the AI Cooling Pure-Play]] and [[Liquid Cooling Mass Adoption]] thesis notes (Q4'25 orders +252% YoY figure)
- [[Cooling-Thermal]] sector note
- Bigdata.com company tearsheet (`analyst_estimates`, `earnings_calendar`) via `find_securities` (rp_entity_id `96D34D`)

---

**Powered by [Bigdata.com](https://bigdata.com)**

*For informational purposes only. Not investment advice.*
