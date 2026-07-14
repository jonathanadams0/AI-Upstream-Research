---
type: intraday-alert
date: 2026-07-14
time_ct: "15:00"
run_type: market-close
alerts_fired: [condition-a-LITE, condition-a-NBIS, condition-b-CCJ, condition-b-FN]
standing_levels: clear
---

# Intraday Alert — 2026-07-14 Close (15:00 CT)

> End-of-day close run. Earlier intraday detail (including news catalysts, action items) captured in [Intraday_Alert_2026-07-14_1306.md]. This note records confirmed closing prices.

---

## Condition A — Move > ±5% at Close

### LITE — Lumentum — **+6.07%**

| Ticker | Current | Daily $ | Daily % | Bear | vs Bear |
|--------|---------|---------|---------|------|---------|
| LITE | $814.78 | +$46.63 | +6.07% | $600 | +$214.78 (+35.8%) |

Confirmed above 5% at close; had pulled back to +4.88% around 1300 CT before recovering into the close. Catalyst: sector read-across from Applied Optoelectronics (AAOI) Texas AI manufacturing expansion — no LITE-specific news. Bear floor ($600) not implicated; stock is 35.8% above bear.

---

### NBIS — Nebius Group — **−7.84%**

| Ticker | Current | Daily $ | Daily % | Bear | vs Bear |
|--------|---------|---------|---------|------|---------|
| NBIS | $194.00 | −$16.51 | −7.84% | $80 | +$114.00 (+142.5%) |

Accelerated from −6.00% at 1306 CT to −7.84% at close. Mixed catalyst day: Reflection AI signed $1B+ compute deal with NBIS (positive demand signal), but Meta cloud-leasing plans (flagged in Motley Fool, context in 1306 note) weighed throughout the session. Bear floor ($80) not at risk — 142.5% above. Thesis-level check recommended at next weekly review.

---

## Condition B — Within 10% of Bear-Case Price

### CCJ — Cameco — **7.7% above bear ($85)**

| Ticker | Current | Daily $ | Daily % | Bear | vs Bear |
|--------|---------|---------|---------|------|---------|
| CCJ | $91.57 | +$1.37 | +1.52% | $85 | +$6.57 (+7.7%) |

Watch zone threshold: $93.50 (10% above $85). CCJ closed inside buffer for a second consecutive session. No name-specific negative catalyst today. Q2 earnings July 31 is the key binary; re-underwrite protocol fires on close below $85.

### FN — Fabrinet — **7.3% above bear ($450)**

| Ticker | Current | Daily $ | Daily % | Bear | vs Bear |
|--------|---------|---------|---------|------|---------|
| FN | $482.74 | +$8.10 | +1.71% | $450 | +$32.74 (+7.3%) |

Watch zone threshold: $495. Closed further inside the buffer vs 1306 snapshot ($484.13). No company-specific catalyst; small upward drift on AI optics tailwind. Next earnings August 18; LITE Aug 11 print is primary read-through.

---

## Full Watch-List Close Snapshot

| Ticker | Current | Daily % | Bear | vs Bear |
|--------|---------|---------|------|---------|
| AMAT | $595.51 | +3.50% | $375 | +58.8% |
| ANET | $182.54 | +0.77% | $90 | +102.8% |
| APLD | $28.46 | −1.32% | $20 | +42.3% |
| AVGO | $389.04 | +1.30% | $350 | +11.2% |
| BE | $243.35 | +4.22% | $120 | +102.8% |
| CAT | $933.82 | +0.25% | $620 | +50.6% |
| **CCJ** | **$91.57** | **+1.52%** | **$85** | **+7.7% ⚠️** |
| CEG | $256.51 | −0.41% | $220 | +16.6% |
| CLS | $344.83 | −0.10% | $250 | +37.9% |
| DLR | $173.13 | −2.69% | $140 | +23.7% |
| **FN** | **$482.74** | **+1.71%** | **$450** | **+7.3% ⚠️** |
| GEV | $1,066.92 | +2.33% | $600 | +77.8% |
| GNRC | $225.05 | −0.84% | $175 | +28.6% |
| HUBB | $483.74 | +1.41% | $320 | +51.2% |
| IRM | $122.64 | +0.22% | $100 | +22.6% |
| **LITE** | **$814.78** | **+6.07% 🔴** | **$600** | **+35.8%** |
| LRCX | $346.32 | +4.97% | $200 | +73.2% |
| MOD | $229.59 | −2.00% | $150 | +53.1% |
| MP | $50.78 | +2.59% | $35 | +45.1% |
| MRVL | $222.50 | +2.28% | $180 | +23.6% |
| **NBIS** | **$194.00** | **−7.84% 🔴** | **$80** | **+142.5%** |
| NRG | $138.34 | −0.82% | $110 | +25.8% |
| SPXC | $218.35 | +1.49% | $150 | +45.6% |
| VRT | $303.67 | −0.72% | $220 | +38.0% |
| VST | $158.39 | +0.17% | $145* | +9.2%* |
| XYL | $121.59 | +0.31% | $85 | +43.0% |

*VST: frontmatter `bear_price: 145` is stale; body text operative bear is **$105** (50.4% above). Not a live condition-B alert. Frontmatter fix flagged in 1306 note.*

---

## Standing Level Alerts — All Clear

| Alert | Trigger | Close | Status |
|-------|---------|-------|--------|
| EME add-zone | ≤$660 | $774.65 (+1.27%) | Clear — 17.4% above trigger |
| MU re-underwrite | ≤$900 | $982.64 (+4.87%) | Clear — 9.2% above trigger |
| AVGO bear floor | ≤$350 | $389.04 (+1.30%) | Clear — 11.2% above floor |

---

*Prices and bear-case distances only — no position data included.*
