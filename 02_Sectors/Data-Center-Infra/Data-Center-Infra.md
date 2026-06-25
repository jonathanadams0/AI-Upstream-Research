---
sector: Data-Center-Infra
last_updated: 2026-06-03
tags: [sector]
---

# Data Center Infrastructure — Sector Primer

> Data centers are the physical manifestation of AI. Every training run, every inference call, every model weight exists inside a building full of servers, cooling systems, and power distribution. The companies that own those buildings, or provide the critical infrastructure within them, are playing one of the most durable roles in the AI buildout.

---

## 1. Industry Overview

Data center infrastructure encompasses the physical layer of AI compute: the real estate, power, connectivity, and auxiliary services that house the servers. This sector has three main archetypes:

1. **Data Center REITs** — Own and operate data center facilities globally, leasing space (colocation) or dedicated capacity to hyperscalers, enterprises, and cloud providers. Revenue model: long-term leases (5-15 year terms) plus metered power. EQIX (colocation focus), DLR (wholesale + colocation), IRM (hybrid — document storage + data centers).

2. **Hyperscale Campus Developers** — Build entire campuses for a single hyperscaler on a long-term lease. The hyperscaler owns the IT equipment; the developer owns the real estate. IRM, DLR, and private players (QTS, CyrusOne, Aligned) all compete here.

3. **GPU Cloud / Infrastructure-as-a-Service** — Companies that own GPU clusters and rent them to AI developers by the hour or by the chip. CoreWeave (CWAI, recently IPO'd) is the most prominent pure-play; also includes Lambda Labs, Coreweave, and portions of AWS/Azure/GCP.

---

## 2. AI/Infrastructure Linkage

**Supply shortage:** Data center capacity — particularly power — is the most acute constraint on AI expansion. Hyperscalers can order GPUs; they cannot always get them powered. PJM, ERCOT, and MISO have multi-year interconnection queues. New data center campuses in Virginia, Texas, and Ohio are constrained by grid capacity.

**Colocation demand:** AI compute requires specialized facilities: higher power density (120+ kW/rack vs. 10-15 kW/rack for conventional), liquid cooling infrastructure, and redundant power. EQIX and DLR are retrofitting existing colocation facilities and building new AI-spec campuses.

**IRM's pivot:** Iron Mountain began life as a document storage company (paper records, physical media). Over the past 5 years it has been building and acquiring data centers, particularly targeting hyperscaler co-location demand. IRM's data center segment is now 30%+ of revenue and growing at 30%+ annually — a structural transformation the market has been slow to price.

**GPU cloud emergence:** CoreWeave (IPO'd early 2025) rents Nvidia H100/H200/B200 GPUs to AI startups and enterprises. CoreWeave has long-term Nvidia GPU supply commitments and Microsoft as a major customer. It represents the "pick and shovel" of the AI inference layer — every AI application that doesn't run on a hyperscaler runs on CoreWeave or similar GPU cloud providers.

---

## 3. Value Chain

```
Land acquisition + permitting
        ↓
Data center design + construction (Turner, Mortenson — private)
        ↓
Power procurement + grid interconnection (utilities, transmission)
        ↓
Cooling infrastructure (Vertiv, Modine — see Cooling-Thermal)
        ↓
Facility operations (EQIX, DLR, IRM — or hyperscaler owned)
        ↓
Tenant: hyperscaler, cloud provider, or GPU cloud operator
```

---

## 4. Competitive Landscape

| Company | Ticker | Business Model | AI Angle |
|---|---|---|---|
| Equinix | EQIX | Global colocation REIT | AI workloads + interconnection hubs; 260+ IBX data centers |
| Digital Realty | DLR | Wholesale + colo REIT | Hyperscale AI campus development; 300+ data centers |
| Iron Mountain | IRM | Document storage + data centers | Fastest-growing DC segment; unique legacy real estate assets |
| CoreWeave | CWAI | GPU cloud / IaaS | Pure-play GPU rental; MSFT as anchor tenant; Nvidia partnership |
| QTS Realty | Private (Blackstone) | Hyperscale REIT | Major hyperscaler campus developer |
| CyrusOne | Private (KKR) | Hyperscale REIT | Growing hyperscale footprint |

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Source |
|---|---|---|
| EQIX same-store revenue growth + new bookings | Organic demand signal | EQIX quarterly |
| DLR backlog and pre-leased percentage | Forward demand visibility | DLR quarterly |
| IRM data center revenue growth | Pivot validation | IRM quarterly |
| CWAI GPU utilization rate | AI cloud demand vs. supply | CoreWeave earnings |
| Data center power pipeline (MW) | Long-lead demand indicator | Company investor days |
| Data center vacancy rates (major markets) | Supply/demand balance | CBRE/JLL research |
| PUE (Power Usage Effectiveness) | Efficiency benchmark; AI facilities target 1.2-1.3 | Company disclosures |

---

## 6. Valuation Context

| Company | EV/EBITDA | Dividend Yield | Notes |
|---|---|---|---|
| EQIX | ~25-28x | ~2.0% | Premium REIT; global interconnection moat |
| DLR | ~20-22x | ~2.8% | Wholesale focus; AI campus development option |
| IRM | ~18-20x | ~2.5% | Discount to pure-play DCs; document storage drag |
| CWAI | NM (pre-profit) | None | Pure-play GPU cloud; valued on revenue growth |

**Key REIT note:** Data center REITs are rate-sensitive (like all REITs) but their AI-driven demand growth can partially offset rising rates. The key underappreciated factor is that AI data center leases are significantly more expensive per square foot than conventional IT leases — driving same-store revenue growth even without occupancy gains.

---

## 7. Why IRM Is the Most Interesting

Iron Mountain is the most contrarian position in this sector. The market still prices IRM like a document storage company (slow growth, low multiples) while the actual data center business is growing 30%+ annually. Key advantages:
- **Existing real estate footprint:** IRM owns hundreds of warehouse and storage facilities globally that can be repurposed as data centers — avoiding the years-long permitting process for greenfield sites
- **Power access:** IRM's existing facilities often have utility service already established — a significant time-to-market advantage
- **Government/regulated-sector relationships:** IRM has deep relationships with government, healthcare, and financial services clients who now need AI data center capacity

---

## 8. Risks

1. **Interest rate sensitivity:** REITs rely on debt financing; rising rates increase cost of capital and compress cap rates
2. **Hyperscaler vertical integration:** Microsoft, Google, and Amazon are increasingly building their own campuses, reducing dependence on third-party REITs
3. **Power procurement delays:** Grid interconnection queues and permitting delays can slow new data center development
4. **CoreWeave GPU cloud risk:** CoreWeave has significant leverage to Nvidia GPU pricing and Microsoft renewal decisions
5. **Market concentration:** Northern Virginia (Ashburn) is the largest data center market; regulatory or infrastructure issues there have outsized impact

---

## 9. Data Sources

- CBRE / JLL data center market reports
- Company quarterly earnings (EQIX, DLR, IRM, CWAI)
- NAREIT data center REIT sector data
- Cushman & Wakefield data center market research
- Bigdata.com — earnings transcripts

---

## 10. Miners to AI Hosts — The Pivot Sub-Sector (Added June 3, 2026)

Bitcoin miners pivoting to GPU/HPC hosting represent a distinct sub-segment: existing power infrastructure + industrial real estate repurposed for AI compute.

| Company | MW Contracted (AI) | Status | Coverage |
|---|---|---|---|
| Core Scientific (CORZ) | 590 MW (CoreWeave) | Being acquired by CoreWeave | [[CORZ]] — Under Review |
| Applied Digital (APLD) | Growing | Independent AI data center | [[APLD]] — Buy/$60 |
| IREN Limited (IREN) | Growing | GPU cloud revenue | [[IREN]] — Hold/$72 |
| CleanSpark (CLSK) | Early | Still mining-heavy | Not rated |
| Riot Platforms (RIOT) | Early | Mining-focused | Not rated |

**Key thesis:** [[Miners to AI Hosts]]

Also in this sector: Lumentum (LITE) and Fabrinet (FN) moved to [[AI-Networking]] primer.
