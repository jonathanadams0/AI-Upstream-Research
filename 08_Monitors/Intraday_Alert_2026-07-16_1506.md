# Intraday Alert — 2026-07-16 15:06 CT

## What fired
- **Condition (a):** 9 Buy-rated names moved >±5% intraday: APLD, AVGO, BE, CLS, FN, LITE, MP, MRVL, NBIS. (VST and VRT rolled off this hour at -4.8% and -3.4%, down from -5.5%/-4.9% at 14:06.)
- **Condition (b):** 6 names trading within 10% of their bear-case price: AVGO (+7.0%), CCJ (+2.8%), FN (+2.3%), MRVL (+4.6%), VST (+5.2%), MU (+6.7% vs. the $800 frontmatter bear) — same set as the 14:06 note, no new names added.
- **Condition (c):** Material news catalyst confirmed on Buy names — see below.
- **Condition (d) — standing level alerts:** MU last trade $853.66, further below the $900 re-underwrite floor (was $847.58 at 14:06). **Still not fired.** Per the staged protocol (08_Monitors/MU_ReUnderwrite_Prep_2026-07-16.md), this executes only on the official settled close (16:00 ET / 15:00 CT). The regular session just ended (last trade stamped 14:59:59 CT) but this data pull still carries yesterday's (7/15) settled close field — no official 7/16 close is available yet. **Close-check against the $900 gate is the next actionable step**, likely on the next scheduled run once a settled quote posts.
- EME add-zone ($660) and AVGO bear-floor ($350) checked — neither triggered (EME $750.02, 13.6% above; AVGO $374.46, 7.0% above — captured under condition (b), not the standing floor).

## Why it's moving
No new incremental catalyst since the 14:06 note — this remains the same second-session AI-infrastructure/semiconductor selloff. Root trigger is TSMC's Q2 print and capex commentary: TSMC beat with record profit, but guided to heavier capital investment, and the market read-through is a valuation/expectations reset across the AI capex chain rather than fresh demand deterioration (Investopedia: "The Chip-Stock Slide Isn't Over. The AI Trade Is Still Under Pressure."). Marvell-specific coverage continues to cite AI capex-slowdown fears directly, with read-through cited into Broadcom, AMD, and Intel (24/7 Wall St: "Marvell Drops 8% as AI Capex Slowdown Fears Weigh on Chips"). Nebius (NBIS) remains down double digits despite unveiling its Echo AI agent and an asset-light cloud model today — 24/7 Wall St frames this explicitly as "the neocloud trade unravels," i.e., sector-beta selling in data-center/cloud names, not name-specific bad news. Bloom Energy (BE) remains the standout divergence, down double digits despite today's positive $1.7B IDF/Oaktree fuel-cell financing tied to Nebius's buildout — sector beta plus the still-pending 7/15 Schall Law fraud-investigation notice continue to swamp the positive headline. Nothing in today's flow trips a Step 2/3 bear-thesis trigger on the MU prep checklist (no second sequential gross-margin decline, no HBM4 slip, no new China restriction disclosure).

## Portfolio snapshot (Buy watch list + EME/MU standing-alert names)

| Ticker | Current | Daily % | Bear | vs Bear |
|---|---|---|---|---|
| APLD | $26.43 | -9.0% | $20.0 | +32.2% |
| BE | $206.51 | -13.7% | $120.0 | +72.1% |
| CLS | $303.75 | -9.3% | $250.0 | +21.5% |
| LITE | $706.37 | -6.1% | $600.0 | +17.7% |
| MP | $45.47 | -8.1% | $35.0 | +29.9% |
| MRVL | $188.35 | -8.7% | $180.0 | +4.6% |
| NBIS | $171.72 | -13.9% | $80.0 | +114.7% |
| VST | $152.54 | -4.8% | $145.0 | +5.2% |
| AVGO | $374.46 | -5.0% | $350.0 | +7.0% |
| CCJ | $87.37 | -4.0% | $85.0 | +2.8% |
| FN | $460.22 | -5.4% | $450.0 | +2.3% |
| MU | $853.66 | -5.6% | $800.0 | +6.7% |
| AMAT | $560.86 | -3.2% | $375.0 | +49.6% |
| ANET | $168.57 | -2.0% | $90.0 | +87.3% |
| CAT | $877.77 | -4.0% | $620.0 | +41.6% |
| CEG | $251.71 | -2.5% | $220.0 | +14.4% |
| DLR | $173.57 | -1.4% | $140.0 | +24.0% |
| GEV | $1036.01 | -1.8% | $600.0 | +72.7% |
| GNRC | $215.62 | -4.8% | $175.0 | +23.2% |
| HUBB | $482.11 | +0.5% | $320.0 | +50.7% |
| IRM | $121.66 | -1.5% | $100.0 | +21.7% |
| LRCX | $320.98 | -4.3% | $200.0 | +60.5% |
| MOD | $226.49 | -2.4% | $150.0 | +51.0% |
| NRG | $132.53 | -3.9% | $110.0 | +20.5% |
| SPXC | $216.08 | -0.7% | $150.0 | +44.1% |
| VRT | $294.21 | -3.4% | $220.0 | +33.7% |
| XYL | $125.27 | +3.2% | $85.0 | +47.4% |
| EME | $750.02 | -2.6% | $480.0 | +56.3% |

## Names within 10% of bear case (condition b)
- **NBIS**, **BE**, **CLS**, **LITE**, **MP**, **APLD** — all >5% movers this hour, none within 10% of bear (see table). Listed here only to confirm they were checked.
- **MRVL** — $188.35 vs. $180 bear (+4.6%). Also a >5% mover (-8.7%). Same capex-slowdown narrative, no new incremental development this hour.
- **FN** — $460.22 vs. $450 bear (+2.3%). Also a >5% mover (-5.4%). No name-specific catalyst found; moving with the broader optics/networking complex.
- **AVGO** — $374.46 vs. $350 bear (+7.0%). No negative name-specific news found today; sector-beta drag, not thesis-relevant.
- **CCJ** — $87.37 vs. $85 bear (+2.8%). Already inside the watch zone per the 7/13 note; not a new development.
- **VST** — $152.54 vs. $145 bear (+5.2%). Unchanged in substance from 14:06. No VST-specific news found; power/IPP names drifting down with the broader complex.
- **MU** — $853.66 vs. $800 frontmatter bear (+6.7%), and last trade below the $900 standing re-underwrite floor — see standing alert section above. Gated to official close; not fired.

## Not triggered (checked, for completeness)
- EME: $750.02 vs. $660 add-zone — 13.6% above, not reached.
- AVGO: $374.46 vs. $350 bear floor — 7.0% above, not breached.

## Flag for review
No rating, PT, or bear-case changes made. MU close-check against the $900 re-underwrite gate remains the single open action item — needs a settled 7/16 close quote, not yet available in this data pull taken right at the closing bell.

---
Prices and bear-case distances only — no position data included.
