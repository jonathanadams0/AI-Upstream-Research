---
date: 2026-06-26
type: thesis-invalidation-check
loop: thesis-invalidation-bear-breach
run: weekly
tags: [stress-test, invalidation, bear-case, weekly]
---

# Thesis Invalidation + Bear-Case Breach Check
*June 26, 2026 | Automated weekly loop | For human review — no ratings changed*

---

## Summary Scorecard

| Thesis | Triggers Checked | Any Fired? | Near-Firing? | Bear-Case Status |
|---|---|---|---|---|
| Gas Turbine Backlog (GEV) | Backlog cancellations, deposit forfeitures, hyperscaler capex cut >20% | ❌ None | — | GEV 81% above bear |
| Nuclear Renaissance (CCJ, CEG) | Nuclear incident, hyperscaler capex mod., SMR delays | ❌ None | — | CCJ +22%; CEG +22% |
| WFE Supercycle (LRCX, AMAT, KLAC) | WFE estimate cut >15%, memory capex cut >20% | ❌ None | — | LRCX +101%; AMAT +78% |
| AI Cooling Pure-Play (VRT) | Orders cut >15%, gross margin <30%, hyperscaler pause | ❌ None | ⚠️ Hyperscaler sentiment | VRT +48% above bear |
| AI Cluster Networking (ANET, CRDO) | Capex deceleration, cluster build deceleration | ❌ None | ⚠️ Networking selloff | ANET +18% — approaching |
| Custom Silicon (AVGO, MRVL) | Google/Meta exit from AVGO, AI revenue cut >15% | ❌ None | ⚠️ AVGO within 10% zone | **AVGO ⚠️ +8.3% — ACTIVE WATCH** |
| Memory Bottleneck (SNDK, MU) | NAND spot decline, NBM renegotiation | ❌ None | — | — |
| HBM Supply Constraint | HBM inventory digest, Samsung exec failure | ❌ None | — | — |
| Miners to AI Hosts (APLD) | CoreWeave anchor risk | ❌ None | — | APLD +105% above bear |
| Rare Earth Decoupling (MP) | Policy reversal, US-China deal | ❌ None | — | MP +89% above bear |
| Copper Structural Deficit (FCX, SCCO) | Recession demand destruction, major new supply | ❌ None | — | FCX +76% above bear |
| SiC Power Conversion (WOLF) | WOLF financial distress | ❌ None | — | — |
| Fuel Cells / On-Site Power (FCEL, BE) | Interconnection queue resolution | ❌ None | — | FCEL below bear (Hold/closed) |
| Transformer Supply Crunch (HUBB, ETN) | GOES capacity additions, demand destruction | ❌ None | — | HUBB +19% — approaching |
| Uranium Supply-Demand (CCJ) | Spot <$70/lb, new-build cancellations, Westinghouse delays | ❌ None | — | CCJ +22% above bear |
| Liquid Cooling Mass Adoption (VRT) | Same as AI Cooling above | ❌ None | — | — |

**Primary alert this week: AVGO at $378.91 — 8.3% above $350 bear case. Only name inside the 10% watch zone among active-rated positions.**

---

## Section A: Invalidation Triggers — Status by Thesis

### 1. Gas Turbine Backlog Pricing Power (GEV)

**Sell triggers (extracted from GEV company note; thesis file lacks explicit section — see §C):**
1. Gas turbine backlog reverses: net cancellations or deposit forfeitures visible in 10-Q
2. Two+ hyperscalers cut 2027 data center capex >20%
3. Equipment EBITDA margin stalls below 11% for two consecutive quarters

**7-day check (Jun 19–26):**
Status: **❌ NOT FIRED — thesis strongly intact.**

News is uniformly positive. Microsoft disclosed purchase of seven GE Vernova gas turbines for a Texas data center built with Chevron (CNBC, Jun 24). Multiple sources report gas turbine prices up ~300% over three years as AI data center demand creates supply scarcity. GEV Q2 2026 earnings (July 22) will be the first 10-Q opportunity to review backlog composition and deposit status. No backlog reversals, cancellations, or hyperscaler capex announcements this week.

**Gap flagged:** 01_Theses/Gas Turbine Backlog Pricing Power.md contains no explicit "Change Rating to Hold/Sell If" section. Triggers above were reconstructed from the GEV company note. This is a documentation gap — see Action Item #2.

---

### 2. Nuclear Renaissance via Hyperscaler PPAs (CCJ, CEG)

**Named invalidation conditions (thesis file):**
1. Major nuclear incident anywhere in the world
2. Hyperscaler capex moderation (sustained, not one-quarter)
3. Breakthrough in grid-scale storage
4. SMR cost or schedule failures

**CCJ sell triggers:**
1. Uranium spot price <$70/lb for two consecutive quarters
2. Two+ nuclear new-build projects cancelled or deferred past 2030
3. Westinghouse SMR licensing delays >2028

**CEG sell triggers:**
1. Adverse PJM ruling against behind-the-meter co-location (CIFP proceeding)
2. Calpine EBITDA below $1.5B
3. Nuclear capacity factor drops below 90% for two consecutive quarters

**7-day check (Jun 19–26):**
Status: **❌ NOT FIRED — signals running strongly positive.**

The most important nuclear policy event in years occurred this week: DOE announced a conditional commitment for up to $17.5B in loans to fund Westinghouse AP1000 long-lead-time supply chain items (Jun 23). Cameco and Westinghouse both issued press releases welcoming the program. This directly addresses the "Westinghouse SMR licensing delays" risk — the AP1000 program is being accelerated, not delayed. Constellation filed license renewal applications for Ginna Clean Energy Center and Nine Mile Point Unit 1 through 2049 (Business Wire, Jun 26), demonstrating proactive fleet extension. No adverse PJM CIFP ruling. No nuclear incidents. No new-build cancellations.

Uranium spot price: **cannot be auto-checked via this connector** — uranium futures not listed. See Action Item #3.

---

### 3. WFE Supercycle (LRCX, AMAT, KLAC)

**Sell triggers:**
1. WFE industry estimate revised down >15% by SEMI or major sell-side analysts
2. Memory customer capex cuts >20% YoY in a single quarter
3. China revenue <20% AND alternative markets fail to offset

**7-day check (Jun 19–26):**
Status: **❌ NOT FIRED — positive product and institutional signals.**

Applied Materials announced a suite of new chipmaking systems targeting DRAM and advanced packaging for AI chips at its own product event (Jun 25) — new epitaxy systems for DRAM, CMP/deposition for HBM stacking, and eBeam metrology for advanced packaging. This is a direct read-through to the HBM supply constraint and packaging demand vectors in the WFE thesis. Separately, AMAT shares rose 9% intraday on a strong institutional buy signal (Benzinga, Jun 26). LRCX was cited by Zacks as an "earnings growth + price strength" stock. No analyst cuts to WFE estimates >15% found. Book-to-bill data not available between quarterly earnings.

KLAC note: Post-split pricing issue open. Post-split price ~$258.8 vs. pre-split PT $1,950 (post-split equivalent ~$244). PT is nominally breached on a pre-split basis — **this is a documentation error requiring PT update, not a thesis invalidation.** See Action Item #4.

---

### 4. Vertiv AI Cooling Pure-Play / Liquid Cooling Mass Adoption (VRT)

**Sell triggers:**
1. Orders guidance cut >15% in any single quarter
2. Gross margin sustained below 30%
3. AI cluster deployment pace slows materially at 2+ of top-5 hyperscalers

**7-day check (Jun 19–26):**
Status: **❌ NOT FIRED — no hard trigger, but watch hyperscaler sentiment.**

No orders guidance cut, no margin disclosure, and no hyperscaler construction pause this week. MSFT stock is down 25–30% from its all-time high, but this is a price/sentiment event. The GEV-Microsoft turbine purchase (seven turbines for a Texas data center, Jun 24) confirms MSFT data center construction is actively proceeding — a direct disconfirmation of the "hyperscaler construction pause" trigger. VRT rating is "Under Review"; bear case $220 is 48% below current $325.57.

The July hyperscaler earnings season (MSFT, GOOG, AMZN, META all report late July 2026) is the next hard test for the cluster-build-pace trigger.

---

### 5. AI Cluster Networking (ANET, CRDO)

**Sell triggers:**
- Capex deceleration reduces new cluster builds materially (>20%)
- Credo (CRDO) revenue stalls as new-market creator

**7-day check (Jun 19–26):**
Status: **❌ NOT FIRED — but networking names under price pressure.**

MarketWatch (Jun 26): "AI's most explosive hardware trades are hitting a wall. Optical and memory stocks are falling." CRDO is among the names referenced in the optical/networking selloff. This is price-level pressure driven by sentiment (OpenAI/SpaceX IPO hype redirecting AI investment away from picks-and-shovels), not a fundamental capex cut announcement.

ANET at $165.45 is 18.2% above its $140 bear case. It is approaching the 20% outer boundary of the watch zone. Not yet flagged, but if networking selloff continues and ANET approaches $155 (10.7% above bear), it enters the 10% alert zone. See Action Item #6.

---

### 6. Custom Silicon (AVGO, MRVL)

**Sell triggers:**
1. Google or Meta publicly discloses transition away from Broadcom for next-gen ASIC development
2. AI semiconductor revenue guidance cut >15%
3. VMware integration costs exceed $2B annually for two or more consecutive years

**7-day check (Jun 19–26):**
Status: **❌ NO TRIGGER FIRED — but AVGO enters bear-case watch zone.**

This is the most significant finding of this week's loop. Broadcom is down >22% from its all-time high (Motley Fool, Jun 26). The current price of $378.91 is 8.3% above the $350 bear case — inside the 10% watch threshold.

**The reason for the decline is not a trigger:** Broadcom's FY2026 Q2 earnings beat on revenue and EPS, but the company did not raise its FY2027 AI chip revenue guidance. Failure to raise ≠ guidance cut. Sell trigger #2 requires a >15% downward guidance revision; that has not occurred.

**Contrary to the bear narrative, a new ASIC engagement was announced this week:** Broadcom and OpenAI unveiled the "Jalapeno" AI chip (Zacks, Jun 26), a custom ASIC for inference workloads with deployment targeted for late 2026. This is a net-new design win — counter to the thesis invalidation scenario. The thesis is intact.

MRVL: Q1 FY2027 operating cash flow reached a record $638.8M, up nearly 2x YoY. Custom silicon demand across the book (Alphabet, Amazon, Microsoft) remains intact. New CFO insider sale flagged by Barron's is routine (first post-hire open-market transaction).

See Section B for full bear-case breach analysis.

---

### 7. Uranium Supply-Demand Inflection (CCJ) — *see also Nuclear Renaissance §2 above*

Status: **❌ NOT FIRED.** DOE AP1000 loan program (Jun 23) is structurally bullish for uranium demand multi-year. No new-build cancellations. Uranium spot not accessible via connector — manual check required. See Action Item #3.

---

### 8. Transformer Supply Crunch (HUBB, ETN)

**Named invalidation conditions:**
1. Meaningful GOES (grain-oriented electrical steel) capacity additions announced
2. Demand destruction from recession
3. Modular or alternative grid architectures materially reducing large power transformer demand

**7-day check:**
Status: **❌ NOT FIRED.** No new GOES capacity announcements. Grid infrastructure news broadly bullish on AI data center power demand. HUBB at $536.04 is 19.1% above its $450 bear case — approaching the outer watch boundary. See Action Item #6 addendum.

---

### 9. Miners to AI Hosts (APLD, CORZ/CRWV)

Status: **❌ NOT FIRED.** CORZ acquisition by CoreWeave (CRWV) remains a closed deal. No CRWV credit deterioration news this week. CRWV credit monitoring per Jun 23 checklist — no new signals.

---

### 10. SiC Power Conversion (WOLF financial risk)

Status: **❌ NOT FIRED.** No new Wolfspeed financial distress signals this week.

---

### 11. Fuel Cells and On-Site Power (FCEL, BE)

Status: **❌ NOT FIRED for thesis.** FCEL at $19.65 is below its $20 bear case, but FCEL is a Hold/closed position as of Jun 23 — not an active thesis position. BE no news this week. Interconnection queue remains structurally long; thesis premise unchanged.

---

### 12. Rare Earth Decoupling from China (MP)

Status: **❌ NOT FIRED.** No US-China rare earth deal. No executive order reversals. Policy and tariff regime unchanged this week.

---

### 13. HBM Supply Constraint

Status: **❌ NOT FIRED.** AI chip selloff today is IPO-euphoria-driven (OpenAI/SpaceX), not a fundamental HBM demand deterioration signal. Micron lifted market sentiment mid-week (Jun 25) with positive earnings read-through per 247wallst. No HBM inventory build reports.

---

### 14. Memory Bottleneck (SNDK, MU)

Status: **❌ NOT FIRED this week.** SNDK key datapoint is Q4 FY2026 earnings (August 13). NAND spot price not pulled this week — TrendForce monthly data should be checked. Micron (MU) appears to have had a strong recent print per market commentary.

---

### 15. Copper Structural Deficit (FCX, SCCO)

Status: **❌ NOT FIRED.** No large mine supply additions announced. New macro risk this week: US military strikes on Iranian targets after ship attack in Strait of Hormuz (WSJ, Jun 26). Potential impact: oil price spike, global trade disruption sentiment. Indirect risk to copper demand via global macro — not a named thesis trigger. Monitor next week.

---

## Section B: Bear-Case Breach Watch List

All names flagged at or below bear case, or within 10% above it. Prices from frontmatter (current as of 2026-06-26 weekly refresh).

| Name | Current Price | Bear Case | % Above Bear | Status | Action |
|---|---|---|---|---|---|
| **AVGO** | $378.91 | $350 | **+8.3%** | ⚠️ **ACTIVE WATCH** | See §C #1 |
| ANET | $165.45 | $140 | +18.2% | 🟡 Approaching | Watch; add if reaches $155 |
| HUBB | $536.04 | $450 | +19.1% | 🟡 Approaching | Transformer thesis intact |
| CCJ | $103.58 | $85 | +21.8% | 🟢 Clear | DOE AP1000 bullish; no trigger |
| CEG | $268.69 | $220 | +22.1% | 🟢 Clear | License renewals; no CIFP ruling |
| VRT | $325.57 | $220 | +48.0% | 🟢 Clear | Rating under review |
| VST | $167.77 | $105 | +59.8% | 🟢 Clear | Cogentrix H2 2026 on track |
| FCX | ~$105 | ~$60 | ~+75% | 🟢 Clear | — |
| AMAT | $668.0 | $375 | +78.1% | 🟢 Clear | New products; +9% buy signal |
| GEV | $1,085.47 | $600 | +80.9% | 🟢 Clear | MSFT turbine deal; no cancellations |
| LRCX | $401.82 | $200 | +100.9% | 🟢 Clear | No WFE estimate cuts |
| FCEL | $19.65 | $20 | **−1.8%** | 🔴 Below Bear | Hold/closed (Jun 23 miss); no action |

### AVGO Bear-Case Breach — Detail

AVGO at $378.91 is the sole active-rated position inside the 10% bear-case watch zone.

**What would confirm the bear case ($350):**
- Google or Meta publicly announces next-gen ASIC development with a non-Broadcom partner
- AVGO FY2027 AI chip revenue guidance cut >15% (not merely failure to raise)
- VMware integration charges exceed $2B annually in FY2027 guidance

**What argues against the bear being reached on fundamentals:**
- OpenAI/Jalapeno chip: brand-new custom ASIC engagement announced this week, deploying late 2026 — adds a third major hyperscaler-class customer
- FY2026 Q2 earnings beat on revenue and EPS; the selloff is a "guidance didn't raise" reaction, not a thesis deterioration
- MRVL's record cash flow confirms the same AI silicon demand vector that underpins AVGO
- Bull case per Gil Luria (Schwab Network, Jun 26): AVGO running on all cylinders; Alphabet partnership ramping

**What the $378→$350 path looks like:** Would require the broader AI hardware selloff to deepen further without a positive fundamental catalyst, or a specific customer defection news item. At $350, the thesis would require immediate re-review per the sell-trigger framework.

**FCEL note:** FCEL at $19.65 is technically below its $20 bear case. This is flagged for completeness but FCEL is a closed position following the Hold miss determination on Jun 23. No action.

---

## Section C: Action Items

**Priority 1 — AVGO position review**

AVGO ($378.91) is inside the 10% bear-case watch zone. No sell trigger has fired. The Jalapeno/OpenAI chip is constructive for the thesis. However, per the position sizing framework, proximity to bear case at the current Tier level warrants a PM review of sizing. **If AVGO trades at or through $360 (~5% below current) on continued weakness without a trigger-qualifying news event, schedule a full thesis re-review within 48 hours.** The next hard fundamental catalyst is Broadcom Q3 FY2026 earnings (September 2026), where the $16B AI chip revenue guide will be measured against actuals.

**Priority 2 — Gas Turbine thesis: add sell-trigger section**

01_Theses/Gas Turbine Backlog Pricing Power.md has no explicit "Change Rating to Hold/Sell If" section. This creates a gap in the weekly loop's ability to auto-check this thesis. The triggers are defined at the company level (GEV note §11) and should be synthesized and added to the thesis file. Low urgency (thesis strongly intact), but documentation quality flag.

**Priority 3 — Uranium spot price: manual check needed**

The uranium spot price (trigger threshold: <$70/lb for two consecutive quarters) is not accessible via the FMP connector — no uranium futures symbol is available in the commodities list. This trigger must be manually checked via Cameco investor relations page, TradingEconomics, or Sprott Physical Uranium Trust (U.UN) NAV. Add a manual uranium spot step to this loop or link to an external monitor. Until resolved, the CCJ uranium spot trigger cannot be confirmed clear by automation.

**Priority 4 — KLAC PT update (High priority)**

KLAC underwent an 8:1 stock split approximately June 2026. Post-split price is ~$258.8; pre-split PT was $1,950 (post-split equivalent ~$244). KLAC is therefore nominally above its pre-split-equivalent PT. This is a documentation error — the vault's KLAC PT needs to be updated to a post-split figure before the next earnings. This was flagged as "under review" in the prior session. **Resolve before KLAC Q4 FY2026 earnings.**

**Priority 5 — July hyperscaler earnings are the next systemic test**

MSFT, GOOG, AMZN, and META all report in late July 2026. Current AI hardware weakness (AVGO, CRDO, optical names) is entirely sentiment-driven — no hyperscaler has cut capex guidance this week. The GEV-MSFT turbine purchase (7 turbines, Texas data center, Jun 24) is a concrete real-world capex action confirming construction continues. July earnings are the next hard fundamental check for: VRT (orders trigger), GEV (hyperscaler capex trigger), CEG (co-location demand), ANET/CRDO (cluster build pace), and AVGO (AI chip demand trajectory). All thesis holders should be prepared to re-run this stress test immediately after each hyperscaler report.

**Priority 6 — ANET and HUBB approaching outer watch boundary**

Neither ANET (+18.2% above bear) nor HUBB (+19.1% above bear) has entered the 10% watch zone. However, if the AI hardware and industrial selloff continues, these could approach the zone by next week's loop. Pre-flag: add both to the leading indicator list for the Jul 3 run.

**Priority 7 — Iran/Strait of Hormuz: new tail risk, no trigger**

US struck Iranian targets after an Iranian attack on a vessel in the Strait of Hormuz (WSJ, Jun 26). Not a named thesis trigger for any name in the vault. Potential second-order effects: oil price spike (positive for VST ERCOT merchant margins, not a sell signal); global trade disruption risk (copper demand watch for FCX/SCCO); broader market risk-off sentiment (amplifies current AI hardware weakness). Monitor next week; escalation could trigger an unscheduled stress-test run.

---

## Macro Context — Not a Named Trigger

Tech and AI stocks had one of their worst weeks of 2026. The S&P 500 and Nasdaq fell every session (WSJ, Jun 26). The selloff driver appears to be a confluence of: (a) OpenAI/SpaceX IPO excitement redirecting speculative capital away from AI hardware names, (b) AVGO's failure to raise FY2027 guidance disappointing momentum traders, and (c) broader investor questions about AI capex ROI. None of these constitute a named thesis trigger across the vault. The correct framing: **this is a sentiment repricing event, not a fundamental thesis invalidation event.** The most important fundamental check — July hyperscaler capex disclosures — has not yet occurred.

The Broadcom-OpenAI "Jalapeno" chip announcement (Jun 26) and the Microsoft-GEV turbine purchase (Jun 24) are the two most important thesis-confirming data points from this week, both of which run counter to the bearish sentiment narrative.

---

*Next run: 2026-07-03 | Companion: [[Thesis_Stress_Test_2026-06-23]] | Vault: [[08_Monitors]]*
