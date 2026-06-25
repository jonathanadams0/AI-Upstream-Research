---
tags: [dashboard]
last_updated: 2026-06-23
---

# Position Sizing Framework

> **Correction 2026-06-23:** LRCX PT $380 → **$450** and AMAT PT $520 → **$680** (both match the company notes + [[Decisions Log]] 6/18; upside/asym recomputed on the table's 2026-06-04 price basis). **ENTG downgraded Buy→Hold 6/18, PT removed** — its row below is retained for history but marked n/a; it is no longer a Buy and is excluded from Buy sizing/tiering (Section 8's tier counts still show the pre-downgrade snapshot). `*` on P-Wt'd flags that the probability-weighted value awaits the next model refresh. All other rows remain at the 2026-06-04 snapshot.

> This framework converts research ratings into actionable portfolio weights. It answers: how much of each name, why, and under what conditions you should resize.

---

## 1. Core Principles

**This is a concentrated thematic portfolio, not a diversified fund.** The AI infrastructure thesis is a single directional bet. Diversification within it reduces individual name risk but doesn't reduce the macro risk that AI capex is cyclical. Sizing should reflect:

1. **Conviction matters more than upside.** A 50% upside with 40% probability is worth less than a 25% upside with 90% probability. The bear case — and how much of your thesis survives it — is the primary sizing input.
2. **Asymmetry over absolute return.** Prefer names where the upside is 2x+ the downside. A $200 upside/$50 downside name sizes bigger than a $200 upside/$150 downside name, even at the same PT.
3. **Sector concentration is a risk, not a diversification.** 8 Buy-rated names in Power-Gen-Grid means one macro event (AI capex freeze) hits them all simultaneously. Size the sector, not just the names.
4. **Variant perception = justification for overweight.** Names where you disagree most with consensus (CEG, NRG, MRVL, BE) deserve outsized positions precisely because the market hasn't priced your view.

---

## 2. Tier Definitions

| Tier | Label | Target Weight | Max Names | Entry Criteria |
|---|---|---|---|---|
| **1** | Large Core | 5–8% | 3–4 | High conviction + asymmetry ≥1.5x + clear variant perception |
| **2** | Core | 3–5% | 8–10 | High conviction OR Medium-High + strong asymmetry |
| **3** | Opportunistic | 1–3% | 10–12 | Medium-High conviction, catalyst-dependent, sector exposure |
| **4** | Speculative | 0.5–1.5% | 5–8 | Medium conviction, pre-profit, or limited near-term upside |

**Total portfolio weight check:** 3 Tier-1 × 6.5% + 9 Tier-2 × 4% + 9 Tier-3 × 2% + 9 Tier-4 × 1% = 19.5 + 36 + 18 + 9 = **~82.5%** invested, ~17.5% cash buffer

---

## 3. Sizing Decision Matrix

For any new position or resize, score these four factors:

| Factor | 3 pts | 2 pts | 1 pt |
|---|---|---|---|
| Conviction | High | Medium-High | Medium |
| Asymmetry (upside ÷ downside) | ≥2.0x | 1.0–2.0x | <1.0x |
| Variant perception | We're ≥30% from consensus PT | 10–30% from consensus | Aligned with consensus |
| Catalyst clarity | Named event within 90 days | Probable within 6 months | Uncertain / no catalyst |

**Score → Tier mapping:** 10–12 pts = Tier 1 | 7–9 pts = Tier 2 | 4–6 pts = Tier 3 | ≤3 pts = Tier 4

---

## 4. Sector Concentration Limits

| Sector | Buy Names | Max Sector Weight | Current Buy-Name Weight (at tier midpoints) | Action |
|---|---|---|---|---|
| Power-Gen-Grid | 8 | ≤35% | 32.5% | ✅ Within limit |
| Cooling-Thermal | 3 | ≤15% | 7.0% | ✅ Within limit |
| AI-Networking | 6 | ≤30% | 18.0% | ✅ Within limit |
| Semi-Materials-Equip | 4 | ≤15% | 8.0% | ✅ Within limit |
| Critical-Minerals | 3 | ≤10% | 7.0% | ✅ Within limit |
| Data-Center-Infra | 5 | ≤15% | 9.0% | ✅ Within limit |
| Power-Electronics | 1 | ≤8% | 1.0% | ✅ Within limit |

> **Power-Gen-Grid note:** 8 Buy names creates natural concentration risk. The mitigation is that each name solves a different bottleneck (gas turbines, nuclear, retail power, fuel cells, generators, transformers, grid equipment). However, a single AI capex freeze would hit all simultaneously. Size the sector total at ≤35% and don't let individual names exceed their tier targets.

---

## 5. All Buy Names — Tier Assignments & Sizing

*Prices as of 2026-06-04. P-weighted = probability-weighted expected value at tier conviction.*

| # | Ticker | Sector | Current | Our PT | Upside | Bear | Asym | P-Wt'd | Tier | Target Wt | Aschenbrenner | Next Catalyst |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | **GEV** | Power-Gen-Grid | $951.66 | $1,200 | +26% | $600 | 0.7x | $1,155 | **T1** | 5–8% | Neutral | Jul 22 Q2 |
| 2 | **CEG** | Power-Gen-Grid | $262.66 | $385 | +47% | $220 | 2.9x | $371 | **T1** | 5–8% | Neutral | Aug 7 Q2 |
| 3 | **NRG** | Power-Gen-Grid | $132.05 | $185 | +40% | $110 | 2.4x | $188 | **T1** | 5–8% | Neutral | Aug 7 Q2 |
| 4 | **VST** | Power-Gen-Grid | $151.03 | $230 | +52% | $145 | 13.1x | $228 | **T2** | 3–5% | Aligned | Aug 7 Q2 |
| 5 | **BE** | Power-Gen-Grid | $283.32 | $330 | +16% | $120 | 0.3x | $318 | **T2** | 3–5% | Aligned #1 | Aug 6 Q2 |
| 6 | **CAT** | Power-Gen-Grid | $933.73 | $1,000 | +7% | $620 | 0.2x | $974 | **T3** | 1–3% | Neutral | Jul Q2 |
| 7 | **GNRC** | Power-Gen-Grid | $277.82 | $320 | +15% | $175 | 0.4x | $304 | **T4** | 0–2% | Neutral | Jul Q2 |
| 8 | **HUBB** | Power-Gen-Grid | $481.39 | $545 | +13% | $320 | 0.4x | $514 | **T3** | 1–3% | Neutral | Jul Q2 |
| 9 | **VRT** | Cooling-Thermal | $318.31 | $370 | +16% | $220 | 0.5x | $372 | **T2** | 3–5% | Neutral | Jul 28 Q2 |
| 10 | **MOD** | Cooling-Thermal | $291.34 | $355 | +22% | $150 | 0.5x | $338 | **T3** | 1–3% | Neutral | Aug Q2 |
| 11 | **SPXC** | Cooling-Thermal | $234.50 | $250 | +7% | $150 | 0.2x | $238 | **T4** | 0–2% | Neutral | Aug Q2 |
| 12 | **AVGO** | AI-Networking | $413.90 | $560 | +35% | $350 | 2.3x | $553 | **T2** | 3–5% | Short! | ~Sep 4 Q3 |
| 13 | **MRVL** | AI-Networking | $308.83 | $370 | +20% | $180 | 0.5x | $364 | **T2** | 3–5% | Short | Aug 27 Q2 |
| 14 | **ANET** | AI-Networking | $164.90 | $185 | +12% | $90 | 0.3x | $175 | **T2** | 3–5% | Neutral | Jul 29 Q2 |
| 15 | **CLS** | AI-Networking | $420.27 | $530 | +26% | $250 | 0.6x | $504 | **T3** | 1–3% | Neutral | Aug Q2 |
| 16 | **FN** | AI-Networking | $687.07 | $720 | +5% | $450 | 0.1x | $711 | **T3** | 1–3% | Neutral | Aug Q2 |
| 17 | **LITE** | AI-Networking | $901.25 | $1,150 | +28% | $600 | 0.8x | $1,102 | **T3** | 1–3% | Neutral | Jul 29 Q2 |
| 18 | **LRCX** | Semi-Materials-Equip | $334.76 | $450 | +34% | $200 | 0.9x | $374* | **T2** | 3–5% | Neutral | Jul 29 Q4 |
| 19 | **AMAT** | Semi-Materials-Equip | $498.52 | $680 | +36% | $300 | 0.9x | $508* | **T3** | 1–3% | Neutral | Aug Q2 |
| 20 | **ENTG** | Semi-Materials-Equip | $141.81 | — | — | $85 | — | — | **n/a** | — | Neutral | **Downgraded Buy→Hold 6/18** |
| 21 | **TOELY** | Semi-Materials-Equip | N/A | $403 | — | N/A | — | — | **T4** | 0–2% | Neutral | Aug Q2 |
| 22 | **CCJ** | Critical-Minerals | $113.94 | $140 | +23% | $85 | 0.9x | $138 | **T2** | 3–5% | Neutral | Aug 6 Q2 |
| 23 | **MP** | Critical-Minerals | $65.99 | $80 | +21% | $35 | 0.5x | $81 | **T3** | 1–3% | Neutral | Aug Q2 |
| 24 | **UUUU** | Critical-Minerals | N/A | $25 | — | $4 | — | — | **T4** | 0–2% | Neutral | Aug Q2 |
| 25 | **IRM** | Data-Center-Infra | $127.07 | $145 | +14% | $100 | 0.7x | $144 | **T3** | 1–3% | Neutral | Jul 30 Q2 |
| 26 | **NBIS** | Data-Center-Infra | $248.01 | $310 | +25% | $80 | 0.4x | $286 | **T2** | 3–5% | Aligned #2 | Aug 14 Q2 |
| 27 | **DLR** | Data-Center-Infra | $185.36 | $205 | +11% | $140 | 0.4x | $194 | **T4** | 0–2% | Neutral | Jul 24 Q2 |
| 28 | **APLD** | Data-Center-Infra | $42.64 | $60 | +41% | $20 | 0.8x | $58 | **T4** | 0–2% | Neutral | Aug Q2 |
| 29 | **XYL** | Data-Center-Infra | $110.04 | $135 | +23% | $85 | 1.0x | $129 | **T4** | 0–2% | Neutral | Aug Q2 |
| 30 | **ON** | Power-Electronics | $129.91 | $160 | +23% | $80 | 0.6x | $154 | **T4** | 0–2% | Neutral | Aug Q2 |

---

## 6. Rebalancing Rules

**Upsize triggers (move up one tier):**
- A catalyst confirms the variant perception (hyperscaler contract signed, backlog beat, guidance raise)
- Stock falls to within 10% of the bear case price without a thesis change (buying opportunity)
- Aschenbrenner 13F shows a new or increased position in the name (45-day lag)

**Downsize triggers (move down one tier):**
- Stock reaches within 5% of our price target without a thesis upgrade → harvest gains, move to Tier 3
- Any of the bear case triggers activates (see ## Bear Case in each company note)
- Position grows to >2x its target weight from appreciation without re-underwriting

**Exit triggers (full sale):**
- Two bear case triggers activate simultaneously
- Management loses credibility (guidance miss >15% + explanation is vague)
- A competitor wins a design displacement at the thesis-critical customer
- Thesis invalidation event (see ## Bear Case in each note for specific triggers)

**Sector rebalancing:**
- If any sector exceeds its limit by >5% (i.e., Power-Gen-Grid >40%), trim the lowest-conviction names in that sector first
- After a major catalyst event, re-run the scoring matrix on affected names — catalyst resolution often changes tier

---

## 7. The Aschenbrenner Overlay

Situational Awareness LP runs a related but partially inverted portfolio. Use as a signal, not a constraint:

| Category | Aschenbrenner | This Vault | Implication |
|---|---|---|---|
| BE (Bloom Energy) | Long ~$900M — **#1 holding** | Tier 2 Core, 3–5% | High alignment. Size at upper end of tier (4–5%) |
| NBIS (Nebius) | Long ~$2.58B — **#2 holding** | Tier 2 Core, 3–5% | Full alignment. His conviction > ours → watch 13F for size changes |
| VST, CEG | Long power infrastructure | Tier 1/2 | Aligned — he got there first on these names |
| AVGO | Short $1.01B puts | Tier 2 Core | **Key disagreement.** His short thesis: custom silicon fragments. Our bull thesis: TAM expands. Monitor quarterly. |
| NVDA | Short $1.57B puts | Not covered | His bet: NVDA structurally challenged. We don't cover. If correct, benefits AI infrastructure alternatives (GEV, BE, NRG). |
| CORZ | Long (acquisition by CWAI) | Under Review | Pending CoreWeave completion — not sizing |

**Aschenbrenner 13F schedule:** Next filing due ~Aug 14, 2026 (45-day lag from June 30 quarter-end). Watch for: (1) AVGO short size change, (2) BE/NBIS increases, (3) new positions not in our coverage.

---

## 8. Portfolio Summary at Target Weights

*Approximate portfolio composition at tier midpoints.*

| Tier | Names | Avg Weight | Total Weight |
|---|---|---|---|
| **Tier 1** | GEV, CEG, NRG | 6.5% | 19.5% |
| **Tier 2** | VST, BE, VRT, AVGO, MRVL, ANET, LRCX, CCJ, NBIS | 4.0% | 36.0% |
| **Tier 3** | CAT, HUBB, MOD, CLS, FN, LITE, AMAT, MP, IRM | 2.0% | 18.0% |
| **Tier 4** | GNRC, SPXC, ENTG, TOELY, UUUU, DLR, APLD, XYL, ON | 1.0% | 9.0% |
| **Total** | 30 names | — | **82.5%** |
| **Cash buffer** | — | — | **17.5%** |

---

## 9. How to Use This Document

1. **Before initiating a position:** Score the name on the 4-factor matrix (Section 3). Assign tier. Size at tier midpoint.
2. **Quarterly review:** Update current prices in [[04_Models/Valuation_Snapshots_All30]] — the P-weighted value column auto-updates. Re-check tier assignments for any name where upside has compressed below tier threshold.
3. **After a catalyst event:** Re-run the bear case triggers (## Bear Case in each note). If two triggers activate, move to exit protocol.
4. **Sector check:** After any major sector-level event (AI capex announcement, power price move), check sector total weights against Section 4 limits.
5. **Aschenbrenner 13F:** Each quarter after the 45-day lag, scan for new positions and size changes. Document in [[05_Sources/Aschenbrenner Portfolio Analysis]].

---

*Last updated: 2026-06-04 | Source: Bigdata.com (bigdata.com) | Valuation data: [[04_Models/Valuation_Snapshots_All30]]*