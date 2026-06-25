---
tags: [dashboard]
last_updated: 2026-06-09
tickers_analyzed: 27
---

# AI Capex Stress Test — June 2026

> **The question this answers:** the 30 Buys are substantially one bet — hyperscaler AI capex keeps growing. What happens to the whole book if it flatlines in 2027? Bear prices below are each note's own bear case (scenario frameworks added June 4), so this is the vault's stated downside, aggregated for the first time.

**Headline (equal-weight, 27 names with complete data):**

| Metric | Value |
|---|---|
| Average upside to PT | **+21.9%** |
| Average downside to bear price | **−34.8%** |
| Asymmetry (avg upside ÷ avg downside) | **0.63x — i.e., unfavorable** |
| Names with asymmetry ≥1.5x (Tier-1 sizing criterion) | **4 of 27** |

**The uncomfortable finding:** the Position Sizing Framework requires asymmetry ≥1.5x for Tier-1 weights, and prefers ≥2x generally. At June 9 prices, only **VST (13.1x), CEG (2.9x), NRG (2.4x), AVGO (2.3x)** clear 1.5x. The other 23 Buys have more bear-case downside than PT upside. The book as a whole is short asymmetry — it wins only if the bear cases stay improbable.

---

## Asymmetry Ranking (PT upside ÷ bear downside, June 9 prices)

| Ticker | Bear | Upside | Ratio | | Ticker | Bear | Upside | Ratio |
|---|---|---|---|---|---|---|---|---|
| VST | −4% | +52% | **13.1** | | GNRC | −37% | +15% | 0.41 |
| CEG | −16% | +47% | **2.9** | | HUBB | −34% | +13% | 0.39 |
| NRG | −17% | +40% | **2.4** | | NBIS | −68% | +25% | 0.37 |
| AVGO | −15% | +35% | **2.3** | | LRCX | −40% | +14% | 0.34 |
| XYL | −23% | +23% | 1.00 | | BE | −58% | +16% | 0.29 |
| GEV | −34% | +32% | 0.93 | | ANET | −45% | +12% | 0.27 |
| CCJ | −25% | +23% | 0.90 | | CAT | −34% | +7% | 0.21 |
| LITE | −33% | +28% | 0.83 | | SPXC | −36% | +7% | 0.18 |
| APLD | −53% | +41% | 0.77 | | FN | −35% | +5% | 0.14 |
| IRM | −21% | +14% | 0.66 | | AMAT | −40% | +4% | **0.11** |
| CLS | −41% | +26% | 0.64 | | MOD | −49% | +22% | 0.45 |
| ON | −38% | +23% | 0.60 | | MP | −47% | +21% | 0.45 |
| VRT | −31% | +16% | 0.53 | | MRVL | −42% | +20% | 0.47 |
| DLR | −24% | +11% | 0.43 | | | | | |

*Excluded for missing data: ENTG (bear price is a placeholder in the note — fix), TOELY and UUUU (no current price — on the manual-update list).*

---

## Transmission Groups: how fast each name dies if AI capex flatlines

**Group 1 — Immediate (revenue *is* AI capex; little backlog cushion).**
NBIS, APLD, BE, MOD, VRT, SPXC, ANET, AVGO, MRVL, LITE, FN, CLS + WFE (LRCX, AMAT, TOELY, ENTG — "capex-of-capex," historically the most violent correction). Bear cases hit within 2-4 quarters of a capex cut. This is **16 of 30 Buys**.

**Group 2 — Backlog-cushioned (contracted revenue converts even if new orders stop).**
GEV (sold out through 2029), CAT ($51B backlog), GNRC, HUBB, IRM, DLR (multi-year leases). Earnings hold for 1-2 years; the *multiple* compresses immediately. Cushioned ≠ immune.

**Group 3 — Partially independent demand.**
CEG, NRG, VST (power markets, PJM capacity, contracted PPAs — demand exists without AI), CCJ/UUUU (utility uranium contracting), MP (defense/EV), ON (auto SiC), XYL (water/municipal). These survive the scenario best — and notably, they hold 4 of the 5 best asymmetry scores.

**The pattern:** the market has already paid up for Group 1 (hence poor asymmetry) and still discounts Group 3. The book's best risk-adjusted exposure to the AI thesis is currently *through the power/commodity names, not the direct plays.*

---

## Scenario: "AI capex flatlines in 2027"

Assumptions: hyperscaler capex growth → 0% in 2027 (not a crash), Group 1 goes to bear prices, Group 2 goes halfway to bear (backlog converts, multiple compresses), Group 3 takes a 10% sentiment haircut.

Equal-weight portfolio impact: roughly **−30%** (Group 1: −41% avg × 16/27; Group 2: −16% avg × 6/27; Group 3: −10% × 7/27, weighted). A diversified-looking 30-name book behaves like a single levered position in one macro variable.

**No hedge leg exists.** Aschenbrenner solves this exact problem with shorts (NVDA, AVGO, SMH, MU). Options, none mutually exclusive:
1. Accept it knowingly — this is a thematic book; the 17.5% cash buffer in the sizing framework is the only shock absorber. (Legitimate — but it should be a *decision*, logged in [[Decisions Log]].)
2. Rebalance toward Group 3 / high-asymmetry names — the sizing framework's own rules already point here.
3. Add a hedge leg — e.g., SMH puts sized to Group 1 exposure. Track Aschenbrenner's short basket as the template.

---

## Actions

- [ ] Decide and log the hedge question (option 1, 2, or 3 above) — this is the single most important open portfolio decision
- [ ] Fix ENTG bear price (placeholder); price TOELY/UUUU manually and add to this table
- [ ] Re-run this analysis with actual tier weights once positions are sized (currently equal-weight)
- [ ] Re-run quarterly and after any >10% market-wide move; prices refresh automatically Fridays
- [ ] Sanity-check Group 1 bear prices against the WFE-cycle history (2018, 2022 corrections were −40-60% peak-to-trough — current bear cases are not conservative outliers)

---

*Method: bear prices from each note's scenario framework; current prices June 3-9, 2026 frontmatter. Asymmetry = (PT − current) ÷ (current − bear).*
