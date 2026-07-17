# Intraday Alert — 2026-07-17 12:05 CT

## What fired
- **Condition (a):** 2 Buy-rated names moving >±5% intraday: **BE (+6.64%)** and **NBIS (+5.87%)**. Both remain in the >5% band that first triggered earlier this session (BE +6.34% / NBIS +5.96% at 11:07).
- **Condition (b):** Four names within 10% of their (frontmatter) bear-case price: **CCJ (+1.46%)**, **FN (+5.24%)**, **MRVL (+7.41%)**, **AVGO (+7.56%)**. All four have drifted slightly further from bear vs. the 11:07 read, consistent with the broader tape firming into midday.
- **Condition (c):** Identifiable, name-specific catalysts behind both condition (a) movers — see "Why it's moving" below.
- **Condition (d) — standing level alerts:**
  - **MU $900 close protocol:** already **FIRED** on the 2026-07-16 official close ($853.20, per [[Close_Check_2026-07-16]]). Today's intraday price ($896.23, +5.04% on the day) remains below the $900 floor — consistent with the already-fired state, not a fresh trigger. Re-underwrite checklist ([[MU_ReUnderwrite_Prep_2026-07-16]]) remains open, anchored to the July 24 SK Hynix print. See also Decisions Log 2026-07-07.
  - **EME add-zone (≤$660):** not reached. Current $739.25, 12.0% above the add zone.
  - **AVGO bear floor (<$350):** not breached (close-based protocol). Current $376.45, 7.6% above the floor — captured under condition (b) proximity, not the standing floor itself.

## Data-quality flag (for review, not an alert condition)
**VST frontmatter `bear_price` is stale.** Frontmatter carries $145, but the company note's §11 explicitly re-underwrote the bear case to **~$105** on 2026-06-23 ("prior $145 figure was a placeholder... retired"). Using the stale $145, VST reads +8.14% from bear (would qualify for condition b); using the correct $105, VST is +49.3% from bear (not close). VST is **excluded** from the condition (b) list below on that basis. This mirrors the CCJ frontmatter fix already logged on 2026-07-13 — recommend the same correction be applied to VST.md frontmatter.

## Why it's moving
Tape-wide: financial media is characterizing today as a continuation of the multi-day AI-infrastructure/semiconductor "shakeout" (Zacks: "highest volatility recorded in decades"; AMD -5%, Intel -4%, Nvidia -3% intraday before partial recoveries, per 24/7 Wall St). BE and NBIS are the two clearest outliers, both bouncing off sharp prior-session declines on name-specific catalysts: NBIS announced a $775M first secured debt facility (backed by deployed GPU infrastructure and contracted cash flows) to fund its AI cloud build-out, though Jim Cramer said on air today NBIS is "not done going down" — sentiment is mixed, and neocloud peers (IREN, CoreWeave) remain in the same "free fall" narrative per Invezz. BE's move follows a $1.7B project investment from Industrial Development Funding and Oaktree (announced 7/16) to deploy Bloom fuel cells for AI infrastructure, explicitly tied to powering Nebius's compute build-out — a direct, name-specific positive catalyst after BE hit a 52-week-plus low this week ("$40 billion wipeout," Invezz). No fresh name-specific negative catalyst found today for AVGO, CCJ, FN, or MRVL; their bear-proximity reflects the same sector-wide capex-slowdown/memory-oversupply/rotation narrative that has compressed the whole cluster over the past several sessions.

## Portfolio snapshot (Buy watch list + EME/MU standing-alert names)

| Ticker | Current | Daily % | Bear | vs Bear |
|---|---|---|---|---|
| APLD | $25.63 | −3.08% | $20.0 | +28.1% |
| AMAT | $545.36 | −2.78% | $375.0 | +45.4% |
| EME | $739.25 | −1.44% | $480.0 | +54.0% |
| CCJ | $86.24 | −1.28% | $85.0 | +1.5% |
| XYL | $124.01 | −1.03% | $85.0 | +45.9% |
| LRCX | $317.78 | −0.99% | $200.0 | +58.9% |
| NRG | $131.67 | −0.81% | $110.0 | +19.7% |
| SPXC | $215.74 | −0.10% | $150.0 | +43.8% |
| CLS | $303.64 | −0.07% | $250.0 | +21.5% |
| DLR | $173.78 | +0.10% | $140.0 | +24.1% |
| VRT | $295.45 | +0.46% | $220.0 | +34.3% |
| AVGO | $376.45 | +0.53% | $350.0 | +7.6% |
| ANET | $169.68 | +0.66% | $90.0 | +88.5% |
| CEG | $253.58 | +0.72% | $220.0 | +15.3% |
| MP | $45.83 | +0.81% | $35.0 | +30.9% |
| CAT | $888.28 | +1.27% | $620.0 | +43.3% |
| GNRC | $218.47 | +1.43% | $175.0 | +24.8% |
| HUBB | $489.03 | +1.45% | $320.0 | +52.8% |
| IRM | $123.62 | +1.61% | $100.0 | +23.6% |
| GEV | $1,061.98 | +2.49% | $600.0 | +77.0% |
| MOD | $231.90 | +2.51% | $150.0 | +54.6% |
| MRVL | $193.34 | +2.68% | $180.0 | +7.4% |
| VST | $156.80 | +2.78% | $105.0* | +49.3%* |
| FN | $473.57 | +2.91% | $450.0 | +5.2% |
| LITE | $737.92 | +4.49% | $600.0 | +23.0% |
| MU | $896.23 | +5.04% | $800.0 | +12.0% |
| NBIS | $181.86 | +5.87% | $80.0 | +127.3% |
| BE | $220.46 | +6.64% | $120.0 | +83.7% |

*VST bear case shown as the corrected $105 (company note §11, re-underwritten 2026-06-23), not the stale $145 frontmatter value — see data-quality flag above. VRT bear case ($220) is from the company note's Bear Case section (§9), not frontmatter — no `bear_price` frontmatter field on file.

## Names within 10% of bear case (condition b)
- **CCJ** — $86.24 vs. $85 bear (+1.5%). Close-based re-underwrite protocol remains armed (7/13); only a settled close below $85 fires it. Yesterday's close was $87.37, +2.8% above.
- **FN** — $473.57 vs. $450 bear (+5.2%). No FN-specific news found; moving with the broader networking/optics complex.
- **MRVL** — $193.34 vs. $180 bear (+7.4%). Same capex-slowdown/memory-oversupply narrative as recent sessions; no new name-specific catalyst.
- **AVGO** — $376.45 vs. $350 bear (+7.6%). No new AVGO-specific negative catalyst found today; MarketBeat piece questioning valuation, Motley Fool piece arguing to buy the dip — no consensus shift.

## Not triggered (checked, for completeness)
- EME: $739.25 vs. $660 add-zone — 12.0% above, not reached.
- AVGO: $376.45 vs. $350 bear floor — 7.6% above, not breached (distinct from the condition-b proximity flag above; close-based protocol).
- VST: using the correct re-underwritten bear ($105), VST is +49.3% from bear — not close (see data-quality flag).

## Flag for review
No rating, PT, or bear-case changes made. (1) VST.md frontmatter `bear_price` is stale ($145 vs. the correct $105 re-underwritten 2026-06-23) — recommend correcting, per the precedent already set for CCJ on 7/13. (2) BE and NBIS remain >5% on identifiable, name-specific catalysts layered on top of sector-wide AI-infrastructure volatility — worth assessing bounce vs. durable reversal. (3) Bear-proximity cluster (CCJ, FN, MRVL, AVGO) is unchanged in composition from the 11:07 alert, drifting modestly away from bear as the tape firms into midday. (4) Carried open item: MU re-underwrite checklist pending, anchored to the July 24 SK Hynix print.

---
Prices and bear-case distances only — no position data included.
