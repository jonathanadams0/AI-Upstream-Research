---
type: intraday-alert
date: 2026-07-10
time: 15:00 CT (market close)
alerts_fired: [bear_proximity, data_quality]
tickers_flagged: [FN, CCJ, VST]
---

# Intraday Alert — 2026-07-10 15:00 CT (Market Close)

Alert conditions firing at close. **FN remains within 10% of its body-stated bear case.** Two additional items: frontmatter `bear_price` fields for CCJ and VST are stale and need correction — prior intraday alerts (14:06 CT) flagged these incorrectly. Flag for review — no rating changes, no trades.

---

## Summary Table

| Ticker | Current | Daily % | Bear | vs Bear |
|--------|---------|---------|------|---------|
| FN | $470.92 | –2.46% | $450.00 | +$20.92 (+4.6%) ⚠ NEAR BEAR |

---

## Alert Detail

### FN — Fabrinet | ALERT (b): Within 4.6% of bear-case price

- Current: $470.92 | Bear case: $450.00 (body-confirmed) | Gap: +$20.92 (+4.6%)
- Down –2.46% today (prev close $482.78); no identified >5% catalyst
- Bear case per note body: "Key OEM customers lose market share in optical transceiver market; industrial segments fail to offset." Gross margin below 9% and two top-3 OEM orders cut >20% in same quarter are the formal rating-change triggers.
- **Near-bear zone reached.** Monitor for optical/interconnect demand signals ahead of next earnings (2026-08-18). No thesis trigger implicated yet.

---

## Data Quality Flags — Action Required

Two frontmatter `bear_price` fields are incorrect and generated false signals in the 14:06 CT alert. These need manual correction.

### CCJ — Frontmatter bear_price: 107 → Should be: 85

The body (Section 11) states: *"Implied Bear Price: $85 (~21% downside from ~$107 current)"* — meaning $107 was the **current price at time of writing**, not the bear case. The frontmatter was populated incorrectly. At today's close of $95.97, CCJ is **+12.9% above its actual $85 bear case** — no breach, no proximity alert. The 14:06 CT alert flagged CCJ as "BELOW BEAR" based on the wrong $107 figure.

> **Fix:** Update `bear_price: 107` → `bear_price: 85` in CCJ.md frontmatter.

### VST — Frontmatter bear_price: 145 → Should be: 105

The body (Section 11) explicitly states: *"The prior $145 figure was a placeholder (only ~4% below the old entry) and is retired. Re-underwritten 2026-06-23 at $105."* At today's close of $158.80, VST is **+51% above its actual $105 bear case** — no proximity alert. The 14:06 CT alert flagged VST as "Within 9.8% of bear-case price" based on the retired $145 figure.

> **Fix:** Update `bear_price: 145` → `bear_price: 105` in VST.md frontmatter.

---

## BE — Close Call (Not Firing)

BE closed at $244.68, down **–4.80%** from prior close of $257.02 — just below the ±5% alert threshold. Context from earlier today's 14:06 CT alert: Hunterbrook short report on scandium supply chain + multiple securities law firm investigations. Stock has recovered ~$3 from intraday lows. Bear case is $120.00 (+103.9% above current) — not implicated. Monitor for further short-report follow-up.

---

## Standing Level Alerts — All Clear

| Alert | Trigger | Current | Daily % | Status |
|-------|---------|---------|---------|--------|
| EME add-zone | ≤$660 | $782.08 | –0.17% | Clear (+18.5% above trigger) |
| MU bear floor | <$900 | $979.11 | –1.26% | Clear (+8.8% above floor) |
| AVGO bear floor | <$350 | $399.99 | –0.28% | Clear (+14.3% above floor) |

**MU note:** At $979 and –1.26% today, MU is 8.8% above the $900 bear floor. Not flagging yet but approaching the 10% proximity zone. Watch next session.

---

Prices and bear-case distances only — no position data included.
