---
sector: Power-Gen-Grid
last_updated: 2026-06-03
tags: [sector]
---

# Power Generation & Grid — Sector Primer

---

## 1. Industry Overview

Data center electricity demand is the single largest structural change in US power markets in decades. Hyperscaler capex has shifted from "incremental load" to "system-defining load" in PJM, ERCOT, and MISO. The grid was built for ~1% annual demand growth; data centers alone could push this to 2–4%+ through the end of the decade.

Three sub-segments matter:
1. **Generation** — IPPs with nuclear/gas fleets positioned to sell to hyperscalers via 20-year PPAs
2. **Transmission & Distribution equipment** — transformers, switchgear, HVDC, cabling (supply-constrained; 2–5 year lead times)
3. **EPC / services** — grid buildout contractors (Quanta, MYR Group)

Key structural reality: every new AI data campus requires *both* the generation supply *and* the grid infrastructure to connect it. Companies that supply both (GEV) enjoy compounding demand.

---

## 2. AI/Energy Linkage

- **Demand:** AI training clusters run 100–500 MW each; a single hyperscaler campus can exceed 1 GW of continuous load. Unlike industrial demand, AI workloads run 24/7 at high utilization — they need *firm dispatchable* power, not intermittent renewables.
- **Nuclear PPAs:** Hyperscalers are signing 20-year contracts for nuclear baseload: CEG/Microsoft (Three Mile Island restart), VST/Meta (2,609 MW PJM), VST/AWS (1,200 MW ERCOT), GEV/Blue Energy (BWRX-300 SMR + gas hybrid, Texas, FID 2027). These re-price nuclear from commodity to contracted.
- **Gas turbines:** GEV's HA-class turbines are the only technology that meets hyperscaler power requirements at scale today. Gas turbine backlog + reservations hit 100 GW in Q1'26 (years ahead of schedule). Slot reservations extending to 2029+.
- **Transformer supply crunch:** Lead times extended from ~50 weeks to 120–180 weeks. Domestic US manufacturing capacity (GEV Prolec, ABB, Hitachi Energy) is sold out through 2027–2028. Every new data center requires large power transformers that are in severe shortage.
- **Interconnect queues:** PJM has multi-year backlogs. ERCOT processing has accelerated but remains a bottleneck. Interconnect queue delays are the primary risk to data center construction timelines.

---

## 3. Value Chain

```
Fuel (gas/uranium) → OEMs (GEV, Siemens) → Generators/IPPs → T&D Equipment → Data Center
                          ↑                        ↑               ↑
                  Turbines + Transformers      VST, CEG       Eaton, Hubbell, Quanta
```

**Margin concentration:**
- OEMs with backlog pricing power: GEV, Siemens Energy — sold-out production, new-price orders 10–20% above backlog
- IPPs with dispatchable baseload: VST, CEG — nuclear re-priced from commodity to contracted
- Grid equipment: ETN, HUBB, PWR — structural demand growth with favorable pricing

---

## 4. Competitive Landscape

| Company | Ticker | Sub-segment | Rating | Notes |
|---|---|---|---|---|
| GE Vernova | GEV | Gas turbines, grid equipment, SMRs | Buy | 100 GW gas backlog; Prolec transformers; BWRX-300 SMR |
| Vistra | VST | IPP (gas + nuclear, ERCOT + PJM) | Buy | Meta + AWS 20yr PPAs; Cogentrix acquisition |
| Constellation | CEG | IPP (largest US nuclear fleet) | — | TMI/Microsoft; pure nuclear premium valuation |
| NRG Energy | NRG | IPP (retail + generation, ERCOT) | — | No nuclear; growing data center retail exposure |
| Eaton | ETN | Electrical equipment, grid | — | Broad grid; data center power distribution leader |
| Quanta Services | PWR | Grid construction / EPC | — | Transmission and distribution construction |
| Hubbell | HUBB | T&D components | — | Grid infrastructure equipment |
| Siemens Energy | ENR.DE / SMNEY | Gas turbines, HVDC, offshore wind | — | Closest GEV comp; ~25x vs GEV's 35x EV/EBITDA |
| Modine | MOD | Data center thermal | — | See Cooling-Thermal primer |

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Where to Find |
|---|---|---|
| GEV gas turbine backlog + reservations | Primary demand signal for the sector; 100 GW Q1'26 → target 110 GW YE26 | GEV quarterly press releases |
| ERCOT peak demand vs. capacity | Determines VST/NRG summer earnings; structural floor rising with data center load | ERCOT.com operational data |
| PJM capacity auction clearing prices | Sets East segment revenue floor for VST/CEG | PJM Interconnection filings |
| Large power transformer lead times | Bottleneck signal for grid electrification pace | Utility Dive, EEI surveys |
| Interconnect queue volumes (PJM/ERCOT) | Demand signal for Quanta EPC work; also data center construction pace | FERC Form 706, PJM queue |
| Hyperscaler capex guidance (MSFT, META, AMZN, GOOGL) | Drives forward power demand; any reduction would be a headwind | Quarterly earnings calls |
| New gas PPA / nuclear PPA signings | Each deal converts commodity exposure to contracted; re-rates the sector | Press releases, 8-Ks |

---

## 6. Valuation Context

| Sub-segment | Typical Multiple | Current State |
|---|---|---|
| Nuclear IPP (contracted) | 14–18x EV/EBITDA | CEG at ~16x; VST nuclear fraction undervalued at 9.7x blended |
| Gas turbine OEM | 25–40x EV/EBITDA | GEV at ~35x; Siemens Energy at ~25x; premium to traditional industrial |
| Grid equipment (ETN, HUBB) | 18–25x EV/EBITDA | Supply-constrained; growing data center exposure supports premium |
| Grid EPC (PWR) | 20–25x EV/EBITDA | Backlog building; structural tailwind |

**Key valuation debate:** Is GEV (35x) justified vs. Siemens Energy (25x)? GEV has higher growth, U.S. listing premium, superior execution. Gap is real but magnitude warrants monitoring — any deceleration in order pace could compress the premium.

---

## 7. Key Theses Impacting This Sector

- [[Transformer Supply Crunch]] — lead times at 120–180 weeks; no meaningful new capacity before 2027
- [[Nuclear Renaissance via Hyperscaler PPAs]] — 20-year contracts converting nuclear from commodity to contracted
- [[Gas Turbine Backlog Pricing Power]] — oligopoly (GEV + Siemens + Mitsubishi) sold out through 2029; new-price orders 10–20% above backlog

---

## 8. Risks

1. **AI capex normalization** — if hyperscalers reduce data center investment, new order pace slows (backlog conversion is protected but future bookings moderate)
2. **State-level data center permitting pushback** — GEV CEO flagged in May 2026; more states resisting large data center siting
3. **Wind tariff uncertainty** — offshore wind project economics remain challenged; GEV's Wind segment drag persists
4. **ERCOT weather risk** — VST/NRG earnings are highly weather-sensitive; mild summers reduce Texas earnings
5. **Interconnect queue delays** — customers who have booked turbines may face permitting delays that push revenue recognition right
6. **Interest rates** — utilities and IPPs are rate-sensitive; rising rates compress equity valuations
7. **Commodity price volatility** — natural gas spikes affect IPP cost structures (partially offset by merchant power price correlation)

---

## 9. Data Sources

- EIA (Form 860, 923) — generation capacity by plant
- FERC filings — interconnect queue data, transmission investment
- PJM / ERCOT / MISO interconnect queues
- Edison Electric Institute (EEI) — capital expenditure surveys
- NERC reliability reports
- Company press releases and 8-Ks for PPA announcements
- Bigdata.com — earnings transcripts, news, analyst reports

---

## 10. Key Concept Links

- [[Interconnect Queue]] — why new generation capacity takes 5–7 years to connect
- [[Transformer Supply]] — why lead times are 120+ weeks and unlikely to normalize before 2028
- [[HBM]] — why AI chips require so much power (see Semi-Materials-Equip primer for context)
- [[Nuclear Renaissance via Hyperscaler PPAs]] — the thesis driving CEG, VST nuclear re-rating

---

## 11. On-Site Generation — The Grid-Bypass Sub-Sector (Added June 3, 2026)

AI data centers cannot wait years for grid interconnection. On-site generation technologies that bypass the queue are becoming a distinct sub-segment within Power-Gen-Grid:

| Company | Technology | AI Contract Scale | Coverage |
|---|---|---|---|
| Bloom Energy (BE) | Solid oxide fuel cells | Oracle 2.8GW + Nebius $2.6B | [[BE]] — Buy/$330 |
| Caterpillar (CAT) | Gas generator sets | 2GW order; $51B backlog +71% | [[CAT]] — Buy/$1,000 |
| Generac (GNRC) | Standby/prime generators | $700M DC backlog | [[GNRC]] — Buy/$320 |
| FuelCell Energy (FCEL) | Molten carbonate fuel cells | AI data center pitch | Research |

**Key thesis:** [[Fuel Cells and On-Site Power]]
