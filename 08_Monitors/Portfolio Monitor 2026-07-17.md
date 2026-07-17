# Upstream Portfolio Monitor — July 17, 2026 (Weekly Vault Price Refresh)

*Automated weekly refresh | Prices as of July 17, 2026 (last-trade-at-3:59:59 PM ET; Robinhood official-close API still lagged one session — showing 7/16 — at run time, same convention as prior weekly marks).*

*60 of 61 company notes refreshed (`current_price` + `last_updated: 2026-07-17`). SMNEY skipped — not resolvable via Robinhood (404, consistent with all prior runs). Manual price update needed.*

*Context: day 4+ of a broad semiconductor/memory selloff (TSMC Q2 sell-the-news carryover, CXMT $8.6B IPO stoking Chinese DRAM competition fears, tape-wide "tech shakeout" momentum unwind per 7/17 intraday coverage). Comparison baselines below use each ticker's last recorded frontmatter price — for several names that's still 7/3 (not refreshed in the interim), so treat magnitude as directional, not a clean 7-day return.*

---

## Model Portfolio — NAV Update

| Metric | Value |
|--------|-------|
| **NAV (7/17 close)** | **$94,350.32** |
| vs. Inception (June 9) | **−5.65%** |
| Week change (vs. $101,532.69 on 7/10) | **−$7,182.37 (−7.07%)** |
| SPY $100k (same day) | $100,831.69 (+0.83%) |
| SMH $100k (same day) | $94,096.56 (−5.90%) |
| **Alpha vs. SPY** | **−6.48pp** |
| **Alpha vs. SMH** | **+0.25pp** |

*Portfolio −5.65% since inception — first mark below the SPY-inception line all-time. Alpha vs. SPY −6.48pp (market outperformance gone). Alpha vs. SMH +0.25pp is relative outperformance only — both lines are down; the book simply fell marginally less than the semis benchmark. No position changes this week; cash unchanged at $11,812 (11.8%).*

### Top 3 Contributors This Week

| Ticker | Weekly Δ ($) | Price Change | Note |
|--------|-------------|--------------|------|
| **CEG** | **+$535.37** | +6.7% ($236.50 → $252.42) | T1 8.5%; PJM BRA clearing follow-through continuing post 7/14 |
| **AVGO** | **+$78.85** | +2.1% ($363.11 → $370.84) | T2 4%; still only 6.0% above bear $350 |
| **VST** | **+$62.23** | +1.5% ($153.16 → $155.44) | T2 4%; frontmatter bear ($145) is stale — see flag below |

### Bottom 3 Contributors This Week

| Ticker | Weekly Δ ($) | Price Change | Note |
|--------|-------------|--------------|------|
| **MRVL** | **−$1,250.00** | −30.7% ($272.05 → $188.65) | T2 4%; now only 4.8% above bear $180 — memory/networking hit hardest |
| **BE** | **−$1,152.80** | −25.8% ($289.50 → $214.68) | T2 4%; no fundamental trigger identified — sector-wide, not Jupiter-specific |
| **LRCX** | **−$955.25** | −20.0% ($391.26 → $313.13) | T2 4%; WFE demand-scare narrative is the risk to watch into Jul 29 print |

---

## Week's Biggest Movers (>±5% vs. last recorded frontmatter price)

| Ticker | Old → New | Change | In Portfolio? |
|--------|-----------|--------|---------------|
| SNDK | $2,032.22 → $1,356.34 | **−33.3%** | No (Hold) |
| MRVL | $272.05 → $188.65 | **−30.7%** | Yes (T2 4%) — near bear |
| GLW | $220.63 → $154.62 | **−29.9%** | No (Hold) |
| FCEL | $25.96 → $18.48 | **−28.8%** | No (Hold) |
| APLD | $35.52 → $25.80 | **−27.4%** | Yes (T4 1%) |
| BE | $289.50 → $214.68 | **−25.8%** | Yes (T2 4%) |
| INTC | $127.02 → $95.03 | **−25.2%** | No (Hold) |
| COHR | $368.65 → $277.55 | **−24.7%** | No (Hold) |
| BW | $12.74 → $9.88 | **−22.4%** | No (Hold) |
| IREN | $43.32 → $33.62 | **−22.4%** | No (Hold) |
| NBIS | $229.18 → $178.17 | **−22.3%** | Yes (T2 4%) |
| CRDO | $259.09 → $202.69 | **−21.8%** | No (Hold) |
| GNRC | $270.22 → $214.85 | **−20.5%** | Yes (T4 1%) |
| WDC | $598.37 → $476.96 | **−20.3%** | No (Hold) |
| KLAC | $266.19 → $212.78 | **−20.1%** | No (Hold) |
| LRCX | $391.26 → $313.13 | **−20.0%** | Yes (T2 4%) |
| AMAT | $650.91 → $529.41 | **−18.7%** | Yes (T3 2%) |
| CLS | $361.62 → $301.04 | **−16.8%** | Yes (T3 2%) |
| MP | $54.28 → $45.23 | **−16.7%** | Yes (T3 2%) |
| ENTG | $165.19 → $138.67 | **−16.1%** | No (exited 6/25; Hold) |
| STX | $915.19 → $786.93 | **−14.0%** | No (Hold) |
| OKLO | $47.61 → $41.10 | **−13.7%** | No (Hold) |
| WOLF | $34.59 → $29.87 | **−13.6%** | No (dropped) |
| HUT | $105.79 → $91.45 | **−13.6%** | No (Hold) |
| FN | $547.18 → $478.36 | **−12.6%** | Yes (T3 2%) — near bear |
| CORZ | $23.71 → $20.95 | **−11.7%** | No (M&A tracking) |
| CAT | $991.41 → $880.28 | **−11.2%** | Yes (T3 2%) |
| UUUU | $12.86 → $11.48 | **−10.7%** | Yes (T4 1%) — PT suspended |
| MU | $938.38 → $848.95 | **−9.5%** | Yes (T2 4%; Hold) — $900 close-trigger already fired 7/16 |
| PWR | $691.40 → $628.42 | **−9.1%** | No (Hold) |
| LITE | $801.16 → $732.75 | **−8.5%** | Yes (T3 2%) |
| SPXC | $231.72 → $211.96 | **−8.5%** | Yes (T4 1%) |
| NRG | $140.80 → $129.12 | **−8.3%** | Yes (T1 8.5%) |
| ON | $94.63 → $87.41 | **−7.6%** | Yes (T4 1%; Hold) |
| VRT | $311.42 → $289.41 | **−7.1%** | Yes (T2 4%) |
| GEV | $1,134.35 → $1,057.24 | **−6.8%** | Yes (T1 6.5%) |
| MOD | $244.49 → $229.20 | **−6.3%** | Yes (T3 2%) |
| CCJ | $90.20 → $85.62 | **−5.1%** | Yes (T2 4%) — closest to bear, close-based trigger armed |
| CEG | $236.50 → $252.42 | **+6.7%** | Yes (T1 8.5%) — sole notable gainer |

*Broad-based decline across the entire book; only CEG posted a gain. Memory/networking (SNDK, MRVL, GLW, NBIS) and speculative/small-cap names (FCEL, BW, IREN, INTC) hit hardest — consistent with the CXMT-IPO/DRAM-competition-fear narrative plus a tape-wide semiconductor rotation (AMD, Intel, Nvidia all down intraday per 7/17 coverage). No single-name catalyst identified for the bulk of the moves.*

---

## PT / Bear-Case Proximity (Sizing Framework Triggers)

### Harvest-Trigger Candidates (within 5% of price target)

None. Closest Buy-rated name to its PT is GEV at 11.9% below $1,200 (down from 5.5% away two weeks ago, following this week's decline).

### Upsize-Trigger Candidates (within 10% of bear case)

| Ticker | Current | Bear | % Above Bear | Note |
|--------|---------|------|---------------|------|
| **CCJ** | $85.62 | $85.00 | +0.7% | T2 4%; close-based re-underwrite protocol armed since 7/13 — only a settled close below $85 fires it |
| **MRVL** | $188.65 | $180.00 | +4.8% | T2 4%; hit hardest this week (−30.7%) — memory/networking demand-fear narrative is the watch item |
| **AVGO** | $370.84 | $350.00 | +6.0% | T2 4%; no AVGO-specific negative catalyst found |
| **FN** | $478.36 | $450.00 | +6.3% | T3 2%; no FN-specific news — moving with the networking/optics complex |

> **Flag — no re-rate.** Four Buy-rated positions are simultaneously within 10% of bear case, the most crowded this cluster has been. CCJ remains closest by a wide margin and has an armed close-based trigger (per 7/13 precedent) — only a settled close below $85 fires it. **Data-quality note carried forward from today's intraday alerts: VST's frontmatter `bear_price` ($145) is stale** — the company note's own re-underwritten bear case is $105 (2026-06-23), which puts VST at +48% above the corrected bear, not close at all. VST is excluded from this table on that basis; frontmatter left uncorrected per this task's scope (prose/bear-case edits are out of bounds for the price-refresh run) but flagged again for manual correction.

---

## Thesis Invalidation Tracker — Price-Action Flags

| Ticker | This Week | Price vs. Trigger | Note | Action |
|--------|-----------|--------------------|------|--------|
| **MU** | −9.5% | $848.95 / bear $800 (+6.1%) | Hold-rated; $900 close-based re-underwrite protocol already **FIRED 7/16** ([[MU_ReUnderwrite_Prep_2026-07-16]]); no new fundamental trigger this week, sector rotation continues | Standing fire — checklist pending, anchored to SK Hynix Jul 24 print |
| **CCJ** | −5.1% | $85.62 / bear $85 (+0.7%) | No negative CCJ-specific catalyst; Cigar Lake mine restart (7/14–7/15) is mildly positive | FLAG — close-based protocol armed since 7/13; monitor for settled close below $85 |
| **MRVL** | −30.7% | $188.65 / bear $180 (+4.8%) | Amazon Trainium / Microsoft Maia sell trigger not confirmed — no guidance cut or program delay found; move tracks sector-wide memory/networking fear | FLAG — largest single-week move in the book; watch for hyperscaler commentary |
| **AVGO** | +2.1% | $370.84 / bear $350 (+6.0%) | No Google/Meta ASIC-dependency announcement found | No new flag — trigger not touched, proximity only |
| **LRCX** | −20.0% | $313.13 / bear $200 (far above) | WFE spending-cut trigger not confirmed; Jul 29 LRCX earnings is the validation gate | Watch — largest T2 dollar detractor this week |
| **NBIS** | −22.3% | $178.17 / bear $80 (far above) | Revenue-deceleration trigger not confirmed; no Q2 print yet (~Aug 14) | No action — far from trigger despite large move |

*No fundamental thesis-break signals confirmed this week — every trigger in the tracker above is earnings/filing/regulatory-gated, and this week's moves read as sector-wide sentiment (semiconductor/memory rotation) rather than name-specific news. The one exception worth flagging for Jonathan's review is the MU $900 standing trigger, which fired 7/16 and has a pending re-underwrite checklist.*

---

## Skipped / Manual Update Needed

- **SMNEY** — not resolvable via Robinhood (404 error; OTC/ADR listing, consistent with all prior runs). Frontmatter unchanged (last price $35.37 as of 2026-07-07). Manual update needed.

---

## Status

**60 of 61 notes refreshed. One new NAV row appended to Model Portfolio. No rating, PT, tier, or bear-case changes made.**

Key items for review this week:
1. **Broad semiconductor/memory selloff** — day 4+, driven by TSMC Q2 sell-the-news carryover and CXMT $8.6B IPO stoking Chinese DRAM competition fears. Hit MRVL, GLW, NBIS, SNDK hardest. No portfolio-specific fundamental trigger confirmed.
2. **MU $900 close-trigger fired 7/16** — re-underwrite checklist ([[MU_ReUnderwrite_Prep_2026-07-16]]) pending, anchored to SK Hynix Jul 24 print.
3. **CCJ within 0.7% of bear case** — closest proximity of the entire book; close-based protocol armed since 7/13.
4. **Four Buy names simultaneously within 10% of bear** (CCJ, MRVL, AVGO, FN) — the most crowded this cluster has been since inception.
5. **VST frontmatter `bear_price` stale** ($145 vs. corrected $105) — carried forward from today's intraday alerts; recommend correcting per the CCJ 7/13 precedent.
6. **NAV alpha vs. SPY has flipped negative** (−6.48pp) for the first time since inception; alpha vs. SMH is positive only because SMH fell further, not because the book is up.
