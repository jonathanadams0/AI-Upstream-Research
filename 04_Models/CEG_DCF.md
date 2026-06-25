---
tags: [model]
ticker: CEG
last_updated: 2026-04-15
---

# CEG DCF Model — v1.0 Skeleton

**File:** [[CEG_DCF_v1.xlsx]]
**Company:** [[CEG]]

## Model Structure

| Tab | Description |
|---|---|
| Cover | Summary, sources, color conventions, health warnings |
| Assumptions | All forecast inputs (revenue growth, margins, WACC). BLUE cells are editable. |
| Revenue | Segment revenue build: Nuclear, Gas (Calpine), Geothermal, Retail/Other |
| P&L | Income statement forecast, bridges to Adj EBITDA |
| FCF | Unlevered free cash flow build (EBITDA → NOPAT → UFCF) |
| DCF | Discounting, terminal value (Gordon + exit multiple), equity bridge |
| Historicals | Clean historical pull from 10-K (CEG standalone, pre-Calpine) |
| Sensitivity | WACC vs terminal growth; WACC vs exit multiple grids |
| Scenarios | Bear / Base / Bull with full assumption tables |
| Comps | IPP and utility peer multiples; implied valuation |

## Key Outputs (Base Case)

| Method | Implied Price | vs. $295 |
|---|---|---|
| Gordon Growth (WACC 8.0%, g 2.5%) | **~$190** | -36% |
| Exit Multiple (14x 2030E EBITDA) | **~$264** | -11% |
| Bear Scenario | ~$88 | -70% |
| Bull Scenario | ~$400 | +36% |

## Key Assumptions

- **WACC:** 8.0% (lower than GEV's 11.3% due to utility-like characteristics + investment grade credit)
- **Terminal growth:** 2.5%
- **Segments:** Nuclear (~53% of 2030E rev), Gas/Calpine (~28%), Retail/Other (~19%)
- **Nuclear EBITDA margin:** 22.5% (2025) → 29% (2030E) — PPA repricing + PTC support
- **TMI/Crane restart:** $1.6B capex phased 2025-2028, 835 MW online 2027
- **Pro forma debt:** ~$20B post-Calpine; 30% debt weight in WACC
- **Tax rate:** 22% normalized

## Health Warnings

1. Calpine closed Jan 2026 — first consolidated quarter is Q1'26. Pro forma historicals are estimates.
2. Nuclear PTC ($15/MWh) assumed through 2032. Extension risk beyond that.
3. TMI/Crane FERC interconnection risk flagged in April 2026 filing.
4. Model does not include potential additional hyperscaler PPAs beyond Microsoft and Meta.

## To-Do

- [ ] Populate with Q1'26 actuals (first Calpine-consolidated quarter) after May 7 earnings
- [ ] Refine Calpine segment estimates with actual pro forma disclosure
- [ ] Build sum-of-parts: Nuclear fleet at $/kW replacement value + Gas at market + PPA NPV
- [ ] Stress-test: what if TMI restart delayed to 2029?
- [ ] Add nuclear PTC sensitivity (with/without extension post-2032)
