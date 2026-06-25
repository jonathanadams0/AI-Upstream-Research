---
tags: [dashboard]
last_updated: 2026-06-04
---

# Portfolio Summary — AI Infrastructure Vault

*Snapshot as of June 9, 2026. 58 covered names across 8 sectors. (BW added Under Review 6/9.)*

> ⚠️ **Static snapshot (early-June prices).** The "Current" and "Upside" columns below are ~June 9 and have drifted materially since (incl. the 6/23 AI/semi selloff). For live ratings and PTs use the Dataview tables in [[Dashboard]]; for the tracked paper book and NAV use [[Model Portfolio]]. Use this page for structure — sector map, cross-portfolio dependencies, catalyst calendar — not for current prices.

---

## Coverage by Sector

| Sector | Total | Buy | Hold | Under Review | Top Buy |
|---|---|---|---|---|---|
| Power-Gen-Grid | 14 | 8 | 3 | 3 | GEV, VST, CEG, NRG, BE, CAT, GNRC |
| Cooling-Thermal | 5 | 3 | 2 | 0 | VRT, MOD |
| Semi-Materials-Equip | 8 | 4 | 4 | 0 | LRCX, AMAT, TOELY, ENTG |
| Critical-Minerals | 5 | 3 | 2 | 0 | CCJ, MP, UUUU |
| Memory-Storage | 4 | 0 | 3 | 1 | — (all Hold; run too far) |
| AI-Networking | 9 | 6 | 3 | 0 | AVGO, MRVL, ANET, LITE, FN |
| Power-Electronics | 3 | 1 | 1 | 1 | ON |
| Data-Center-Infra | 10 | 5 | 3 | 2 | NBIS, APLD, IRM, DLR |
| **Total** | **58** | **30** | **21** | **7** | |

---

## Top 15 Highest Conviction Buys

| Rank | Ticker | Sector | PT | Current | Upside | Conviction | Thesis |
|---|---|---|---|---|---|---|---|
| 1 | GEV | Power-Gen-Grid | $1,200 | $952 | +26% | High | Gas turbine oligopoly; sold out through 2029 |
| 2 | ANET | AI-Networking | $185 | $165 | +12% | High | AI Ethernet dominant; $11.5B rev guide raised |
| 3 | NRG | Power-Gen-Grid | $185 | $132 | +40% | High | BYOP; 5.4GW GEV/Kiewit pipeline; 45% below consensus |
| 4 | CEG | Power-Gen-Grid | $385 | $263 | +47% | High | Calpine+nuclear; 47% below consensus $391 PT |
| 5 | IRM | Data-Center-Infra | $145 | $127 | +14% | High | Data center pivot; priced as document storage |
| 6 | CCJ | Critical-Minerals | $140 | $114 | +23% | High | Nuclear renaissance; Westinghouse JV; sold out |
| 7 | AVGO | AI-Networking | $560 | $414 | +35% | High | Custom AI silicon (Google/Meta/Apple) + networking |
| 8 | MRVL | AI-Networking | $370 | $309 | +20% | High | Amazon Trainium + Microsoft Maia; 50+ design wins |
| 9 | VRT | Cooling-Thermal | $370 | $318 | +16% | High | AI cooling pure-play; +195% YoY orders bellwether |
| 10 | BE | Power-Gen-Grid | $330 | $283 | +16% | High | Bloom fuel cells; Oracle 2.45GW; Aschenbrenner #1 |
| 11 | NBIS | Data-Center-Infra | $310 | $248 | +25% | High | European AI cloud; +529% YoY; NVDA alliance |
| 12 | LRCX | Semi-Materials-Equip | $380 | $335 | +14% | High | HBM TSV etch; SAM expanding; WFE supercycle |
| 13 | VST | Power-Gen-Grid | $230 | $151 | +52% | High | Meta+AWS nuclear PPAs; Cogentrix H2 2026 |
| 14 | MOD | Cooling-Thermal | $355 | $291 | +22% | High | Fastest-growing DC cooling; +218% YoY |
| 15 | CAT | Power-Gen-Grid | $1,000 | $934 | +7% | Medium-High | $51B backlog +71%; 2GW AI generator order |

---

## The Aschenbrenner Overlap Matrix

*Green = aligned, Yellow = partial, Red = disagreement*

| Category | Aschenbrenner | This Vault | Alignment |
|---|---|---|---|
| Power infrastructure (VST, CEG) | Long | Buy | ✅ Aligned |
| Fuel cells (BE) | Long $900M | Buy/$330 | ✅ Aligned |
| Miners to AI hosts (CORZ, APLD, IREN) | Long basket | CORZ Under Review, APLD Buy, IREN Hold | ✅ Broadly aligned |
| European AI cloud (NBIS) | Long $2.58B | Buy/$310 | ✅ Aligned |
| GPU cloud (CWAI) | Long | Hold-equivalent | ✅ Aligned |
| Optical interconnect (COHR) | Long | Hold | ✅ Broadly aligned |
| Semiconductor ETF (SMH) | Short $2B | — | N/A (ETF not covered) |
| Nvidia (NVDA) | Short $1.57B | Not covered | — |
| **Broadcom (AVGO)** | **Short $1.01B** | **Buy/$560** | **❌ Key disagreement** |
| AMD | Short $969M | Not covered | — |
| Micron (MU) | Short puts | Hold/$1,100 | ⚠️ Partial (his short vs our hold) |
| ASML | Short puts | Hold/$1,730 | ✅ Both cautious at current price |
| Corning (GLW) | Short | Under Review (NVDA deal changes thesis) | ⚠️ Changed — NVDA deal may invalidate his short |

---

## Cross-Portfolio Dependencies

Key relationships between covered names — where one company's success directly requires another's product:

```
NBIS (AI cloud) ←— uses power from —→ BE (Bloom fuel cells)
                     Aschenbrenner long both

CORZ/APLD/IREN (AI hosts) ←— need GPUs from —→ CWAI/NVDA
CORZ ←— being acquired by —→ CWAI (CoreWeave)

ANET (switches) ←— uses ASICs from —→ AVGO (Broadcom Tomahawk)
COHR/LITE (transceivers) ←— manufactured by —→ FN (Fabrinet)
LRCX ←— services memory for —→ MU, SNDK, STX

GEV ←— turbines ordered by —→ NRG (GEV/Kiewit/NRG venture)
GEV ←— SMR technology for —→ CEG, VST (nuclear uprates, BWRX-300)

VST/CEG ←— fuel from —→ CCJ, UUUU (uranium)
GEV, ETN, HUBB ←— grid equipment for —→ VST, CEG, NRG grid connections

BE ←— SOFC power for —→ NBIS, Oracle AI campuses
```

---

## Key Upcoming Catalysts (Next 90 Days)

| Date | Company | Event | What to Watch |
|---|---|---|---|
| Jun 8, 2026 | FCEL | Q2 earnings | First read on fuel cell AI data center pipeline |
| ~Jul 16 | ASML | Q2 earnings | EUV shipment pace vs ≥60 target; non-EUV DUV growth |
| ~Jul 22 | GEV | Q2 earnings | Gas turbine backlog vs 110GW target; Electrification DC orders |
| ~Jul 22 | FCX, HUBB | Q2 earnings | Copper production; Utility Solutions backlog |
| ~Jul 24 | DLR | Q2 earnings | AI campus backlog; pre-leased % |
| ~Jul 28 | ETN, GNRC | Q2 earnings | DC orders; margin recovery from Q1 trough (ETN); hyperscaler approval update (GNRC) |
| ~Jul 29 | KLAC, ANET | Q2/Q4 earnings | KLA advanced packaging $1B milestone; ANET AI Ethernet backlog |
| ~Jul 30 | EQIX, SPXC, IRM, NVT | Q2 earnings | EQIX AI bookings; IRM DC revenue growth |
| ~Aug 6, 7 | CCJ, WOLF, NRG, CORZ | Q2 earnings | CCJ uranium contract progress; VST summer ERCOT |
| ~Aug 7 | VST | Q2 earnings | ERCOT summer weather; Cogentrix timeline |
| Jul 2026 | PJM Capacity Auction | Market event | Clearing price for 2027/2028 delivery — catalyst for VST/CEG/NRG |
| ~Aug 12 | HUT | Q2 earnings | AI hosting revenue progress |
| ~Aug 14 | NBIS | Q2 earnings | Revenue growth vs +684% YoY Q1; profitability continuation |

---

## The Aschenbrenner Framework Applied to This Vault

**What he got right that we initially missed:**
1. Bloom Energy — grid-bypass fuel cells for AI; +1,396% YoY
2. Nebius — European AI cloud; +599% YoY
3. Core Scientific — miner-to-AI-host; CoreWeave acquisition validation
4. Caterpillar backlog growth — AI generator orders not priced in

**What he is doing that we are not:**
- Running a pairs trade: long infrastructure, short expensive chip names (NVDA, AVGO)
- We rate AVGO Buy — this is the primary tactical disagreement

**The screening framework takeaway:**
Every quarter, run the [[AI Bottleneck Screener]] on:
1. Any industrial company with "data center" appearing in earnings transcripts for the first time
2. Any 8-K from a non-tech company naming a hyperscaler as counterparty
3. Backlog data for industrial power generation, specialty chemicals, and construction companies
4. 13F filings from Situational Awareness LP (45-day lag) for new positions

---

---

## Thesis Invalidation Tracker

*One metric per name. If observed → re-underwrite immediately. Two triggers active simultaneously → default to exit.*
*Last updated: 2026-06-04. Update quarterly and after each bear case trigger event.*

| Ticker | Rating | Sell Trigger (single most important) | Monitor Via | Last Checked |
|---|---|---|---|---|
| GEV | Buy | Gas turbine backlog declines from 110 GW target | Quarterly earnings backlog slide | 2026-06-04 |
| CEG | Buy | PJM/FERC rules against hyperscaler co-location model | FERC CIFP proceeding final order | 2026-06-04 |
| NRG | Buy | No GEV/Kiewit LOI converts to signed PPA by Jun 2027 | Quarterly earnings; 8-K filings | 2026-06-04 |
| VST | Buy | Cogentrix fails to close or is materially repriced | Regulatory approval disclosures | 2026-06-04 |
| BE | Buy | Oracle Project Jupiter delayed or scoped below 1 GW | Oracle/Bloom 8-K; earnings calls | 2026-06-04 |
| AVGO | Buy | Google or Meta announces reduced Broadcom ASIC dependency | Annual developer conferences | 2026-06-04 |
| MRVL | Buy | Amazon or Microsoft delays Trainium 3 / Maia 3 program | AWS/MSFT earnings; developer days | 2026-06-04 |
| ANET | Buy | Revenue guidance cut >15% citing InfiniBand share shift | Quarterly guidance; hyperscaler commentary | 2026-06-04 |
| VRT | Buy | Order guidance cut >15% in single quarter | Quarterly orders slide | 2026-06-04 |
| NBIS | Buy | Revenue growth decelerates below 50% YoY for 2 quarters | Quarterly earnings release | 2026-06-04 |
| LRCX | Buy | WFE industry spending cut >15% by SEMI or major analyst | SEMI World Fab Forecast; peer guidance | 2026-06-04 |
| CCJ | Buy | Uranium spot price below $60/lb for 2 consecutive quarters | UxC weekly uranium spot | 2026-06-04 |
| IRM | Buy | Data center pre-lease rate falls below 70% on new campus | Quarterly leasing disclosures | 2026-06-04 |
| CAT | Buy | North America construction orders decline >15% YoY for 2 quarters | Monthly ABI; quarterly guidance | 2026-06-04 |
| GNRC | Buy | No hyperscaler generator approval within 9 months | Earnings call; 8-K filings | 2026-06-04 |
| HUBB | Buy | Utility Solutions backlog growth decelerates below 5% YoY | Quarterly backlog disclosure | 2026-06-04 |
| MOD | Buy | Data center revenue growth decelerates below 20% YoY for 2 quarters | Quarterly segment revenue | 2026-06-04 |
| CLS | Buy | Single customer >40% of revenue reduces orders >20% | Quarterly revenue concentration | 2026-06-04 |
| FN | Buy | Two top-3 OEM customers reduce orders >20% same quarter | Quarterly customer disclosures | 2026-06-04 |
| LITE | Buy | Revenue guidance cut >10% in single quarter | Quarterly guidance; sector commentary | 2026-06-04 |
| AMAT | Buy | WFE industry spending revised down >15% | SEMI; peer guidance (LRCX, KLAC) | 2026-06-04 |
| ENTG | Buy | Management cites customer inventory correction | Earnings call language | 2026-06-04 |
| MP | Buy | China removes rare earth export restrictions | Chinese Ministry of Commerce | 2026-06-04 |
| UUUU | Buy | Uranium spot below $60/lb sustained; no utility contract in 12 months | UxC + 10-Q disclosures | 2026-06-04 |
| DLR | Buy | Pre-lease rate below 60% on new development | Quarterly leasing update | 2026-06-04 |
| APLD | Buy | Balance sheet refinancing fails or prices at >300bps premium | 8-K debt filings | 2026-06-04 |
| SPXC | Buy | HVAC segment bookings decline >20% for 2 quarters | Quarterly bookings | 2026-06-04 |
| ON | Buy | Automotive SiC guidance cut >15% citing inventory overbuild | Quarterly automotive segment; OEM EV volumes | 2026-06-04 |
| XYL | Buy | Infrastructure Solutions revenue declines >10% YoY for 2 quarters | Quarterly segment revenue | 2026-06-04 |
| TOELY | Buy | WFE industry spending cut >15%; Japan-US export control escalation | SEMI; US Commerce Dept | 2026-06-04 |

## Vault Maintenance Schedule

| Task | Frequency | Priority |
|---|---|---|
| Update `current_price` in all frontmatter | Weekly (automated — Fri 4:30 PM, "weekly-vault-price-refresh" scheduled task) | Medium |
| Earnings prep notes for upcoming reporters | 2 weeks before | High |
| Run AI Bottleneck Screener | Quarterly | High |
| Check Aschenbrenner 13F (45-day lag) | Quarterly | High |
| Add new sector/company if passes screener | As needed | High |
| Update thesis conviction levels | Quarterly | Medium |
| 10-Q review for top 10 Buy names | Quarterly | Medium |
