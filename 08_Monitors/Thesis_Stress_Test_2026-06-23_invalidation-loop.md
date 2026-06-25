---
date: 2026-06-23
type: stress-test
topic: Thesis Invalidation + Bear-Case Breach Loop (automated weekly)
related: Thesis_Stress_Test_2026-06-23.md
tags: [stress-test, invalidation, sell-triggers, bear-breach, monitor, automated-loop]
---

# Thesis Stress Test — Invalidation Triggers + Bear-Case Breach
*Automated loop run · June 23, 2026 · AI/Semi selloff day*

> **Scope note.** This is the structured **invalidation-trigger / bear-breach** loop output. It is filed alongside today's separate scenario doc [[Thesis_Stress_Test_2026-06-23]] (AI capex deceleration) rather than overwriting it; the two are companions.
>
> **Price source.** Company `current_price` frontmatter was last refreshed **2026-06-19** (last_updated tag), supplemented by the **2026-06-23 intraday** portfolio monitor for GEV/MU/SNDK. Live quote and news connectors were gated on the current data plan this run, so trigger checks below rely on web search of the trailing 7 days. **Caveat:** today (06-23) was a broad AI/semi selloff (GEV −6.6%, MU −6.0%); several semi/AI/power names are likely trading *below* the 06-19 prices used here, which would *tighten* every bear-case gap shown. Treat the bear-breach gaps as conservative (wide).
>
> **No ratings or PTs were changed by this loop.** Surfacing only.

---

## (a) Invalidation Triggers Checked

| # | Thesis / Name | Named trigger | Status (last 7 days) | Verdict |
|---|---|---|---|---|
| 1 | Gas Turbine / [[GEV]] | Backlog decline or deposit forfeitures; order-pace deceleration | Backlog **grew** to ~100 GW (from 80 GW), guided to ~110 GW by YE2026. No forfeitures. | **Not fired** (opposite). New non-thesis watch: Vineyard Wind litigation (Iberdrola >$1B countersuit). |
| 2 | Nuclear PPAs / [[CEG]] | FERC ruling **against** co-located / behind-the-meter load | FERC set to **finalize** the >20 MW large-load interconnection rulemaking **by end of June 2026** — i.e. within ~1 week. Outcome not yet published. | **NEAR-FIRING — imminent.** Single most time-sensitive trigger in the book. |
| 3 | WFE Supercycle / [[LRCX]] [[AMAT]] [[TOELY]] | Shared >15% WFE decline (China controls / memory capex cut) | 2026 WFE **revised up** (MS +5%→+10%, ~$128B); SK Hynix capex +17% ($20.5B), Samsung +11% ($20B), Samsung HBM capacity +50%. **But** China leg escalated: AMAT flags **$600–710M** FY26 revenue loss from expanded US controls; LRCX China rev falling 43%→<30%; China's **June 11** tech-transfer controls + 50% domestic-equipment mandate threaten ~$18B combined AMAT/LRCX/KLAC China revenue. | **Aggregate trigger not fired** (WFE rising). **China sub-risk firing** — the explicitly named WFE risk #1 is escalating. Monitor book-to-bill. |
| 4 | Uranium / [[CCJ]] | Spot < $70/lb **sustained**; Kazakh/Russian supply returns | Spot ~**$85/lb**, range-bound since April; LT contract ~$90; Cameco signed 22 Mlb India deal. | **Not fired** (~$15 / ~18% above trigger). |
| 5 | Rare Earth / [[MP]] | China relaxes / floods NdPr market (structural bear) | **Opposite:** China **escalated** June 22, adding MP Materials to its export-control entity list (entity-specific — limits what MP *receives*, not its sales). DoD $110/kg NdPr floor intact. | **Not fired** — thesis reinforced. Note: entity listing is a minor operational headwind, not the bear scenario. |
| 6 | Vistra / [[VST]] | PJM capacity-auction disappointment; ERCOT mild summer | Recent PJM BRAs cleared at the **cap** ($329–333/MW-day, +1.3%) — positive. Next BRA ~July 1 (calendar placeholder). | **Not fired** on auctions. (Bear-breach watch — see section b.) |
| 7 | Custom Silicon / [[AVGO]] | Q3 FY26 AI revenue miss vs ~$16B guide | Next print September 2026 — no new datapoint this week. | **Pending** (Sept). |
| 8 | Memory / [[MU]] | HBM share loss, HBM4 program slip, or China shock → exit < $900 | HBM4 certified for Nvidia Vera Rubin; Anthropic multi-year HBM deal (Jun 22); 2026 sold out. **MU prints tonight (06-23 after close).** | **Not fired** pre-print. **Re-check post-print** for 2027 HBM language. |

### Trigger-definition gaps to close
Several active theses carry only **qualitative** "Risks" sections with **no quantified sell trigger**. Recommend adding explicit, monitorable triggers to: **AI Cluster Networking**, **Liquid Cooling Mass Adoption**, **Vertiv pure-play**, **Copper Structural Deficit**, **SiC Power Conversion**, **Memory Bottleneck**, **Advanced Packaging Bottleneck**, **Fuel Cells / On-Site Power**, and **Miners-to-AI-Hosts** (CoreWeave concentration is named but not thresholded). Theses that already carry usable triggers: Gas Turbine, Nuclear PPAs, WFE Supercycle, HBM Supply Constraint, Custom Silicon, Transformer Supply Crunch.

---

## (b) Bear-Case Breach Watch List

Covered names ranked by proximity to their stated bear-case price. **No name is strictly at/below or within 10% above its bear case on the 06-19 prices** — but **VST is the clear standout at +12.9%**, and on today's selloff likely tighter (the VST note records it trading ~$151 recently, within ~4% of the $145 bear, consistent with the "has traded below it" flag). Six names sit within ~25% of bear; the rest of the book has wide cushion.

| Ticker | Current (px date) | Bear case | % above bear | Notes |
|---|---|---|---|---|
| **VST** | $163.73 (06-19) | **$145** (de-rate) / $105 (DCF) | **+12.9%** / +56% | **Tightest in book.** Two bear levels in note: $145 generic de-rate vs $105 fundamental DCF (ERCOT mild + Cogentrix delay, 9x — the ratified playbook bear). Has flirted with $145 intraday. Watch item per loop spec. |
| AVGO | $410.79 (06-19) | $350 | +17.4% | Selloff-sensitive; custom-silicon thesis intact, Q3 print not until Sept. |
| TOELY | $245.49 (06-19) | $212 (margin-squeeze) / $130 (base) | +15.8% / +89% | Closest bear is the margin-compression / China-escalation scenario — relevant given trigger #3 China escalation. |
| NRG | $135.01 (06-19) | $110 | +22.7% | Power/IPP; mild-weather + leverage bear. |
| CEG | $274.09 (06-19) | $220 | +24.6% | **Cross-references trigger #2** — an adverse FERC co-location ruling (imminent) is the live path toward this bear. |
| CCJ | $106.50 (06-19) | $85 | +25.3% | Loop spec flagged a "~10% zone"; on 06-19 prices it is **+25%**, not within 10% — would need a drop to ~$93.50 to enter the 10% band. Uranium spot ~$85 supports the gap. Keep on watch but **not** near-breach today. |
| FN | $573.88 (06-19) | $450 | +27.5% | — |
| IRM | $127.84 (06-19) | $100 | +27.8% | — |
| XYL | ~$110 (06-19) | $85 | ~+29% | — |
| DLR | $188.08 (06-19) | $140 | +34.3% | — |
| VRT | ~$318 (06-19) | $220 | +44.5% | — |
| CLS | $372.26 (06-19) | $250 | +48.9% | — |
| ON | $121.53 (06-19) | $80 | +51.9% | — |
| CAT | $985.23 (06-19) | $620 | +58.9% | — |
| GNRC | $279.32 (06-19) | $175 | +59.6% | — |
| SPXC | $242.80 (06-19) | $150 | +61.9% | — |
| HUBB | $524.14 (06-19) | $320 | +63.8% | — |
| AMAT | $616.70 (06-19) | $350–400 | ~+64% | China-leg trigger escalating but valuation cushion wide. |
| MRVL | $310.85 (06-19) | $180 | +72.7% | — |
| MP | $60.86 (06-19) | $35 | +73.9% | — |
| ANET | $169.65 (06-19) | $90 | +88% | — |
| LRCX | $388.45 (06-19) | $200 | +94% | — |
| MOD | $297.15 (06-19) | $150 | +98% | — |
| APLD | $46.57 (06-19) | $20 | +133% | — |
| BE | $328.90 (06-19) | $120 | +174% | — |
| NBIS | $287.03 (06-19) | $80 | +259% | — |
| UUUU | $16.57 (06-19) | $4 | +314% | — |

*Names with only qualitative bear cases (no single bear price) and therefore not rankable here: STX, WDC, SNDK ($400 bear far below ~$2,260 current), MU, ENTG ($85–100 range vs ~$179), INTC ($60 vs ~$134), SCCO, PWR, ETN, NVT, TT, SMNEY, FCEL, FCX.*

---

## (c) Action Items Flagged for Review

1. **CEG — FERC large-load ruling (by end of June 2026).** Highest-priority near-term trigger in the book. An adverse co-location ruling is the named CEG invalidation and the live path to its $220 bear. **Set a watch for the FERC order in the next ~7 days**; on release, run an earnings-reaction / re-underwrite pass on CEG (and read-through to co-location-exposed power names).
2. **VST — bear-case proximity.** Closest name to its bear ($145 de-rate level, +12.9% on stale 06-19 px; likely tighter post-selloff). Reconcile the **two bear levels** ($145 vs ratified $105 DCF) into one operative watch line in VST.md so future loops flag consistently. No rating change — surface only.
3. **WFE China leg (LRCX / AMAT / TOELY / KLAC).** The named "China controls" risk is **actively escalating** (AMAT $600–710M FY26 hit; China June 11 controls + 50% domestic-equipment mandate; ~$18B combined revenue exposure). Aggregate WFE is still rising, so the >15%-decline trigger is **not** fired — but flag for the next book-to-bill prints (LRCX/AMAT/KLAC) as the confirming/denying datapoint.
4. **MU — post-print re-check (tonight, 06-23 after close).** Re-run trigger #8 once results land: confirm no HBM share loss / HBM4 slip / China shock and capture 2027 HBM language. Exit condition remains < $900 on a bearish print per the MU prep note.
5. **GEV — Vineyard Wind litigation.** Not a thesis trigger, but the Iberdrola >$1B countersuit + MA injunction is a new contingent-liability risk; watch Q2 call (~July 22) for management commentary. Backlog trigger itself is firmly **not** fired.
6. **CCJ — keep on commodity watch, not near-breach.** Re-label the loop's "~10% zone" expectation: on current prices CCJ is +25% above the $85 bear and uranium spot (~$85) supports it. Would need spot < $70 sustained *and* a price drop toward ~$93 to become actionable.
7. **Close trigger-definition gaps.** Add quantified sell triggers to the 9 theses listed in section (a) so subsequent automated runs have explicit conditions to test rather than qualitative risk prose.

---

*Automated invalidation + bear-breach loop. Data: web search (trailing 7 days, 06-23-2026) + company note frontmatter (06-19 refresh) + [[portfolio_monitor_2026-06-23]]. Companion: [[Thesis_Stress_Test_2026-06-23]] (capex-deceleration scenario).*

Sources: [GE Vernova backlog to 100 GW](https://www.industrialinfo.com/iirenergy/industry-news/article/ge-vernovas-global-natural-gas-turbine-reservations-and-order-backlog-grows-to-100-gw--356705) · [FERC to finalize large-load rules by end of June 2026](https://cryptobriefing.com/ferc-data-center-grid-connection-ruling/) · [Constellation co-location complaint / FERC response](https://www.womblebonddickinson.com/us/insights/articles-and-briefings/grid-supporting-cloud-fercs-regulatory-response-data-center-co) · [Vistra PJM 2027/28 auction $333.44](https://www.stocktitan.net/sec-filings/VST/8-k-vistra-corp-reports-material-event-8ad57af4d7ba.html) · [Uranium ~$85/lb June 2026](https://investingnews.com/uranium-forecast/) · [China adds MP Materials to export-control list (June 2026)](https://www.stocktitan.net/articles/china-rare-earth-export-controls-mp-usa-rare-earth-june-2026) · [2026 WFE outlook raised; memory driver](https://www.datacenterdynamics.com/en/news/samsung-and-sk-hynix-to-scale-up-memory-production-capacity-in-2026-to-meet-ai-demand/) · [AMAT $600M+ China export-control revenue hit](https://www.alphaspread.com/market-news/regulatory-actions/applied-materials-warns-of-revenue-loss-due-to-new-us-export-restrictions-to-china) · [China June 2026 tech controls + 50% domestic-equipment mandate](https://fintool.com/news/china-50-percent-domestic-chip-equipment)
