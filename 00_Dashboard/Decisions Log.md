---
tags: [dashboard]
last_updated: 2026-06-29
---

# Decisions Log

> Every rating or PT change, recorded at the moment it's made: date, price, reasoning, methodology. The point is a measurable track record — hit rate, upside captured, and which *methodologies* actually predict. Review quarterly; score each closed decision.

---

> ### 📊 Q2 2026 Quarterly Scoring — completed 2026-06-23
>
> **Two new closes this quarter, both Holds whose PTs were breached to the upside:** **FCEL** Hold/$18 → $21.82 (+21% above PT, +31% above entry in 5 sessions) scored **~**; **INTC** Hold/$120 → $132.28 (+10% above PT; probability-weighted fair value was $106 vs $132 actual) scored **✗**. Together with the previously-scored GEV Hold/$440 (✗), **all three closed decisions to date are neutral / fair-value-anchored calls the market overran to the upside** — the same conservatism error as Lesson #1, now generalized in new **Lesson #3**.
>
> **Cumulative hit rate (n=3 scorable closes):** 0 clean hits (✓), 1 partial (~), 2 wrong (✗) → **0% on a ✓-only basis, ~17% counting ~ as half.** By methodology: DCF/comps **0/1**, thesis-driven **0/2** (one ~). No methodology has yet been validated by a closed decision. Note the counter-signal: the only individually-deliberated *Buy* (GEV upgrade to $1,200) remains **open and working** (+8% since 6/3) — the one decision that broke the conservative-anchor pattern.
>
> **Reconciliation gaps (Model Portfolio.md not updated):** AMAT PT still **$520** (should be $680), LRCX PT still **$380** (should be $450), ENTG still listed **Buy/$155** (downgraded to Hold, PT removed 6/18). CCJ net-cash and KLAC split corrections require no Model-Portfolio change (CCJ PT unchanged; KLAC not a position). **All four flagged corrections propagated correctly into the `03_Companies/*.md` notes.**
>
> *Caveat: FCEL and INTC closed only 5 sessions after initiation. The closes are valid per Rule 4 (PT hit/invalidated has no time minimum) but the methodology read should be weighted lightly given the tiny sample and short holding periods.*

**Rules:**
1. Log the decision the same day it's made. No backfilling reasoning later.
2. Record the price *at decision time* — that's the entry the decision is judged against.
3. Note the dominant methodology (DCF / comps / variant perception / screener / thesis-driven) so methodology hit rates can be computed.
4. A decision is "closed" when the rating changes again or the PT is hit/invalidated. Score: PT hit (✓), direction right but PT missed (~), wrong (✗).
5. Quarterly review: compute hit rate by methodology and by sector. Update the Lessons section.
6. **Scoring a Hold:** a Hold's PT is a fair-value estimate, not a bullish target. If the stock breaks *above* a Hold PT, the call was too conservative — score it **~** (if the note explicitly flagged the upside risk) or **✗** (if the note leaned bearish), **never ✓**. ✓ is reserved for Buy/Sell PTs reached in the intended direction. (Added 2026-06-23 to resolve the FCEL/INTC closes.)

---

## Open Decisions

| Date | Ticker | Decision | Price @ Decision | PT | Methodology | One-line reasoning | Score |
|---|---|---|---|---|---|---|---|
| 2026-05-05 | GEV | Initiate Hold/$440 | ~$995 | $440 | DCF + Tier-1 comps | DCF said $218, comps $440; no input set justified $995 | Closed 6/3 — ✗ (see Lessons #1) |
| 2026-06-03 | GEV | Upgrade Hold→Buy, PT $440→$1,200 | $959 | $1,200 | Thesis-driven (NTM P/E 35x) | 100GW backlog 3 qtrs early; May 27 pullback = overreaction; consensus $1,120 | Open |
| 2026-04-15 | CEG | Initiate Under Review | — | — | — | Calpine close + FY25 results; pending DCF | Closed 6/3 |
| 2026-06-03 | CEG | Rate Buy/$385 | $263 | $385 | DCF + variant perception | 47% below consensus PT $391; nuclear+Calpine repricing | Open |
| 2026-06-03 | VST | Initiate Buy/$230 | $151 | $230 | Variant perception | Meta+AWS PPAs, Cogentrix; stock 52% below aligned consensus | Open |
| 2026-06-03 | — | Vault-wide rating pass: 25 names rated | various | various | Mixed | Full coverage rated in one session — flag: batch decisions deserve extra scrutiny at review | Open |
| 2026-06-03 | NBIS | Initiate Buy/$310 | $263 | $310 | Aschenbrenner 13F + growth | His 2nd largest position; +599% YoY | Open |
| 2026-06-03 | TSEM | Initiate Hold/$285 | $275 | $285 | Comps | Specialty foundry; limited upside at price | Open |
| 2026-06-03 | HUT | Initiate Hold/$145 | $137 | $145 | Comps | Miner-to-host; +72% past month = entry risk | Open |
| 2026-06-03 | XYL | Initiate Buy/$135 | ~$110 | $135 | Screener | Water as DC bottleneck; near 52-wk low | Open |
| 2026-06-09 | BW | Initiate Under Review | $15.49 | — | Screener (5/5) | $2.4B APLD contract; bookings +1,900%; rating pends 10-Q + multiple | Open |
| 2026-06-09 | — | Model Portfolio inception: 29 positions, $100k, tier midpoints | 6/9 closes | — | Sizing framework | Benchmarked vs SPY ($737.05) and SMH ($591.01) same-day; 18.5% cash | Open |
| 2026-06-09 | TOELY | **Excluded from model portfolio** | $189.37 (ADR) | $403 (suspect) | Data integrity | PT appears denominated in Tokyo per-share terms, not ADR; at plausible ADR ratio PT may be *below* current price — no position until restated | Closed 6/20 |
| 2026-06-20 | TOELY | **PT reinstated at $270; ADR error resolved** | $245.49 (ADR) | $270 | Comps + variant perception | 1 ADR = 0.5 Tokyo shares; USD/JPY ~¥130. FY2026 actuals: ¥2,443.5B rev (+0.5%), EPS $4.83 ADR (trailing 51x). FY2027 H1 guide +33% YoY. Base-case FY2027 EPS ~$5.65; bull ~$6.00; PT = 45x bull = $270. Consensus $6.48 set aside — TEL stopped issuing full-year guidance, H2 visibility limited, gross margin compressed 1.8pp. 1% T4 slot still in cash; add decision pending. Bear $130 (20x $4.70 on margin compression + China escalation). | Open |
| 2026-06-18 | ENTG | Downgrade Buy→Hold, PT $155→none | $178.08 | Valuation | Stock 32.5% above entry, 15% above PT, 25%+ above consensus avg (~$133–142). EV/EBITDA ~47x on 2 years of flat revenue ($3.2B) with $3.34B net debt — no scenario in original note justifies current price. Note was Screening Mode (no DCF built). No new PT until Q2 filings reviewed and model constructed. Bear $85 unchanged. | Closed 6/25 — position exited; see 6/25 exit decision |
| 2026-06-25 | ENTG | Exit T4 (1%) position | $176.28 | — | Model Portfolio discipline | Stock +31% from $134.35 entry; near 52W high ($180.94). At base-case fair value: ~$1.0B FY2026E adj. EBITDA × 30x EV/EBITDA − $3.1B net debt / 152.5M shares ≈ $176. Revenue flat/declining 3 years ($3.5B→$3.2B); Q2 (late July) needed to confirm recovery. No defensible PT above current price on base assumptions. Proceeds $1,312 returned to cash ($15,812 total). Re-entry threshold: confirmed YoY revenue growth + PT >$200 with ≥1.5x asymmetry. Hold rating maintained on the research note. | Executed |
| 2026-06-25 | PORTFOLIO | Accept current asymmetry as-is (hedge Option 1 of 3) | — | — | Risk management | Tier-weighted book asymmetry 1.12x at inception (vs. 0.63x equal-weight per AI Capex Stress Test) — acceptable given T1 concentration in Group 3 power names (CEG/NRG/VST/GEV). "AI capex flatlines 2027" risk lower post-MU print: Q4 guide $50B, HBM4 2x ramp, hyperscaler Q1 capex +40–60% YoY. Option 2 (rebalance toward Group 3) rejected — T1 weighting already implements it implicitly. Option 3 (SMH puts) rejected — roll/management complexity unsuitable for paper research book. **Guardrail added:** no new Group 1 name enters at T2 or above without first clearing ≥1.5x asymmetry threshold. Cash buffer: 15.8% post-ENTG exit. | Logged |
| 2026-06-18 | AMAT | PT $520→$680, maintain Buy | $616.32 | Revised estimates | Q2 FY2026: record revenue $7.91B (+11% YoY), non-GAAP EPS $2.86 (+20%), gross margin 50.0% (record). AMAT raised WFE calendar 2026 growth outlook to >30%. Original $520 PT anchored on stale estimates. FY2027E EPS ~$13.50–14.50; at 48x = $680. Cantor $650 / Citi $710 — we sit between them. ~10% upside to new PT. Bear $300 unchanged. | Open |
| 2026-06-18 | LRCX | PT $380→$450, maintain Buy | $393.81 | Revised estimates | Q3 FY2026: revenue $5.84B (+24% YoY), EPS $1.47 (beat). Q4 FY2026 guidance: $6.6B ±$400M revenue, EPS ~$1.65, GM 50.5%. Annualized Q4 run rate = $26.4B (vs $18.4B FY2025). FY2027E EPS tracking ~$7.25; at ~60x = $435, bull case ~65x = $472; PT $450 reflects WFE supercycle thesis printing ahead of consensus. Consensus high $425 — we remain above. Q4 earnings July 29 added to Catalyst Playbooks. Bear $200 unchanged. | Open |
| 2026-06-18 | AVGO | Confirmed Buy/$560 — no change after Q2 FY2026 scoring | $408.24 | Thesis-driven (invalidation trigger check) | Q2: AI semi $10.8B (+143% YoY), Q3 guide $16.0B AI semi (+200% YoY). All 3 invalidation triggers clean. VMware miss ($7.18B vs $7.32B est.) was noise; post-print -12.59% was sell-the-news. Aschenbrenner's Situational Awareness LP took new long in Q1 2026 — short thesis empirically inverted. Rating/PT unchanged. | Open |
| 2026-06-25 | MU | Upgrade Hold→Buy, PT $1,100→$1,500 | $1,165.94 | $1,500 | Catalyst Playbook | Q3 FY2026: rev $41.46B (beat $35.59B by 16.5%), non-GAAP EPS $25.11 (beat $20.60 by 22%), GM 84.9%. Q4 guide $50.0B ±$1.0B vs $42B upgrade threshold — beat by $8B. GM guide ~86% (expanding). HBM4 ramp 2x faster than HBM3E; >$1B shipped; booked through CY2027. All three Catalyst Playbook upgrade conditions cleared. 16 SCAs (~$22B) signed. At $1,166 = ~9.7x NTM EPS (~$120); cheapest AI-infra name in book on earnings yield. Added T2 (4%) in Model Portfolio at $1,166. Bear $900 (two sequential GM declines + HBM4 slip + China restriction). Read-through: positive LRCX (HBM4 TSV), positive AMAT (capex step-up), positive ASML (EUV deal confirmed); SNDK NAND positive, upgrade deferred. | Open |
| 2026-06-29 | ON | Downgrade Buy→Hold, PT $160→$100 | $88.57 | $100 | Thesis-driven (M&A event) | Synaptics $7B all-stock (1.35x exchange ratio, close mid-2027): ~12% share dilution; EPS accretive only ~late 2028 per mgmt; pivots ON from pure-SiC/EV to "physical AI platform." Original 3 bear triggers (EV volume, inventory correction, SiC displacement) NOT fired — downgrade is strategic, not fundamental. Bear revised $80→$65 (integration failure + EV SiC weakness = trough P/E ~$65). TD Cowen downgraded to Hold day-1; Street consensus PT $102.73. Re-entry: post-close synergy proof + PT >$120 with ≥1.5x asymmetry, or pullback to $70–75 with SiC intact. | Open |
| 2026-06-18 | FCEL | Under Review → Hold/$18 | $16.60 | Thesis-driven (binary event check) | Q2 binary event (hyperscaler contract ≥100 MW) NOT triggered. Revenue $35.6M (-5% YoY). Pipeline +267% to 4 GW (90% DC, avg proposal 130 MW). Not a Buy without a signed contract; not a Pass given extraordinary pipeline growth. T4 (1%) maintained. Upgrade if: contract signed. Exit if: no contract in 2 qtrs or cash runway <4 qtrs. | **Closed 6/23 — ~** (PT $18 breached +21%; stock $21.82, +31% from entry in 5 sessions; neutral PT undershot — see Lessons #3) |
| 2026-06-18 | INTC | Initiate Hold/$120 | $121 | Thesis-driven (turnaround + foundry optionality) | Initiating on day of Trump-announced Apple 18A deal. 6 straight beats under Lip-Bu Tan. DCAI +22% YoY. Coalition: $8.9B CHIPS Act + $5B NVIDIA + Apple foundry. FCF −$3.1B TTM, $45B debt. 18A yields 65–75%; industry standard 2027. At $121 (>100x FY2026E Non-GAAP EPS) turnaround is real but priced in. P-W EV ~$106 (−12%). Upgrade: pullback to $95–105 or hyperscaler 14A commit. | **Closed 6/23 — ✗** (PT $120 breached +10%; stock $132.28 vs PW fair value $106; bearish-leaning Hold, stock +9% in 5 sessions — see Lessons #3) |

---

## Closed Decisions Scorecard

| Period | Decisions closed | ✓ | ~ | ✗ | Hit rate (✓-only) | Best methodology | Worst |
|---|---|---|---|---|---|---|---|
| Q2 2026 | 3 (GEV Hold/$440, FCEL Hold/$18, INTC Hold/$120) | 0 | 1 | 2 | 0% (~17% w/ ~ half-credit) | — (none validated) | Fair-value-anchored Holds |

*Scorable closes only. Excluded as non-scorable: CEG "Initiate Under Review" (placeholder, no PT/rating to judge) and the TOELY exclusion→reinstatement (data-integrity correction, no directional thesis).*

### Hit rate by methodology (cumulative)

| Methodology | Closed | ✓ | ~ | ✗ | Hit rate (✓-only) |
|---|---|---|---|---|---|
| DCF / DCF + comps | 1 | 0 | 0 | 1 | 0% |
| Thesis-driven | 2 | 0 | 1 | 1 | 0% (25% w/ ~ half) |
| Variant perception | 0 | — | — | — | n/a (none closed) |
| Comps (standalone) | 0 | — | — | — | n/a (none closed) |
| Screener | 0 | — | — | — | n/a (none closed) |
| **Total** | **3** | **0** | **1** | **2** | **0% (~17%)** |

### Hit rate by sector (cumulative)

| Sector | Closed | ✓ | ~ | ✗ | Hit rate (✓-only) |
|---|---|---|---|---|---|
| Power / Utilities / Electrical | 2 (GEV ✗, FCEL ~) | 0 | 1 | 1 | 0% |
| Semiconductors | 1 (INTC ✗) | 0 | 0 | 1 | 0% |
| **Total** | **3** | **0** | **1** | **2** | **0%** |

> **The unmistakable pattern:** 100% of closed decisions are Holds the market overran to the upside. Zero closed *Buy* decisions yet (the GEV upgrade, CEG, VST, NBIS, AMAT, LRCX, AVGO and others all remain open). The track record so far measures only the cost of being too conservative — not the methodologies' ability to pick winners. That test arrives when the open Buys close.

---

## Lessons

**#1 — GEV (May→June 2026): DCF anchoring in a supply-constrained repricing.**
The Hold/$440 was driven by a Gordon-growth DCF ($218) that mechanically could not price sold-out-through-2029 backlog with structurally rising prices — the model treated a *contracted* margin expansion as speculative terminal-value optionality. The market was right; the framework was wrong by ~2.7x. Rule going forward: when backlog/orders give multi-year revenue visibility with disclosed price escalation, weight comps/NTM-earnings frameworks over DCF, and treat the DCF as the "cycle breaks" bear case only. (Same logic now applies to: CAT, GNRC, HUBB, BW.)

**#2 — June 3 batch initiation risk (open question).**
~40 names were rated in one session. Expect mean reversion in quality: the quarterly review should specifically test whether June 3 batch decisions underperform decisions made with individual deliberation (GEV upgrade, VST initiation). *Q2 2026 update: no June 3 batch decision has closed yet, so the test is still pending. Early counter-signal — the two individually-deliberated 6/18 Holds (FCEL, INTC) both closed as misses, suggesting deliberation alone does not fix a framework-level conservatism bias; see Lesson #3.*

**#3 — Conservative Holds blow through their PTs to the upside in a momentum AI-infrastructure tape (May–June 2026).**
Every decision closed to date is a neutral or fair-value-anchored call the market overran: GEV Hold/$440 (✗, DCF-anchored, closed at ~2.7x), FCEL Hold/$18 (~, neutral PT undershot a +31% move in 5 sessions), INTC Hold/$120 (✗, probability-weighted fair value $106 vs $132 actual, +9% in 5 sessions). The common failure is treating a *static fair-value PT as a safe default* on names with visible positive catalysts (backlog, contract pipeline, foundry optionality). Meanwhile the one decision that broke the pattern — the GEV upgrade to Buy/$1,200 — is the only open winner. Rule going forward: on an AI-infrastructure name with a known catalyst pipeline, a Hold is an *active lean against momentum* that must be justified, not a default; set the Hold PT no lower than a defensible base case, widen the required upside band before defaulting to neutral, and treat any fair-value anchor (DCF or static multiple) as the "cycle breaks" floor per Lesson #1. (Watch: TSEM Hold/$285 sits just 0.8% below PT at $282.65 — the next Hold to test this.)

---

## Change Log

- `2026-06-29` — **ON downgraded Buy→Hold.** PT $160→$100, bear $80→$65. Synaptics $7B all-stock acquisition announced June 26; stock −24% to $88.57 by decision date (June 29). Original SiC/EV thesis intact — downgrade is strategic (M&A dilution + pivot to "physical AI platform"), not fundamental. Re-entry gated on post-close synergy proof or pullback to $70–75.
- `2026-06-25` — **MU upgraded Hold→Buy.** PT $1,100→$1,500 after Q3 FY2026 print ($41.46B rev, $25.11 EPS). Q4 guide $50B midpoint cleared the Catalyst Playbook $42B upgrade threshold by $8B; HBM4 ramping 2x faster; GM expanding 84.9%→86%. Added T2 (4%, ~$4,000) in Model Portfolio at $1,165.94. Read-throughs: LRCX/AMAT/ASML all positive; SNDK upgrade deferred pending valuation check.
- `2026-06-23` — **Q2 2026 quarterly scoring run.** Closed and scored FCEL Hold/$18 (~, PT breached +21%) and INTC Hold/$120 (✗, PT breached +10%) — both Holds the market overran to the upside. Scorecard rebuilt with by-methodology and by-sector tables (cumulative n=3: 0 ✓ / 1 ~ / 2 ✗). Added Lesson #3 (conservative-Hold anchoring) and a Hold-scoring convention (Rule 6). Reconciliation check: AMAT/LRCX PT raises and ENTG downgrade have NOT propagated into Model Portfolio.md (still $520 / $380 / Buy $155); all four flagged corrections did propagate into the 03_Companies notes. Prices: GEV $1,034.98, CEG $270.26, VST $162.39, NBIS $275.25, TSEM $282.65, HUT $120.51, XYL $110.40, BW $15.90, TOELY $227.80, ENTG $168.22, AMAT $585.88, LRCX $371.33, AVGO $380.15, FCEL $21.82, INTC $132.28 (official closes 6/23).
- `2026-06-20` — TOELY PT restatement resolved. ADR error ($403 → $270) logged; prior exclusion closed.
- `2026-06-18` — AVGO and FCEL post-earnings scoring logged. Decisions Log updated to reflect last_updated.
- `2026-06-09` — Log created; seeded from company-note change logs. First scorecard entry: GEV initial Hold scored ✗.
