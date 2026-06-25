---
status: Active
conviction: High
last_updated: 2026-06-23
tags: [thesis]
---

# Liquid Cooling Mass Adoption

> Air cooling fails above ~40 kW per rack. Nvidia's Blackwell GB200 NVL72 dissipates 120 kW per rack. This is not a preference — it is a physics constraint. Every frontier AI training cluster deployed from 2025 onward requires liquid cooling infrastructure, creating a structural, non-reversible demand step-up for Vertiv, Modine, and the broader thermal management supply chain.

---

## The Core Thesis

Data centers have been air-cooled since IBM introduced the first commercial mainframe in 1952. Air cooling has scaled from 1 kW/rack to ~40 kW/rack over seven decades — a 40x improvement driven by better airflow design, higher fan speeds, and more efficient CRAC (Computer Room Air Conditioning) units.

It cannot scale further for AI workloads. The GB200 NVL72 — Nvidia's current flagship AI system — draws 120 kW per rack. Air simply cannot remove heat at that density without creating hot spots that throttle GPU performance. Liquid cooling is not optional for frontier AI infrastructure; it is mandatory.

This creates an irreversible demand inflection. Every new hyperscaler AI cluster requires direct liquid cooling infrastructure — cold plates, coolant distribution units (CDUs), secondary cooling loops, and facility-level chillers. The installed base of air-cooled data centers may persist for general compute, but all incremental AI capacity goes liquid.

---

## The Physics Constraint

Air cooling capacity (kW per rack) is constrained by:
1. **Airflow volume:** Limited by fan power and noise
2. **Air heat capacity:** Air has very low specific heat (1.005 J/g·K vs. water at 4.18 J/g·K)
3. **Temperature delta:** Data centers must maintain 18-27°C air inlet; coolant loops can operate at 40-60°C, dramatically increasing the usable temperature delta

Water's heat capacity is 4x that of air, and liquid cooling can operate at far higher differential temperatures. This means a CDU with modest fluid flow can remove 10-20x more heat than an equivalent air handling unit, in a fraction of the floor space.

ASHRAE's TC 9.9 (Thermal Guidelines for Data Processing Environments) defines the boundary: beyond A3 class (40 kW/rack), air cooling is no longer practical. AI GPU racks crossed this threshold in 2023. Next-generation AI systems (Rubin, Blackwell Ultra) will be at 200+ kW/rack.

---

## Technology Map

| Cooling Method | Max Rack Power | Penetration (2026E) | Growth Trajectory |
|---|---|---|---|
| Air (CRAC/CRAH) | ~40 kW | ~65% of installed base | Declining share of new builds |
| Rear-door HEX | ~60 kW | ~10% | Stable (retrofit only) |
| Direct liquid cooling (cold plate + CDU) | ~120 kW | ~20% of new AI builds | Fastest growing; mandatory for GB200 |
| Full immersion | 100 kW+ | <5% | Early commercial; growing |

The secular shift: as GPU generations advance (Blackwell → Rubin → next), density requirements escalate and liquid cooling penetration increases. This curve is steep and one-directional.

---

## Market Size and Growth

The data center liquid cooling market was ~$3-4B in 2023 and is projected to exceed $15-20B by 2030, a ~20-25% CAGR. This growth is driven entirely by the AI density inflection — general-purpose compute does not require liquid cooling.

Key market segments:
- **CDUs (coolant distribution units):** The primary system component; routes coolant from facility-level chiller to rack-level cold plates
- **Cold plates:** Directly attach to GPU/CPU; highest precision component
- **Facility chillers:** Reject heat from CDU secondary loop to ambient; traditional HVAC market expanding
- **Services and commissioning:** Highest-margin segment; growing as operators need ongoing system management

---

## Investment Implications

| Company | Liquid Cooling Position | Notes |
|---|---|---|
| [[VRT]] | **Full-stack leader** — CDUs, power distribution, IT infrastructure, services | Backlog ~$15B; orders +252% YoY in Q4'25; CEO: "infrastructure density increases and deployment timelines compress" |
| [[MOD]] | **Fastest-growing mid-cap** — data center thermal management primary growth driver | Revenue +226% YoY; consensus PT $358 vs. stock $302 |
| [[TT]] | **Facility-level cooling** — chillers and HVAC; data center ~25% of revenue | Diversified; less pure than VRT/MOD |
| [[NVT]] | **Mixed exposure** — thermal management segment growing; enclosures primary business | Growing liquid cooling product line; less pure-play |
| [[SPXC]] | **Indirect** — cooling towers used in facility-level heat rejection | Less direct exposure to liquid cooling specifically |

---

## Why VRT Is the Canonical Expression

Vertiv is unique in covering the full thermal management stack: power distribution (PDUs, UPS), thermal management (CDUs, chillers, cold plates), IT infrastructure (racks, KVM), and lifecycle services. No other public company offers this combination at scale.

This integrated position matters because hyperscalers are moving from component procurement to system-level procurement — they want one vendor to design, deliver, and service the complete data center power and cooling infrastructure. Vertiv's "grid to chip" offering (including the Boyd Thermal acquisition for white-space liquid cooling) positions it for this transition.

VRT Q1'26: Americas organic sales +44%, adj. operating margin 20.8% (+430 bps YoY). Management guided 30% organic revenue growth and 51% EPS growth for 2026. CEO Albertazzi: "As infrastructure density increases and deployment timelines compress, we're positioned to be the partner customers need to bring their most ambitious projects to life, at scale."

---

## Duration and Risks

**Duration:** The GPU density escalation trend is driven by fundamental semiconductor physics (transistor density improvements, power wall) and AI model scaling laws. This is a 5-10 year structural trend, not a cyclical uptick.

**Risks:**
1. **Hyperscaler capex digestion:** If AI build rates slow in 2027-2028, liquid cooling order books compress with a 6-12 month lag
2. **Immersion leapfrog:** If full immersion achieves mainstream penetration faster than expected, vendors without strong immersion portfolios face share loss (Vertiv is building immersion capability)
3. **Commoditization:** Cold plates could become commodity components; value shifts to systems integration and services
4. **Customer concentration:** Top 4 hyperscalers = majority of VRT/MOD orders

---

## Stress-Test Note (2026-06-23)

Applied AI capex deceleration scenario (75% → 20-25% YoY growth). Key findings:

**Why this thesis is structurally different from HBM/WFE:** The demand driver is physics, not volume acceleration. A 120 kW rack requires liquid cooling regardless of how many racks are being deployed — ASHRAE A3 class (40 kW) is a hard ceiling for air. At 20-25% capex growth, fewer new clusters are deployed per year, but every single new cluster still mandates liquid cooling. The direction is unambiguous; only the pace changes.

**The order normalization risk (most important):** VRT's Q4'25 orders came in at +252% YoY — historically extraordinary and mathematically unsustainable. When Q2'26 orders are reported and comp against that level, even a healthy 40-60% YoY figure will look like a sharp deceleration. The market is likely to misread this as AI capex deterioration. This is a **stock risk, not a thesis risk** — but it's real and worth being prepared for.

**Retrofit demand is an underappreciated floor:** The ~65% of installed base still on air cooling represents a multi-decade retrofit opportunity (rear-door HEX, then full liquid conversion) that is largely independent of new cluster buildout pace.

**Conviction: Maintained at High.** No rating change. See [[Thesis_Stress_Test_2026-06-23]].

---

## Change Log

- `2026-06-03` — Thesis created. Evidence base: VRT Q1'26 earnings, Investor Day May 2026, RBC research notes, ASHRAE thermal standards.
- `2026-06-23` — Stress-tested under AI capex deceleration scenario. Conviction maintained at High. Order normalization risk added explicitly.
