---
date: 2026-06-23
type: stress-test
topic: High-Sensitivity Thesis Review — AI Capex Deceleration Scenario
related: AI_Semi_Selloff_Analysis_2026-06-23.md
tags: [stress-test, macro, AI-capex, WFE, HBM, NAND, packaging, networking]
---

# Thesis Stress Test — AI Capex Deceleration Scenario
*June 23, 2026 | In response to today's AI/semi selloff*

---

## The Scenario Being Applied

The evidence from the selloff analysis points to one central shift: **AI capex growth is decelerating from ~75% YoY (2025 peak) toward ~20-25% YoY by end-2026.** Absolute spending is still rising — hyperscalers will invest $650-700B in 2026. But the *rate of change* that powered a multi-hundred-percent run in semiconductor stocks is moderating.

This stress test asks a precise question for each thesis: **which core assumptions break, weaken, or hold under a sustained 20-25% AI capex growth environment?**

Importantly, this is not a "AI is over" scenario. It's a "we're in the second inning of a long game but valuations were priced for the first inning's pace forever" scenario.

---

## Summary Scorecard

| Thesis | Verdict | Conviction Change | Urgency |
|---|---|---|---|
| HBM Supply Constraint | **Holds — with key signal to watch** | High → High | Medium |
| Memory Bottleneck | **Weakens** | High → Medium | High |
| WFE Supercycle | **Holds 2026; uncertain 2027+** | High → Medium-High | Medium |
| Advanced Packaging Bottleneck | **Resolving — thesis matures** | High → Medium | Medium |
| AI Networking & Custom Silicon | **Split: Custom holds, Networking moderates** | High → Mixed | Medium-High |

---

## 1. HBM Supply Constraint

**Thesis recap:** HBM is structurally supply-constrained regardless of which AI company wins because each new HBM generation is more etch-intensive. LRCX and AMAT benefit from capacity expansion regardless of volume.

### Assumptions tested

| Assumption | Under Stress | Assessment |
|---|---|---|
| HBM demand grows faster than capacity additions through 2027 | 20-25% AI capex growth = 20-25% GPU volume growth = ~20-25% HBM volume demand growth | **Holds** — still positive demand growth, and capacity additions are still lagging (18-24 month lead times) |
| Each HBM generation is more etch-intensive per wafer | HBM4 transition is happening regardless of AI capex cycle pace | **Holds** — this is architecture-driven, not volume-driven |
| Equipment orders are durable (backlog visibility) | Orders placed in 2025/H1 2026 support 2026 revenue; deceleration affects 2027+ orders | **Holds for 2026; watch 2027** |
| Memory manufacturers keep investing in HBM capacity | If AI GPU demand decelerates meaningfully, SK Hynix/Samsung could cut WFE capex quickly — this is exactly how memory cycles work | **Fragile** — this is the key risk |

### What breaks first

The thesis's Achilles heel is the **memory OEM capex decision loop.** Unlike logic chips, memory manufacturers have historically been fast to cut equipment spending when demand signals weaken. If SK Hynix or Samsung leadership signals any HBM capex pause in upcoming earnings calls, LRCX/AMAT HBM-related orders could soften faster than the current 2026 revenue implies.

The structural safeguard: Micron's US CHIPS Act investment is committed and partly US-government backstopped — that portion of HBM capex is more durable than commercial decisions.

### Verdict
**Thesis holds.** Downgrade risk is low for 2026 equipment revenue; higher for 2027 assumptions. The HBM generation-upgrade mechanism (more etch intensity per wafer regardless of volume) is the most durable element of the thesis and survives capex deceleration.

**Signal to monitor:** SK Hynix Q2 2026 earnings call (late July) — any guidance change on HBM capacity investment. Also watch LRCX book-to-bill ratio: >1.0 means orders still growing; <1.0 is an early warning.

---

## 2. Memory Bottleneck

**Thesis recap:** AI is memory-bandwidth-limited across all three layers — HBM (on-package), NAND (inference storage), HDD (cold tier). Each layer is simultaneously supply-constrained, creating a multi-year pricing tailwind.

### Assumptions tested

| Assumption | Under Stress | Assessment |
|---|---|---|
| HBM component: demand > supply through 2027 | See HBM thesis above | **Holds** |
| NAND prices remain elevated (5-10x above 2023 trough) | NAND is the most cyclical component. Price levels this elevated require continued demand acceleration to hold; deceleration risks price normalization | **At risk** |
| HDD demand (Seagate +500% YoY) reflects structural AI storage demand | Cold storage demand grows with AI data assets regardless of capex pace — but valuation is pricing in continued acceleration | **Partially at risk** |
| SNDK's NBM contracts protect against NAND cycle reversal | The contracts provide floor-ceiling pricing — *if* they hold in a down scenario | **Dependent on NBM durability** |

### What breaks first

**NAND pricing** is the most exposed element. The 5-10x price recovery from the 2023 trough was driven partly by genuine AI demand and partly by a structural supply correction (memory OEMs had cut too deep in 2023). At these elevated prices, any deceleration in AI data growth or inference expansion means NAND supply additions start to outpace demand increments — and NAND prices correct faster than they rise.

The most direct read-through: **SNDK's Q4 FY2026 earnings (August 13)** — if gross margins hold at 78-80% and the NBM contracts are intact, the thesis survives. If hyperscalers are renegotiating contracts or deferring purchases, the thesis structure breaks.

HDD is a secondary concern — Seagate at +500% YoY is pricing a lot of AI storage optionality. 20-25% AI capex growth is still positive but doesn't justify peak-narrative valuations for HDD (the vault has STX at Hold $910; maintain).

### Verdict
**Thesis weakens. Conviction drops from High to Medium.** The HBM component remains sound but the NAND pricing premium and HDD valuation theses are directly vulnerable to capex deceleration. The thesis structure isn't broken — but it needs monitoring at every earnings cycle.

**Actions:**
- SNDK: Don't add until Q4 earnings confirm NBM intact and margins hold (see portfolio monitor)
- WDC/STX: Hold ratings appropriate; thesis still directionally correct but valuation upside is reduced
- Watch NAND spot price indices (TrendForce publishes monthly) — any sustained decline from current levels is a thesis flag

---

## 3. WFE Supercycle

**Thesis recap:** WFE is entering a $140B+ structural plateau (vs. prior $100B peak) driven by AI infrastructure investment. Multiple simultaneous demand vectors (logic, HBM, NAND, packaging) and SAM expansion for equipment companies means this isn't a traditional boom-bust cycle.

### Assumptions tested

| Assumption | Under Stress | Assessment |
|---|---|---|
| WFE reaches $140-155B in 2026 | 2026 revenue is substantially backed by orders already placed; delivery lead times mean current year is largely locked in | **Holds for 2026** |
| WFE reaches $215B ±$20B by 2030 | This requires sustained ~10-12% CAGR from $140B. Under 20-25% AI capex growth (vs. prior 50-75%), this is achievable but with wider error bars | **Uncertain** |
| "WFE doesn't go back" — structural step-up above $100B | Even under capex deceleration, hyperscaler commitments and the AI chip arms race prevent a full cycle reset | **Holds in principle; magnitude uncertain** |
| SAM expansion (LRCX, KLAC) means faster revenue growth than WFE | SAM expansion is architecture-driven (more etch/inspection per wafer as nodes advance), not purely volume-driven | **Holds** |
| Four simultaneous demand vectors prevent traditional cycle | If any of the four (logic, HBM, NAND, CoWoS) slow simultaneously, the "counter-cyclical diversification" argument weakens | **Partially at risk** |

### The lag structure is your ally — for now

This is the key nuance for WFE: there is a 6-18 month lag between equipment order and revenue recognition. The WFE supercycle's 2026 revenue is not at risk from today's sentiment shift — it was booked in 2025. **The risk is to 2027 bookings and 2027-2028 revenue.** This gives you a 6-12 month window to see how capex deceleration plays out before it shows up in equipment financials.

Watch the **book-to-bill ratio** as the leading indicator. If LRCX, AMAT, or KLAC report book-to-bill <1.0 for two consecutive quarters, the 2030 target comes under real pressure.

### China tail risk amplification

Under capex deceleration, China export controls become relatively more important as a risk factor — the US WFE companies have 15-30% China revenue that is exposed to tightening restrictions independent of global AI capex trends. If capex growth globally decelerates AND China revenue gets restricted, the WFE names face a double headwind that is not in the current base case.

### Verdict
**Thesis holds for 2026 due to backlog. Medium-High conviction with elevated 2027+ uncertainty.** The structural step-up argument is sound but the $215B by 2030 scenario requires assumptions that are now harder to defend without re-acceleration.

**Signal to monitor:** Quarterly book-to-bill ratio at LRCX, AMAT, KLAC. SAM guidance updates (LRCX CEO has been the most explicit — watch his commentary at any upcoming conferences). TSMC capex guidance for 2027 (usually disclosed in Q4 analyst day).

---

## 4. Advanced Packaging Bottleneck

**Thesis recap:** CoWoS is the binding constraint on AI GPU supply. TSMC's capacity expansion drives equipment orders at LRCX, AMAT, and KLAC. The bottleneck creates premium orders and elevated equipment spending per wafer.

### Assumptions tested

| Assumption | Under Stress | Assessment |
|---|---|---|
| CoWoS capacity remains the binding constraint on AI GPU supply | TSMC expanding from 5K wspm (2023) → 35-40K wspm (2026E) — 7-8x capacity in 3 years. At some point, supply meets demand. | **Weakening** |
| Capacity expansion drives ongoing equipment orders | Expansion phase drives orders; once at steady-state capacity, replacement cycle is the driver (much smaller revenue) | **Transitioning** |
| AI GPU demand continues to outpace CoWoS capacity additions | At 20-25% AI capex growth, GPU demand grows 20-25% per year — still positive but TSMC may be catching up | **Uncertain** |

### The thesis is maturing — not breaking

This is the subtlest of the five stress tests. The Advanced Packaging Bottleneck thesis was written when CoWoS was *violently* undersupplied (H100 availability was gated by CoWoS in 2023). The thesis has been playing out successfully — TSMC has invested billions and expanded capacity 8x. The equipment revenue from that expansion has already benefited LRCX/KLAC/AMAT.

The question is: **is the bottleneck still a bottleneck at 40K wspm?** At 20-25% AI capex growth, TSMC's aggressive expansion may be catching up with demand. If CoWoS utilization rates normalize (vs. the near-100% they were in 2023-2024), the "crisis premium" in equipment orders disappears. Advanced packaging remains a real and growing equipment segment — just not at the "emergency expansion" premium.

**This isn't a thesis break — it's a thesis completion.** The bottleneck played out and was resolved by investment. The question now is what the steady-state growth rate looks like, which is more like a normal WFE growth thesis (covered by the WFE Supercycle thesis) than a "bottleneck premium" thesis.

### Verdict
**Thesis is maturing from bottleneck to steady-state. Conviction drops from High to Medium.** The emergency capacity expansion phase is likely approaching its end. Advanced packaging remains a growing equipment sub-segment but no longer commands a "crisis premium" thesis. Consider archiving or downgrading this thesis and folding the ongoing advanced packaging tailwind into the WFE Supercycle thesis.

**Suggested action:** Revise status from Active (High) → Active (Medium) and add note: *"Bottleneck phase largely resolved; ongoing demand growth now captured under WFE Supercycle thesis."*

---

## 5. AI Networking and Custom Silicon

**Thesis recap:** Two sub-theses: (1) Hyperscalers are building custom AI silicon via Broadcom and Marvell to reduce Nvidia dependency — multi-year, sticky design commitments. (2) AI clusters at 100K GPU scale require entirely new networking infrastructure (Arista 800G switching, Coherent transceivers, Credo AEC cables).

### Custom Silicon — HOLDS (and counter-cyclical to capex anxiety)

| Assumption | Under Stress | Assessment |
|---|---|---|
| Hyperscalers committed to custom silicon programs (3-5 year cycles) | Mid-cycle design programs don't stop due to quarterly capex sentiment | **Holds** |
| Custom silicon provides 40-70% cost savings vs. Nvidia | Under AI capex budget pressure, the cost savings argument STRENGTHENS | **Strengthens** |
| Broadcom and Marvell are the dominant design partners | No near-term change to hyperscaler silicon relationships | **Holds** |

This is the most counter-intuitive element of the stress test: **capex deceleration anxiety is actually a tailwind for custom silicon.** If hyperscalers need to justify every dollar of AI infrastructure spend, owning their own silicon (vs. paying Nvidia's premium) becomes more economically compelling, not less. Google TPU, Amazon Trainium, Microsoft Maia — these programs get *more* strategic urgency when overall AI budgets face scrutiny.

**Broadcom's $16B Q3 guide vs. $17.2B estimate was a disappointment at the margin, but $16B in a single quarter of custom AI chip revenue is still staggering.** The thesis is intact; the market was priced for more.

### AI Networking — MODERATES

| Assumption | Under Stress | Assessment |
|---|---|---|
| AI cluster buildout pace drives new switch/transceiver demand | At 20-25% capex growth, cluster adds decelerate proportionally | **Moderates** |
| 800G → 1.6T upgrade cycle provides recurring demand | Bandwidth upgrade cycles are driven by cluster efficiency needs, not just new builds | **Partially holds** |
| Arista dominates AI Ethernet switching | Market position unchanged | **Holds** |
| Credo AEC is a new market being created | New market creation always at risk if the underlying GPU cluster buildout slows | **At risk** |

Arista (ANET) at 22% below ATH with a consensus PT of $186 is the most interesting situation here. The stock is correcting from a peak narrative, but the fundamental business (AI Ethernet switching) continues to grow — just at the pace of new cluster builds, which at 20-25% capex growth is still double-digit expansion. The vault holds a Buy at $185; the selloff may create that entry.

Coherent (COHR) and Credo (CRDO) are more exposed — the vault already has both at Hold. That rating is confirmed, not changed.

### Verdict
**Split.** Custom silicon (AVGO, MRVL): thesis holds and may be strengthened by the cost-efficiency imperative. Networking (ANET, COHR): thesis intact but growth rate moderates. CRDO: most exposed; Hold confirmed with elevated monitoring.

---

## Cross-Thesis Synthesis — What This Tells You

Three structural observations emerge from stress-testing all five theses together:

**1. Equipment companies have a time buffer; memory and storage names don't.**
LRCX, AMAT, KLAC have 6-18 month revenue lag from orders. Their 2026 results are largely protected. Memory (MU, SNDK) and storage (STX, WDC) have more direct exposure to current pricing and demand — any deceleration shows up in the next quarter, not the next year.

**2. The "per-wafer intensity" argument is the most durable element across all theses.**
Every thesis that relies on *architecture complexity growing regardless of volume* (HBM etch steps increasing per generation, CoWoS interposer processing, logic GAA transistors) is more resilient than theses that rely on *volume continuing to accelerate.* This means LRCX/AMAT are more durable in a deceleration than the memory manufacturers themselves.

**3. Custom silicon is the contrarian bright spot.**
In every other sub-thesis, capex deceleration is neutral-to-negative. For custom silicon (AVGO, MRVL), it's arguably a positive catalyst — the more hyperscalers need to justify their AI spending, the more they need Trainium and TPU economics vs. Nvidia H100 economics. This is the one area where the macro anxiety creates a direct fundamental tailwind.

---

## Recommended Thesis Updates

| Thesis | Current Status | Recommended Change |
|---|---|---|
| HBM Supply Constraint | Active / High | **Maintain** — add "watch SK Hynix/Samsung capex guidance" as primary signal |
| Memory Bottleneck | Active / High | **Downgrade to Medium conviction** — NAND pricing premium is directly at risk |
| WFE Supercycle | Active / High | **Maintain, note 2027+ uncertainty** — add book-to-bill as required monitoring metric |
| Advanced Packaging Bottleneck | Active / High | **Downgrade to Medium; flag for potential archiving** — bottleneck is resolving; fold into WFE Supercycle |
| AI Networking & Custom Silicon | Active / High | **Split into two sub-theses at different conviction levels** — Custom Silicon: High; Networking: Medium |

---

## Key Signals to Monitor (Master List)

| Signal | Source | Frequency | What It Tells You |
|---|---|---|---|
| SK Hynix / Samsung HBM capex guidance | Earnings calls | Quarterly | Whether memory OEMs are cutting WFE spending |
| LRCX / AMAT / KLAC book-to-bill | Earnings releases | Quarterly | Leading indicator of WFE 6-12 months forward |
| NAND spot price index | TrendForce | Monthly | Whether NAND pricing premium is holding |
| SNDK gross margins (Q4 FY2026, Aug 13) | Earnings | Next report Aug 13 | NBM contract durability + NAND cycle health |
| TSMC CoWoS utilization commentary | Earnings calls | Quarterly | Whether packaging bottleneck has cleared |
| Broadcom Q3 FY2026 AI revenue vs. $16B guide | Earnings (Sep 2026) | Next report | Custom silicon demand trajectory |
| Hyperscaler Q2 2026 capex — actual vs. guide | MSFT/GOOG/AMZN/META earnings (July 2026) | Quarterly | **The most important near-term datapoint** |

The last signal is the most critical. July 2026 hyperscaler earnings (Microsoft, Alphabet, Amazon, Meta all report in late July) will either confirm or challenge the capex deceleration narrative. If any hyperscaler *raises* their AI capex guide for 2026, it resets the entire narrative. If they all come in flat or light, today's repricing accelerates.

---

*Companion document: [[AI_Semi_Selloff_Analysis_2026-06-23]]*
