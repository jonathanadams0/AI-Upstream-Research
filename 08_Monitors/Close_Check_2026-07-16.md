---
date: 2026-07-16
time_ct: "post-close"
type: close_check
conditions_fired: [MU_900_close]
flag_for_review: true
prior_alert: Intraday_Alert_2026-07-15_close.md
---

# MU / CCJ Close Check — 2026-07-16 (Scheduled)

> Post-close verification of two armed close-based triggers: MU $900 re-underwrite (armed 7/7) and CCJ $85 re-underwrite (armed 7/13). FMP settled quotes, 16:00:01 ET, NASDAQ/NYSE confirmed closed.

## MU $900 Close Trigger: **FIRED**

**MU official close: $853.20** (−5.65%, prev close $904.28). Margin below the $900 floor: **−$46.80 / −5.2%**. First close below the floor after three consecutive sessions of intraday-only proximity (7/13, 7/15, 7/16 intraday).

- Driver (one line): day 3 of the semi/memory selloff — TSMC Q2 sell-the-news carryover plus CXMT $8.6B IPO stoking Chinese DRAM competition fears; memory complex weakest (MRVL −8.7%).
- Intraday: dayLow print $840.51 (vendor print, unconfirmed per 7/15 precedent) — moot; the close itself is below the floor.
- **Action: re-underwrite protocol FIRED.** Execute the staged checklist [[MU_ReUnderwrite_Prep_2026-07-16]] next working session, anchored to the SK Hynix July 24 print as the designated hard datapoint. **No rating, PT ($1,200), or bear ($800) change made — flagged for Jonathan's review only. No trades.**

## CCJ $85 Close Trigger: NOT FIRED

**CCJ official close: $87.37** (−3.97%, prev close $90.98). Margin above the $85 floor: **+$2.37 / +2.8%**. Second consecutive session inside ~7% of the trigger; intraday low $86.44 (+1.7% from floor). Protocol stays armed.

## Bear-Proximity Cluster

| Ticker | Close | Chg % | Bear floor | Distance to floor |
|---|---|---|---|---|
| MU | $853.20 | −5.65% | $900 (trigger) | **BREACHED −5.2%** |
| CCJ | $87.37 | −3.97% | $85 | +2.8% |
| MRVL | $188.30 | −8.71% | $180 | +4.6% |
| FN | $460.22 | −5.43% | $450 | +2.3% |
| VST | $152.54 | −4.80% | $145 | +5.2% |
| AVGO | $374.45 | −5.03% | $350 | +7.0% |
| SMH (context) | $568.92 | −3.70% | — | — |

Whole cluster compressed toward bear floors today; FN and CCJ are the next-closest triggers (<3%).

## Next Steps

1. Jonathan to review MU fire and run the re-underwrite checklist (anchor: SK Hynix Jul 24).
2. CCJ $85 protocol remains armed; FN has no armed trigger but sits +2.3% from bear — consider arming if weakness persists.
