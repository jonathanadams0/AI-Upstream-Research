# AI Upstream Research Vault

Equity research vault mapping the full AI infrastructure stack — from electricity generation to chip manufacturing to data center real estate. 8 sectors, 58 rated companies, 16 theses.

**Coverage universe:** 58 rated companies (as of 2026-06-09) | **Active theses:** 16 | **DCF models:** 5 | **Sectors:** 8

> Counts in this README are snapshots. The Dataview tables in `00_Dashboard/Dashboard.md` are the source of truth.

> **Disclaimer:** Personal research project for educational purposes. All portfolios here are **hypothetical paper books** — nothing in this vault is investment advice, a recommendation, or a solicitation, and it does not reflect real positions or trading. Data is drawn from public filings and third-party feeds and may contain errors. See [DISCLAIMER.md](DISCLAIMER.md).

---

## Quick Start

1. **Open this folder as an Obsidian vault** (Obsidian → Open folder as vault)
2. **Install community plugins** (Settings → Community Plugins → Turn on):
   - **Dataview** — powers the dashboard auto-generated tables. Required.
   - **Templater** — one-click new company/sector notes. Recommended.
3. **Enable in Dataview settings:** "Enable JavaScript Queries" and "Enable Inline JavaScript Queries"
4. **Set Templater template folder** to `99_Templates`
5. Open `00_Dashboard/Dashboard.md` — if the tables render with data, Dataview is working.

---

## Vault Structure

| Folder | Contents | Status |
|---|---|---|
| `00_Dashboard/` | Coverage tracker, Portfolio Summary, to-do list | Live |
| `01_Theses/` | 16 investment theses (all sectors covered) | Complete |
| `02_Sectors/` | 8 sector primers with competitive maps | Complete |
| `03_Companies/` | 58 company notes + 13 briefs/prep files | All rated |
| `04_Models/` | 5 DCF models (GEV v7, VST v1, CEG v1, NRG v1) | Active |
| `05_Sources/` | Aschenbrenner analysis, earnings notes | Active |
| `06_Concepts/` | 17 concept/glossary notes + screener runs | Complete |
| `07_Reports/` | Full research reports and Word documents | Active |
| `08_Monitors/` | Portfolio monitor snapshots | Active |
| `99_Templates/` | Note templates | Stable |

---

## Coverage Universe (as of June 3, 2026)

### Power Generation & Grid

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| GEV | Buy | $1,200 | High |
| VST | Buy | $230 | High |
| CEG | Buy | $385 | High |
| NRG | Buy | $185 | High |
| ETN | Hold | $420 | Medium |
| HUBB | Buy | $545 | Medium-High |
| PWR | Hold | $680 | Medium |
| SMNEY | Hold | $175 | Medium |

### Cooling & Thermal

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| VRT | Buy | $370 | High |
| MOD | Buy | $355 | High |
| TT | Hold | $515 | Medium |
| NVT | Hold | $180 | Medium |
| SPXC | Buy | $250 | Medium |

### Semiconductor Materials & Equipment

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| LRCX | Buy | $380 | High |
| AMAT | Buy | $520 | High |
| ASML | Hold | $1,730 | Medium |
| KLAC | Hold | $1,950 | Medium |
| TOELY | Buy | $403 | High |
| ENTG | Buy | $155 | Medium-High |
| MKSI | Hold | $310 | Medium |

### Critical Minerals

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| FCX | Hold | $72 | Medium |
| SCCO | Hold | $165 | Low |
| CCJ | Buy | $140 | High |
| MP | Buy | $80 | Medium-High |
| UUUU | Buy | $25 | Medium-High |

---

## Active Theses

1. **Nuclear Renaissance via Hyperscaler PPAs** — 20-year contracts re-pricing nuclear from commodity to contracted
2. **Transformer Supply Crunch** — 120-180 week lead times; GEV Prolec is the primary beneficiary
3. **Gas Turbine Backlog Pricing Power** — oligopoly sold out through 2029; new-price orders 10-20pts above backlog
4. **Liquid Cooling Mass Adoption** — physics constraint drives mandatory liquid cooling for AI GPU racks
5. **WFE Supercycle** — $140B+ WFE in 2026; multi-vector demand (HBM, NAND, logic, packaging)
6. **Copper Structural Deficit** — 10-15yr mine-to-production lag vs. AI/EV/grid demand growing 3-4% annually
7. **HBM Supply Constraint** — HBM etch intensity compounds with each GPU generation; LRCX dominant
8. **Advanced Packaging Bottleneck** — CoWoS capacity = AI GPU supply; equipment suppliers benefit from every expansion
9. **Rare Earth Decoupling from China** — bipartisan US policy + EU CRMA creating structural MP Materials demand

---

## Key Concept Notes

- [[HBM]] — High Bandwidth Memory architecture and implications
- [[CoWoS]] — TSMC's advanced packaging process behind every AI GPU
- [[SMR]] — Small Modular Reactors: status, timeline, portfolio implications
- [[HVDC]] — High Voltage Direct Current transmission: GEV position, market structure
- [[Transformer Supply]] — Why lead times hit 3.5 years and who benefits
- [[PJM Capacity Auction]] — How the RPM market works; July 2026 auction catalyst for VST/CEG
- [[Interconnect Queue]] — Why connecting new power to the grid takes 5-7 years

---

## Frontmatter Conventions

**Company notes:**

```yaml
ticker: GEV
sector: Power-Gen-Grid          # Power-Gen-Grid | Cooling-Thermal | Semi-Materials-Equip | Critical-Minerals
rating: Buy                     # Buy | Hold | Sell | Under Review
price_target: 1200.0
current_price: 959.36
market_cap: 258                 # USD billions
enterprise_value: 251           # USD billions
ai_exposure: Direct             # Direct | Indirect | Derivative
conviction: High                # High | Medium-High | Medium | Low
next_earnings: 2026-07-22       # YYYY-MM-DD
last_updated: 2026-06-03        # YYYY-MM-DD
tags: [company]
```

**Sector notes:** `tags: [sector]` | **Theses:** `tags: [thesis]` | **Concepts:** `tags: [concept]`

---

## Linking Conventions

- Company notes link to their sector: `[[Power-Gen-Grid]]`
- Company notes link to relevant theses: `[[Gas Turbine Backlog Pricing Power]]`
- First use of a technical term links to concept: `[[CoWoS]]`, `[[HBM]]`
- Earnings prep notes named `TICKER_Q#_prep.md` or `TICKER_brief.md`

---

## Workflow for New Coverage

1. Create company note from template (`99_Templates/Company Report Template.md`)
2. Fill in thesis and business overview
3. Assign rating + PT in frontmatter
4. Link to sector primer and relevant theses
5. Dashboard updates automatically via Dataview

---

## Expansion Coverage — Added June 3, 2026

### Memory & Storage (new sector)

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| MU | Hold | $1,100 | Medium |
| SNDK | Under Review | — | — |
| WDC | Hold | $560 | Medium |
| STX | Hold | $910 | Medium-Low |

### AI Networking (new sector)

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| AVGO | Buy | $560 | High |
| MRVL | Buy | $370 | High |
| ANET | Buy | $185 | High |
| COHR | Hold | $420 | Medium-High |
| CRDO | Hold | $250 | Medium |

### Power Electronics (new sector)

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| MPWR | Hold | $1,700 | Medium |
| ON | Buy | $160 | Medium-High |
| WOLF | Under Review | — | — |

### Data Center Infrastructure (new sector)

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| EQIX | Hold | $1,150 | Medium |
| DLR | Buy | $205 | Medium-High |
| IRM | Buy | $145 | High |

### Additional Theses (added June 3, 2026)
- **Memory Bottleneck** — HBM/NAND/HDD are all supply-constrained layers of the AI data hierarchy
- **AI Networking and Custom Silicon** — Broadcom/Marvell custom ASICs + AI Ethernet (Arista/Coherent/Credo)
- **SiC Power Conversion** — Silicon carbide enables AI-density power conversion; ON/WOLF/Infineon

---

## Aschenbrenner Expansion — Added June 3, 2026

### On-Site Power Generation (added to Power-Gen-Grid)

| Ticker | Rating | PT | Conviction | Thesis |
|---|---|---|---|---|
| BE | Buy | $330 | High | Bloom fuel cells; Oracle 2.8GW; Aschenbrenner #1 holding |
| CAT | Buy | $1,000 | Medium-High | Gas generators; $51B backlog +71%; 2GW AI order |
| GNRC | Buy | $320 | Medium-High | Standby/prime power; $700M DC backlog |
| OKLO | Under Review | — | — | Micro-reactor; SAlt-backed; speculative |

### AI Networking additions

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| LITE | Buy | $1,150 | High |
| FN | Buy | $720 | Medium-High |
| CLS | Buy | $530 | Medium-High |

### Miners to AI Hosts (added to Data-Center-Infra)

| Ticker | Rating | PT | Conviction |
|---|---|---|---|
| CORZ | Under Review | — | — |
| APLD | Buy | $60 | Medium-High |
| IREN | Hold | $72 | Medium |

### New Theses (Aschenbrenner expansion)
- **Fuel Cells and On-Site Power** — Bloom/CAT/GNRC bypassing grid interconnection queues
- **Miners to AI Hosts** — Bitcoin miners repurposing power infrastructure for GPU hosting

### Key New Concept
- **[[AI Bottleneck Screener]]** — repeatable framework for finding the next Bloom Energy

### Key Source
- **`05_Sources/Aschenbrenner Portfolio Analysis.md`** — full portfolio comparison, where we agree/disagree, lessons learned

---

## Aschenbrenner Deep-Dive — Added June 3, 2026

### Remaining Aschenbrenner longs initiated

| Ticker | Rating | PT | Price | Notes |
|---|---|---|---|---|
| NBIS | Buy | $310 | $263 | Nebius Group — European AI cloud; +599% YoY; his 2nd largest position |
| HUT | Hold | $145 | $137 | Hut 8 — miner-to-host; +72% past month |
| TSEM | Hold | $285 | $275 | Tower Semiconductor — specialty analog/mixed-signal foundry |

### Company briefs completed
- CCJ_brief.md — Cameco; Buy/$140; Q2 preview; uranium + Westinghouse thesis
- HUBB_brief.md — Hubbell; Buy/$545; T&D grid infrastructure; 12% below consensus PT

### Key research added to 05_Sources/
- **Aschenbrenner Portfolio Analysis** — full thesis comparison, where we agree/disagree, the AVGO divergence, portfolio construction lessons

### The Full Picture: Where This Vault Aligns with Aschenbrenner
**Agreement:** Power infrastructure, fuel cells, optical interconnect, AI hosting from miners, GPU cloud
**Partial agreement:** ASML (both cautious), MU (his short, our hold)
**Disagreement:** AVGO — we rate Buy/$560; he has $1B in puts. Our thesis: custom silicon lock-in + networking moat > multiple risk.
