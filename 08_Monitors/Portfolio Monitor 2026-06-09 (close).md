# Upstream Portfolio Monitor — June 9, 2026 (Weekly Vault Price Refresh)

*Automated weekly refresh | Prices as of June 9 market close (4:00 PM ET) via Robinhood quotes. FMP quote and chart endpoints remain blocked on current plan.*

*57 of 58 company notes refreshed (`current_price` + `last_updated: 2026-06-09`). Note: an intraday monitor for today already existed, so this note uses the "(close)" suffix per the June 4 convention.*

---

## Week's Biggest Movers (>±5% vs. prior frontmatter price, baseline mostly 6/3–6/4)

| Ticker | Old → New | Change | Rating |
|--------|-----------|--------|--------|
| FCEL | $24.40 → $17.49 | -28.3% | Under Review |
| WOLF | $61.06 → $48.86 | -20.0% | Under Review |
| MP | $65.99 → $54.35 | -17.6% | Buy |
| OKLO | $67.23 → $56.47 | -16.0% | Under Review |
| FN | $687.07 → $586.49 | -14.6% | Buy |
| MRVL | $308.83 → $266.88 | -13.6% | Buy |
| GLW | $200.40 → $173.88 | -13.2% | Hold |
| TSEM | $259.34 → $228.24 | -12.0% | Hold |
| CLS | $420.27 → $371.64 | -11.6% | Buy |
| COHR | $401.13 → $355.95 | -11.3% | Hold |
| NBIS | $248.01 → $220.13 | -11.2% | Buy |
| IREN | $60.75 → $54.02 | -11.1% | Hold |
| WDC | $582.65 → $517.99 | -11.1% | Hold |
| CCJ | $113.94 → $102.28 | -10.2% | Buy |
| HUT | $125.28 → $112.61 | -10.1% | Hold |
| ON | $129.91 → $117.00 | -9.9% | Buy |
| SCCO | $192.20 → $174.94 | -9.0% | Hold |
| VRT | $318.31 → $289.59 | -9.0% | Buy |
| CRDO | $214.89 → $234.23 | **+9.0%** | Hold |
| LITE | $901.25 → $821.68 | -8.8% | Buy |
| STX | $926.65 → $845.69 | -8.7% | Hold |
| BE | $283.32 → $259.58 | -8.4% | Buy |
| ANET | $164.90 → $152.19 | -7.7% | Buy |
| FCX | $69.61 → $64.23 | -7.7% | Hold |
| CORZ | $29.05 → $27.02 | -7.0% | Under Review |
| GNRC | $277.82 → $260.78 | -6.1% | Buy |
| NVT | $174.26 → $163.83 | -6.0% | Hold |
| ENTG | $141.81 → $134.34 | -5.3% | Buy |
| MPWR | $1,617.75 → $1,531.98 | -5.3% | Hold |
| AVGO | $413.90 → $392.74 | -5.1% | Buy |

Context (per today's intraday monitor): broad risk-off across AI/semis — geopolitical concerns plus expected SpaceX IPO capital absorption. The breadth of the decline (29 of 30 movers down) points to market beta, not name-specific thesis breaks. FCEL actually rose +12.8% *today* (prev close $15.50); its -28% is the full-week move from the 6/3 baseline.

---

## Buy-Rated: PT / Bear-Case Proximity

- **No Buy-rated name traded through its bear-case price.** Closest: AVGO $392.74 vs. bear $350 (12% above); MRVL $266.88 vs. bear $180; FN $586.49 vs. bear $450.
- **AMAT $499.54 — within 5% of its $520 PT** (3.9% below). The only Buy name near its target after this week's selloff. Worth a review of whether the PT still has headroom or the position is approaching full value.

---

## Thesis Invalidation Tracker — Flags (flag only, no re-rates)

| Ticker | Move | Trigger Plausibly Touched | Action |
|--------|------|---------------------------|--------|
| MP | -17.6% | "China removes rare earth export restrictions" — a drop this size out of proportion to the sector is consistent with policy-easing headlines | Verify China MOFCOM news this week |
| CCJ / UUUU | -10.2% / n.a. (UUUU -5.5% today) | "Uranium spot below $60/lb" — coordinated uranium-name weakness warrants a spot price check | Check UxC weekly spot |
| MRVL | -13.6% | "Amazon or Microsoft delays Trainium 3 / Maia 3" — decline exceeds sector beta | Verify any AWS/MSFT custom-silicon news vs. pure market contagion |

All other movers look like market-wide risk-off; no fundamental trigger evidence in price action alone.

---

## Personal Holdings P&L

*Section removed 2026-07-07 — personal holdings data is no longer stored in the public vault. See `_private/` (gitignored).*

---

## Skipped / Manual Update Needed

- **SMNEY** — not resolvable via Robinhood quotes (also historically unresolvable via Bigdata.com and FMP). Frontmatter left untouched (`last_updated: 2026-06-03`, no current_price). Manual price update needed.
- TOELY, TT, UUUU, BW — successfully priced this run via Robinhood ($189.37, $470.35, $14.37, $15.49); `current_price` fields added where previously missing.

---

## Status

**Prices refreshed; no rating or PT changes made.** Three tracker flags above need verification; AMAT approaching PT.
