---
tags: [dashboard]
---

# AI Upstream Research — Dashboard

> Central hub. All tables auto-update from YAML frontmatter in company/sector/thesis notes.
> 
> **→ [[Portfolio Summary]]** — top 15 buys, sector breakdown, Aschenbrenner overlap, earnings calendar, maintenance schedule
> **→ [[Decisions Log]]** — every rating/PT change with reasoning; quarterly hit-rate scorecard
> **→ [[AI Capex Stress Test]]** — portfolio-level bear-case aggregation; asymmetry ranking (June 2026: only 4 of 27 Buys clear the 1.5x sizing bar)
> **→ [[Catalyst Playbooks]]** — pre-committed decision trees: SK Hynix ~7/24, Samsung ~7/30 (macro inputs), ASML 7/16, GEV ~7/22, LRCX 7/29, PJM ~Jul, VST ~8/7, BE/Jupiter
> **→ [[Global Macro Overlay]]** — geopolitical risk layer: Korea (Samsung/SK Hynix capex), Taiwan (TSMC), US-China export controls; breach thresholds → re-underwrite triggers; monthly auto-monitor
> **→ [[Verification Worklist]]** — 295 "(confirm from latest filings)" flags, prioritized
> **→ [[Hold PT Watch]]** — Holds trading at/above PT; next candidates for the Lesson #3 "conservative Hold overrun" error
> **→ [[Model Portfolio]]** — $100k paper book at tier weights (inception 6/9/26), NAV tracked weekly vs SPY/SMH

---

## Coverage by Rating

```dataview
TABLE WITHOUT ID
  file.link AS "Company",
  ticker AS "Ticker",
  sector AS "Sector",
  rating AS "Rating",
  price_target AS "PT",
  conviction AS "Conv."
FROM "03_Companies"
WHERE rating
SORT rating ASC, conviction DESC
```

---

## Buy-Rated Names (High Conviction)

```dataview
TABLE WITHOUT ID
  file.link AS "Company",
  ticker AS "Ticker",
  sector AS "Sector",
  price_target AS "PT",
  ai_exposure AS "AI Exposure"
FROM "03_Companies"
WHERE rating = "Buy" AND (conviction = "High" OR conviction = "Medium-High")
SORT conviction DESC
```

---

## Upcoming Earnings (Next 60 Days)

```dataview
TABLE WITHOUT ID
  file.link AS "Company",
  ticker AS "Ticker",
  next_earnings AS "Earnings Date",
  rating AS "Rating"
FROM "03_Companies"
WHERE next_earnings AND date(next_earnings) >= date(today) AND date(next_earnings) <= date(today) + dur(60 days)
SORT next_earnings ASC
```

---

## Coverage by Sector

```dataview
TABLE WITHOUT ID
  sector AS "Sector",
  length(rows) AS "# Companies",
  length(filter(rows, (r) => r.rating = "Buy")) AS "Buys",
  length(filter(rows, (r) => r.rating = "Hold")) AS "Holds",
  length(filter(rows, (r) => r.rating = "Sell")) AS "Sells"
FROM "03_Companies"
WHERE sector
GROUP BY sector
```

---

## Active Theses

```dataview
TABLE WITHOUT ID
  file.link AS "Thesis",
  status AS "Status",
  conviction AS "Conv."
FROM "01_Theses"
WHERE status
SORT file.name ASC
```

---

## Stale Notes (Not Updated in 30+ Days)

```dataview
TABLE WITHOUT ID
  file.link AS "Company",
  last_updated AS "Last Updated"
FROM "03_Companies"
WHERE last_updated AND date(last_updated) < date(today) - dur(30 days)
SORT last_updated ASC
LIMIT 10
```

---

## To-Do

- [x] Complete first full reports — [[GEV]] (May 5, upgraded to Buy June 3) + [[VST]] (initiated June 3)
- [x] Build DCF models — GEV v7, CEG v1, VST v1, NRG v1
- [x] Populate sector primers — all 4 done (Power-Gen-Grid, Cooling-Thermal, Semi-Materials-Equip, Critical-Minerals)
- [x] Rate all coverage names — 25 companies, all rated as of June 3, 2026
- [ ] Read latest 10-Q for each Buy-rated name
- [ ] Set price alerts for key names (ASML Q2 July 16, GEV Q2 ~July 22, VST ~Aug 7)
- [x] CCJ and HUBB company briefs — Done (CCJ_brief.md, HUBB_brief.md)
- [x] Research Nebius Group (NBIS) — Done (NBIS.md; Buy/$310; +599% YoY; his 2nd largest position)
- [x] Research Tower Semiconductor (TSEM) and Hut 8 (HUT) — Done (TSEM.md Hold/$285; HUT.md Hold/$145)
- [x] Run AI Bottleneck Screener quarterly — Q3 run done 2026-06-23; top find EME (4/5 HIGH, initiation queued); next run Sep 2026
- [x] Initiate BW (Babcock & Wilcox) — screener 5/5 HIGH — Done 2026-06-09 (BW.md, Under Review pending price/10-Q)
- [x] BW: pull price + entry multiple, read Q1'26 10-Q, assign rating — **Hold/$18, bear $4** (2026-06-29)
- [x] **Decide the hedge question** — Decided 2026-06-25: Option 1, accept current asymmetry (1.12x tier-weighted); Group-1 guardrail added (no new Group 1 name at T2+ without ≥1.5x asymmetry). Logged in [[Decisions Log]] 6/25. *(Checkbox cleared 7/2 — was stale.)*
- [x] Ratify DRAFT thresholds in [[Catalyst Playbooks]] before July 16 — Done 2026-06-23; six events ratified (MU ✅ resolved 2026-06-25); MU FQ4 playbook added
- [x] Fix ENTG bear price placeholder — bear $85 confirmed in §8, sourced from verified adj. EBITDA multiples (2026-06-22)
- [x] **VST: re-underwrite bear price** — Done 2026-06-23. Bear restated $145 → **~$105** with real downside math (EBITDA $6.5B × 9x; range $90–112); asymmetry corrected 13.1x → **~1.1x**; PJM "add" rerouted to CEG/NRG in [[Catalyst Playbooks]]. Upsize-to-T1 trigger now ~$115 (within 10% of bear). Still watch CCJ — ~$95, ~12% above its $85 bear, near the 10% trigger zone
- [x] **TOELY: restate PT in ADR terms** — Done 2026-06-20. PT $403 (Tokyo) → **$270 ADR** (1 ADR = 0.5 shares; FY2027 bull EPS ~$6.00 at 45x). T4 slot still in cash pending add decision.
- [x] **MU post-earnings: upgrade Hold→Buy** — Done 2026-06-25. Q3 revenue $41.46B, Q4 guide $50.0B (>> $42B upgrade threshold). PT $1,100→**$1,500**; added T2 (4%) in Model Portfolio at $1,165.94. FQ4 playbook added (~Sep 25, 2026).
- [x] Earnings prep automated — Monday 8 AM scheduled task (set up 2026-06-09): scans next_earnings, drafts prep notes 14 days out
- [ ] Evaluate WMB (screener 4/5) for initiation — Q2 2026
- [ ] Initiate EME (EMCOR) — screener Q3 4/5 HIGH; DC-build laggard, RPO $15.6B (+33%), ~24x fwd (under 25x bar)
- [x] All theses written — 16 total (Uranium Supply-Demand Inflection + Vertiv as AI Cooling Pure-Play added)
- [x] Periodic refresh: automated weekly (Fri 4:30 PM scheduled task, set up 2026-06-09) — writes monitor note to 08_Monitors/

---

## Coverage Statistics (as of June 9, 2026)

> ⚠️ Static snapshot — recomputed from frontmatter 2026-06-09. The Dataview "Coverage by Sector" table above is the source of truth; prefer it over this table.

| Sector | Companies | Buys | Holds | Under Review |
|---|---|---|---|---|
| Power-Gen-Grid | 14 (incl. BW, OKLO) | 8 | 3 | 3 |
| Cooling-Thermal | 5 | 3 | 2 | 0 |
| Semi-Materials-Equip | 8 | 4 | 4 | 0 |
| Critical-Minerals | 5 | 3 | 2 | 0 |
| Memory-Storage | 4 | 0 | 3 | 1 |
| AI-Networking | 9 (incl. LITE, FN, CLS) | 6 | 3 | 0 |
| Power-Electronics | 3 | 1 | 1 | 1 |
| Data-Center-Infra | 10 (incl. NBIS, HUT, CORZ, APLD, IREN) | 5 | 3 | 2 |
| **Total** | **58** | **30** | **21** | **7** |
