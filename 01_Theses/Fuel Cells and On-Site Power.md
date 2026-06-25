---
status: Active
conviction: High
last_updated: 2026-06-03
tags: [thesis]
---

# Fuel Cells and On-Site Power — Bypassing the Grid

> The US grid interconnection queue has multi-year backlogs. A data center applying for grid connection today may wait 3-7 years. On-site generation — fuel cells (Bloom Energy), gas generator sets (Caterpillar, Generac), and modular power plants — bypasses this queue entirely. Hyperscalers are paying significant premiums for the time advantage. This is the thesis Aschenbrenner's Situational Awareness fund built its largest position around.

---

## The Core Problem

Every new AI data center needs megawatts of reliable power. Hyperscalers have the money to build — but they cannot get the power in time. The US interconnection queue (PJM, ERCOT, MISO, WECC) now totals over 2,000 GW of requests against a grid that adds ~50 GW of new generation annually. In PJM alone, a new generator requesting interconnection today faces a 5-7 year queue.

The math is brutal for hyperscalers:
- Nvidia B200 clusters consume 120 kW per rack × 1,000 racks = 120 MW per campus
- A hyperscaler building 10 AI campuses per year needs 1,200 MW of new power annually
- At 5-7 year grid interconnection timelines, they'd need to apply for capacity in 2019-2021 to get power by 2026-2028

The solution is **on-site generation** — power generated at the data center site, reducing or eliminating grid dependence.

---

## Technology Map

| Technology | Provider | Power Range | Deployment Time | Carbon Profile |
|---|---|---|---|---|
| Solid oxide fuel cells | Bloom Energy (BE) | 1 MW - GW | 12-18 months | Low (natural gas); zero-carbon (hydrogen/biogas) |
| Reciprocating gas engines | Caterpillar (CAT) | 500 kW - 10+ MW | Weeks-months | Moderate (natural gas combustion) |
| Standby/prime generators | Generac (GNRC) | 5 kW - 10 MW | Weeks | Moderate (diesel/natural gas) |
| PEM fuel cells | Plug Power (PLUG) | 100 kW - MW | 6-12 months | Varies (hydrogen source dependent) |
| Combined Heat & Power | Multiple | 1-100+ MW | 12-24 months | Efficient (waste heat capture) |
| Modular nuclear (SMR) | GEV Hitachi, NuScale | 77-300 MW | 5-8 years | Zero-carbon | 

**Near-term winners:** Bloom, CAT, and Generac — technologies deployable in months to 18 months. SMRs remain a 2030+ story.

---

## Evidence of Hyperscaler Adoption

**Bloom Energy (BE):**
- Oracle: Up to 2.8 GW for Project Jupiter AI data centers
- Nebius: $2.6B, 10-year, 328 MW agreement
- Backlog: $20B (product + service contracts)
- Revenue: $751M Q1'26 (+130% YoY)

**Caterpillar (CAT):**
- American Intelligence & Power Corp: 2 GW gas generator sets, delivered Sept 2026-Aug 2027
- Microsoft-Nvidia: Named infrastructure partner for AI campus
- Joule project (Utah): CAT G3520K generators powering AI campus
- Company backlog: $51B entering 2026, +71% YoY

**Generac (GNRC):**
- $700M data center product backlog
- "Final stages of vendor approval with multiple hyperscale customers"
- C&I segment sales: +28% YoY from data centers
- Full-year 2026 guidance raised

---

## The Pricing Paradox

All three companies are priced as industrial equipment businesses, not as AI infrastructure companies:
- BE trades at fuel cell company multiples (historically 20-50x)
- CAT trades at industrial equipment multiples (~20-25x)
- GNRC trades at industrial equipment multiples (~20x)

The AI infrastructure sector (data center REITs, GPU cloud) trades at 25-40x EV/EBITDA. As data center power generation becomes recognized as AI infrastructure — not industrial equipment — these multiples should converge.

**The Bloom Energy example:** BE re-rated from ~$80 (industrial fuel cell company) to $291+ (AI infrastructure company) as the Oracle and Nebius contracts established the new customer archetype. CAT and GNRC are at earlier stages of the same re-rating process.

---

## Investment Implications

| Company | Current Framing | Target Framing | Rating |
|---|---|---|---|
| [[BE]] | Fuel cell company | AI power infrastructure | Buy/$330 |
| [[CAT]] | Mining/construction equipment | AI power infrastructure + industrial | Buy/$1,000 |
| [[GNRC]] | Residential/C&I generators | AI data center power | Buy/$320 |

---

## Risks

1. **Grid expansion accelerates:** If US permitting reform allows faster grid interconnection, the urgency for on-site generation decreases
2. **Natural gas price spikes:** High gas prices make on-site generation expensive vs. grid power
3. **Hydrogen economics:** For clean on-site power, green hydrogen fuel costs remain uncompetitive vs. grid clean power at scale
4. **Technology displacement:** If storage + renewables enable reliable on-site clean power at lower cost, fuel cells lose their advantage

---

## Review Note (2026-06-23)

Thesis reviewed against AI capex deceleration scenario. **Partially counter-cyclical.**

The interconnection queue problem (2,000+ GW of requests, 5-7 year waits) is structural and does not shrink if AI capex decelerates — it shrinks if permitting reform passes or generation capacity is added, neither of which is imminent. If hyperscalers become more selective about which data centers to build, they will prioritize sites where power is available *now* — precisely the use case for Bloom/CAT/GNRC on-site generation. Capex deceleration may therefore redirect AI infrastructure spending *toward* on-site power rather than away from it.

Existing backlogs are enormous and multi-year: BE $20B, CAT $51B. Revenue visibility is high regardless of near-term sentiment.

The multiple re-rating thesis (industrial → AI infrastructure multiples) may proceed more slowly in a deceleration environment, but the fundamental earnings trajectory is insulated. **Conviction maintained at High.** No changes needed.

---

## Change Log
- `2026-06-03` — Thesis created. Evidence base: Bloom Energy contracts (Oracle, Nebius), Caterpillar SEC filings, Generac earnings, Aschenbrenner portfolio research.
- `2026-06-23` — Reviewed under AI capex deceleration. Thesis intact; partially counter-cyclical. No rating changes.
