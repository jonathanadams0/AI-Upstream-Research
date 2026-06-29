---
tags: [dashboard, macro, geopolitical]
last_updated: 2026-06-25
---

# Global Macro Overlay — Geopolitical Risk Layer

> This is a first-order input layer, not a background watchlist. Every position in the Semi-Materials-Equip and Memory-Storage sectors has direct revenue exposure to at least one of the three vectors below. A breach condition here triggers a re-underwrite of affected names — same discipline as a bear-case breach.
>
> **Monthly check:** automated loop runs first trading day of each month → writes `08_Monitors/Macro_Geo_Check_<date>.md`.
> **Ad-hoc:** catalyst-execution loop (weekday 7am) picks up any >±5% move in Samsung (005930.KS) or SK Hynix (000660.KS) on days they report.

---

## Vector 1 — Korea: Samsung & SK Hynix

### Why it matters
Samsung and SK Hynix together control ~55% of global NAND flash supply and ~50% of DRAM. Their capex decisions are the single most important input for wafer fab equipment (WFE) spending — which is the direct revenue driver for LRCX, AMAT, ASML, and ENTG. Their pricing/volume signals set the NAND/DRAM cycle, which drives MU and SNDK.

### Key companies to watch
| Company | Ticker | Reports | What to track |
|---|---|---|---|
| Samsung Electronics | 005930.KS | Preliminary flash ~4 weeks post-quarter; full ~6 weeks | **Capex guidance (₩ trillion)** — primary input; NAND/DRAM ASP commentary; HBM share vs SK Hynix |
| SK Hynix | 000660.KS | Full report ~4–5 weeks post-quarter | **HBM capacity ramp** (SK Hynix leads HBM3E/4); NAND bit growth; capex vs prior guidance |
| TrendForce | (monthly report) | First week of each month | **NAND/DRAM contract price index** — leading indicator; watch QoQ % change |

### Portfolio exposure map
| Portfolio name | How Korea affects it | Severity |
|---|---|---|
| [[LRCX]] (Buy/$450) | Samsung + SK Hynix are top 2 WFE customers; memory capex = LRCX revenue | **Critical** |
| [[AMAT]] (Buy/$680) | Same customer base; AMAT CVD/ALD tools in every NAND layer | **Critical** |
| [[ASML]] (Hold/$1,730 stale) | Samsung is largest EUV customer globally; SK Hynix EUV ramp for HBM | **High** |
| [[ENTG]] (Hold/no PT) | Patterning materials, CMP, advanced packaging — all tied to memory capex | **High** |
| [[MU]] (Buy/$1,500) | Direct competitor; Korean price/supply decisions set MU's ASP ceiling | **High** |
| [[SNDK]] (Hold/$2,000) | Pure-play NAND; Korean supply discipline = SNDK margin | **High** |

### Breach thresholds → action required
| Signal | Threshold | Read | Action |
|---|---|---|---|
| Samsung capex cut | >15% YoY reduction in guided semi capex | WFE supercycle stalling | **Re-underwrite LRCX, AMAT, ENTG**; check shared WFE sell trigger in [[Catalyst Playbooks]] |
| Samsung capex cut | >25% YoY | Cycle turn likely | **Downgrade trigger** for LRCX/AMAT per bear case; flag ASML |
| SK Hynix HBM capex cut | Explicitly guides lower or delays HBM4 | HBM cycle slowing | **Negative read-through LRCX** (HBM TSV etch revenue); flag before Jul 29 LRCX print |
| NAND contract price decline | >10% QoQ (TrendForce) | ASP erosion starting | **Bear check on SNDK** ($400 bear); note in MU watch |
| NAND contract price decline | >20% QoQ | Cycle reversal | **Re-underwrite SNDK**; flag MU GM |
| Samsung supply surge commentary | Explicit NAND bit growth >30% guided | Supply flooding | Prepare bear scenarios; SNDK asymmetry already unfavorable from $2,335 |
| Korean earnings beat on capex raise | >10% capex raise vs prior guidance | Supercycle extending | **Positive read-through LRCX/AMAT**; confirm PTs; note before next print |

### Earnings calendar (rolling — update each quarter)
| Event | Approx. date | Notes |
|---|---|---|
| Samsung Q2 2026 preliminary flash | ~July 7–8, 2026 | Revenue/OP estimate only; capex in full report |
| Samsung Q2 2026 full earnings | ~July 30–31, 2026 | Capex guidance here — same week as LRCX (Jul 29) |
| SK Hynix Q2 2026 earnings | ~July 24, 2026 | HBM4 ramp update; will move LRCX thesis |
| Samsung Q3 2026 preliminary flash | ~October 7–8, 2026 | |
| SK Hynix Q3 2026 earnings | ~October 22–24, 2026 | |

---

## Vector 2 — Taiwan: TSMC

### Why it matters
TSMC is the foundry for virtually every advanced chip driving AI demand — Nvidia, AMD, Broadcom, Apple. TSMC's capex cycle drives EUV tool demand (ASML), etch/deposition demand (LRCX, AMAT), and advanced packaging demand. Separately, Taiwan's geopolitical status vs. China is the tail-risk scenario that reprices the entire semi complex.

### Key companies to watch
| Company | Ticker | Reports | What to track |
|---|---|---|---|
| TSMC | TSM / 2330.TW | Monthly revenue (10th of following month); quarterly earnings ~3rd week of month | **Monthly revenue** (real-time demand signal); capex guidance (annual, updated quarterly); CoWoS capacity; 2nm ramp |
| Taiwan cross-strait headlines | — | Ongoing | PLA military exercises; US arms sales; Taiwan Strait incident frequency |

### Portfolio exposure map
| Portfolio name | How Taiwan affects it | Severity |
|---|---|---|
| [[ASML]] (Hold/$1,730 stale) | TSMC is #1 ASML customer; TSMC CoWoS/2nm drives High-NA demand | **Critical** |
| [[LRCX]] (Buy/$450) | TSMC advanced logic = significant portion of LRCX logic revenue | **High** |
| [[AMAT]] (Buy/$680) | Gate-all-around transition at TSMC is an AMAT tool-intensive node | **High** |
| [[TSEM]] (Hold/$285) | Tower Semi is a specialty foundry; TSMC competitive overlap minor but geopolitical risk shared | **Medium** |
| [[ENTG]] (Hold/no PT) | Advanced patterning materials for TSMC nodes | **Medium** |

### Breach thresholds → action required
| Signal | Threshold | Read | Action |
|---|---|---|---|
| TSMC monthly revenue decline | >5% MoM for 2 consecutive months | Fab utilization falling | Note in monthly macro check; watch ASML order intake |
| TSMC capex cut | >15% vs current $38–42B annual guidance | Cycle softening | **Re-underwrite ASML, LRCX, AMAT** simultaneously |
| TSMC capex raise | >10% above guidance | Supercycle extended | Positive read-through; confirm PTs |
| Taiwan Strait military escalation | PLA naval/air incursion into 12nm territorial waters or strait blockade exercise | Geopolitical risk premium repricing | **Reduce semi equipment exposure** — this is a tail scenario, not base case; document in [[Decisions Log]] |
| US export restriction tightening | New rule restricting TSMC access to US equipment/materials | Supply chain disruption | Re-underwrite entire semi equipment book |

### Data to pull monthly
- TSMC monthly revenue (TWD; released ~10th of month via TWSE filing)
- Any CoWoS or advanced packaging capacity commentary

---

## Vector 3 — US-China Export Controls

### Why it matters
Export control policy is the single largest binary risk in the book. ASML, LRCX, AMAT, ENTG, and TOELY all have China revenue that could be impaired by further rule tightening. ASML's China revenue was ~29% of total in Q1 2026; LRCX's China share is a key watchlist item in the [[Catalyst Playbooks]]. A major escalation reprices the whole semi equipment complex.

### Key regulatory bodies to watch
| Body | What to monitor |
|---|---|
| Bureau of Industry and Security (BIS) | New Entity List additions; Foreign Direct Product Rule (FDPR) expansions; EAR rule updates |
| OFAC | Designations of Chinese semi companies (SMIC, etc.) |
| Dutch government / ASML | ASML export license renewals (require annual Dutch govt approval) |
| Japanese METI | Japan's parallel controls on Tokyo Electron + Shin-Etsu — Japan aligned with US in 2023; watch for tightening |

### Portfolio exposure map
| Portfolio name | China revenue exposure | Severity |
|---|---|---|
| [[ASML]] (Hold/$1,730 stale) | ~29% of revenue (Q1 2026) — DUV tools only; EUV already blocked | **Critical** |
| [[LRCX]] (Buy/$450) | China share ~20–25%; **explicit invalidation trigger** if <20% with no offset | **Critical** |
| [[AMAT]] (Buy/$680) | China ~25–28% of revenue | **Critical** |
| [[ENTG]] (Hold/no PT) | China exposure via Chinese fab customers | **High** |
| [[TOELY]] (Hold/$270 ADR) | Tokyo Electron — Japan controls aligned with US; China exposure meaningful | **High** |

### Breach thresholds → action required
| Signal | Threshold | Read | Action |
|---|---|---|---|
| BIS new rule — equipment controls | Expanded to include DUV tools or specific etch/dep categories | Direct revenue impairment | **Re-underwrite LRCX, AMAT, ASML immediately**; China share <20% invalidation trigger fires for LRCX |
| ASML Dutch license non-renewal | Dutch government declines ASML China DUV license | ~29% revenue risk | **Downgrade ASML**; re-underwrite from scratch |
| BIS Entity List — major Chinese foundry | SMIC tier-2 entities or new entrants added | Customer access cut | Flag LRCX/AMAT China revenue; check customer concentration |
| Escalation de-escalation | US-China bilateral agreement or carve-out announced | China revenue risk reduced | Positive read-through; review ASML/LRCX PT upside |
| Export control loosening | BIS grants new general licenses or raises chip thresholds | China opportunity re-opens | Positive for all semi equipment names |

### News sources to check monthly
- BIS Federal Register (regulations.gov, "Export Administration Regulations")
- Reuters / WSJ US-China trade desk
- CSIS and Semiconductor Industry Association (SIA) policy trackers

---

## Cross-Vector Risk: The "Perfect Storm" Scenario

If all three vectors fire negative simultaneously:
- Samsung cuts capex >20% (Korea)
- TSMC cuts capex >15% (Taiwan)
- BIS expands DUV controls (China)

This is the bear case for the entire semi equipment cluster: LRCX, AMAT, ASML, ENTG all re-underwrite simultaneously. Under this scenario, the [[AI Capex Stress Test]] Group 2 bear cases activate. Probability assessed as low (5–10%) given current supercycle momentum, but the tail is severe — LRCX bear $200 (−48% from $388), AMAT bear not formally stated.

**Pre-committed response to the "Perfect Storm":** if any 2 of 3 vectors breach simultaneously within a 30-day window, convene a full portfolio re-underwrite session before acting. Do not make piecemeal decisions under cross-vector stress.

---

## Maintenance

- **Monthly:** automated loop writes `08_Monitors/Macro_Geo_Check_<YYYY-MM-DD>.md` on first trading day of each month
- **Quarterly:** update the earnings calendar table above at the start of each quarter
- **After any breach signal:** log the event in [[Decisions Log]] same day, even if no action is taken (documents the reasoning)
- **After LRCX/ASML/AMAT prints:** check if the Korean/Taiwan inputs are consistent with what management said on the call; update the "Earnings calendar" table

*Layer established: 2026-06-25*
