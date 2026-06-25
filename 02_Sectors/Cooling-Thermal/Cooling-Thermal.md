---
sector: Cooling-Thermal
last_updated: 2026-06-03
tags: [sector]
---

# Cooling & Thermal Management — Sector Primer

---

## 1. Industry Overview

The shift from air cooling to liquid cooling is the most consequential hardware transition in the data center industry. GPU rack densities have moved from ~15 kW/rack (CPU era) to 60–120+ kW/rack (GB200/Blackwell era) — air cooling breaks down above ~40 kW/rack, making liquid cooling mandatory for frontier AI training and inference infrastructure.

This is not a cyclical trend or a speculative thesis. It is a physics constraint. Nvidia's Blackwell GB200 NVL72 rack (a 72-GPU system) dissipates up to 120 kW per rack and requires liquid cooling by design. Every hyperscaler building AI clusters must deploy liquid cooling — there is no air-cooled alternative.

Sub-segments:
1. **Direct liquid cooling (DLC)** — cold plates on CPUs/GPUs + CDUs (coolant distribution units); highest growth; required for frontier AI
2. **Rear-door heat exchangers** — retrofit solution for existing air-cooled facilities; moderate growth
3. **Immersion cooling** — submerging hardware in dielectric fluid; highest density, early-stage commercial deployment
4. **Facility-level** — chillers, air handlers, cooling towers (still growing because total compute grows faster than cooling efficiency gains)

---

## 2. AI/Energy Linkage

- Every new Nvidia GB200, AMD MI300X, or Google TPU v5 deployment requires direct liquid cooling infrastructure
- Typical GB200 NVL72 rack: 120 kW. At 100 racks per MW of data center: 12 MW of cooling load from GPUs alone
- The "pick and shovel" framing is apt: regardless of which AI company wins, all frontier AI requires thermal management
- Vertiv (VRT) management has called cooling orders the "canary in the coal mine" for hyperscaler capex — orders lead revenue by 6–12 months
- Cooling represents ~30–40% of total data center capital cost in liquid-cooled facilities

**Key data points:**
- VRT backlog and book-to-bill ratio are the cleanest real-time signals for AI infrastructure capex pace
- Management at VRT, Modine, and SPX consistently cite 3–5 year visibility on data center cooling demand
- ASHRAE standards for Thermal Guidelines for Data Processing Environments define the framework that makes liquid cooling mandatory above 40 kW/rack

---

## 3. Value Chain

```
Components (pumps, cold plates, manifolds) → CDU/system integrators → Hyperscaler/colo installation
        ↑                                              ↑
  Specialty manufacturers                    Vertiv, Modine, SPX
  (Parker, Alfa Laval, etc.)               (full system vendors)
  
Facility-level cooling:
Chillers (Trane, Carrier, York) → Cooling Towers (SPX) → Computer Room ACs (VRT, Stulz)
```

**Where value concentrates:** Full-stack providers who can supply both the rack-level CDU and the facility-level chiller integration (Vertiv). Systems integration capability commands premium margins over component suppliers.

---

## 4. Competitive Landscape

| Company | Ticker | Sub-segment | Notes |
|---|---|---|---|
| Vertiv | VRT | Full-stack (power + cooling + management) | Clear leader; AI data center pure-play; orders transparency makes it the bellwether |
| Modine Manufacturing | MOD | Data center thermal; growing share | HPC/AI-focused; smaller but fastest growth rate in sub-sector |
| Trane Technologies | TT | Chillers, HVAC, facility-level cooling | Diversified; data center is ~25% of revenue and growing |
| SPX Technologies | SPXC | Cooling towers, HVAC components | More utility-oriented; data center exposure is indirect |
| nVent Electric | NVT | Enclosures, precision cooling, thermal mgmt | Growing liquid cooling exposure; smaller data center fraction |
| Schneider Electric (unlisted) | — | UPS, data center infrastructure management | Private competitor to VRT's power management |
| Huawei/ZTE (unlisted) | — | China-based cooling solutions | Restricted in US/EU markets |

**Vertiv's lead:** VRT is the only publicly traded company where data center thermal + power management is the *core* business (~85%+ of revenue). This makes VRT the cleanest AI infrastructure proxy in the cooling sub-segment.

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Source |
|---|---|---|
| VRT orders growth and book-to-bill | Leads revenue by 6–12 months; best real-time AI capex signal | VRT quarterly earnings |
| VRT backlog | Multi-year demand visibility; growing from $6B to $10B+ range | VRT press releases |
| Data center liquid cooling penetration (% of new builds) | Secular shift metric; currently ~20–30% of new capacity; heading toward 60–70% | Uptime Institute surveys |
| Nvidia GPU shipment pace (H100, B200, GB200) | Each GPU requires CDU capacity; Nvidia's production = VRT's future orders | NVDA supply chain commentary |
| Hyperscaler CapEx guidance (MSFT, META, AMZN, GOOGL) | Aggregate demand signal | Quarterly earnings calls |
| VRT/MOD gross margin trends | Pricing power test; supply-constrained market should sustain margins | Quarterly P&L |
| Cooling tower orders (SPXC) | Lagging indicator — utility and large facility cooling |  SPXC quarterly |

---

## 6. Valuation Context

| Company | EV/EBITDA (NTM) | Revenue Growth (NTM) | Data Center % | Notes |
|---|---|---|---|---|
| Vertiv (VRT) | ~25–30x | ~15–20% | ~85% | Premium AI infrastructure multiple |
| Modine (MOD) | ~15–20x | ~15–20% | ~60% (and growing) | Discount to VRT; smaller scale |
| Trane (TT) | ~22–25x | ~8–12% | ~25% | Conglomerate discount vs. pure-play |
| SPX (SPXC) | ~18–20x | ~8–10% | <20% | More utility/industrial |
| nVent (NVT) | ~18–22x | ~8–12% | ~30% | Mixed exposure |

**Key valuation debate:** VRT's premium (25–30x) is justified by AI pure-play purity and orders visibility. The question is whether the multiple holds through a capex digestion period. VRT bull case: orders continue accelerating as GB200 and next-gen GPU ramps require even more cooling density. VRT bear case: hyperscaler build pace slows in 2027-2028 digestion period, compressing order growth and multiple simultaneously.

---

## 7. Key Theses

- **Liquid Cooling Mass Adoption** — physics makes liquid cooling mandatory above 40 kW/rack; each new GPU generation pushes density higher; adoption curve is steep and non-reversible
- **Vertiv as the Pure-Play** — no comparable public company offers full-stack data center power + cooling + management at VRT's scale
- **Modine as the catch-up play** — smaller, faster-growing, trades at discount to VRT with similar secular tailwinds

---

## 8. Sub-Segment Deep Dive: Liquid Cooling Technologies

| Technology | Rack Density Support | Current Penetration | Key Vendors | Notes |
|---|---|---|---|---|
| Air cooling (CRAC/CRAH) | Up to ~40 kW/rack | ~70% of installed base | VRT, Stulz, Schneider | Declining in new AI builds |
| Rear-door HEX | Up to ~60 kW/rack | ~10% of installed | VRT, Coolcentric | Retrofit; extends air cooling life |
| Direct liquid cooling (DLC) | Up to ~120 kW/rack | ~15–20% of new builds | VRT, Modine, Airedale | Fastest growing; GB200-required |
| Full immersion | 100 kW+/rack | <5% of installs | GRC, LiquidCool, Submer | Highest density; complex; growing |

The secular trend is clear: as GPU generations advance, each successive generation requires higher rack density and forces a step-up in cooling technology. Nvidia's roadmap (Blackwell → Rubin → next) implies continued density escalation through at least 2028.

---

## 9. Risks

1. **Hyperscaler capex digestion** — the primary risk; if hyperscalers pause or slow building in 2027-2028, the cooling order book compresses
2. **Commoditization** — cold plates and CDUs could become commodity as more manufacturers enter; VRT's moat is systems integration and service relationships
3. **Technology shift to immersion** — if immersion cooling achieves mainstream penetration faster than expected, vendors without immersion portfolios face share loss
4. **Customer concentration** — top 4 hyperscalers (MSFT, META, AMZN, GOOGL) = majority of VRT/MOD orders; any single customer slowdown is material
5. **Manufacturing capacity** — lead times are extended; VRT has invested in capacity, but supply chain constraints (copper, specialty components) can create delivery delays

---

## 10. Data Sources

- Uptime Institute Annual Global Data Center Survey
- Dell'Oro Group data center capex forecasts
- ASHRAE Technical Committees (TC 9.9) — thermal standards
- Hyperscaler capex disclosures in quarterly earnings
- VRT quarterly earnings and investor presentations (most informative public data on the sector)
- Bigdata.com — earnings transcripts, news, analyst reports
