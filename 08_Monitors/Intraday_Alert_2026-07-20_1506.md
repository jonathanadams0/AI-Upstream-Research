---
tags: [monitor, intraday-alert]
date: 2026-07-20
time_ct: "15:06"
---

# Intraday Alert — 2026-07-20 15:06 CT (market close)

## Summary

Closing-bell read. APLD and BE both closed >5% movers in opposite directions — APLD extending the sector-wide data-center rebound, BE giving back ground on a fuel-cell pair-trade split (FCEL up, BE down). CCJ closed through its $85 bear case for a fifth consecutive hourly read, still with no negative company-specific catalyst identified. AVGO, FN, and MRVL remain within 10% of their bear cases on proximity only. MU's standing $900 alert (Decisions Log 2026-07-07) is technically live at the close, but the vault's own MU note shows the operative bear case was cut to $800 that same day — worth flagging as a stale-threshold check rather than a fresh deterioration signal.

## Triggered Conditions

1. **Buy names >5% daily move:** APLD (+8.0%), BE (−8.2%)
2. **Bear-case within 10% / breached:** CCJ closed through its $85 bear case; AVGO, FN, and MRVL all within 10% of bear
3. **Standing level alert (Decisions Log 2026-07-07):** MU closed at $866.28, below the $900 threshold cited in the standing alert — see data-quality note below
4. **EME add-zone ($660):** not reached — closed ~$743, ~11% above the add-zone trigger

## Portfolio Snapshot

| Ticker | Current | Daily % | Bear | vs Bear |
|---|---|---|---|---|
| APLD | $27.85 | +8.0% | $20.00 | +28.2% |
| BE | $197.28 | −8.2% | $120.00 | +39.2% |
| CCJ | $84.85 | −0.9% | $85.00 | **−0.2% (breached)** |
| AVGO | $378.21 | +2.0% | $350.00 | +7.5% |
| FN | $494.79 | +3.4% | $450.00 | +9.0% |
| MRVL | $195.03 | +3.4% | $180.00 | +7.7% |
| MU | $866.28 | +2.0% | $800.00 | +7.7% (also below $900 standing threshold) |

## What Moved and Why

**APLD +8.0%** — Sector-wide data-center rebound: 24/7 Wall Street reports IREN, Applied Digital, TeraWulf, and Core Scientific all sharply higher Monday; Benzinga frames APLD as oversold with a bullish momentum score ahead of earnings. No fresh company-specific catalyst — this is a broad reversal off last week's AI-infra selloff.

**BE −8.2%** — 24/7 Wall Street flags a fuel-cell pair-trade split: FCEL up ~6% while BE is down on the same day, framed as rotation within the group rather than a BE-specific negative. Also in today's tape: a 13F showing BNY Mellon trimmed its BE stake ~29% (filing reflects a prior quarter, not new selling). No thesis-relevant news found. Still well above bear case (+39%).

**CCJ closed through bear case, −0.9%** — No adverse company-specific news; today's CCJ coverage is constructive-to-neutral (DOE's Nuclear Fuel Cycle Consortium announcement, sector-rebound commentary, confirmation Cigar Lake/McClean Lake are back online). The breach continues to read as sector risk-off (semis/uranium complex) rather than a name-specific catalyst, consistent with the 7/13 note in CCJ.md. Formal re-underwrite watch remains armed per that note.

**AVGO / FN / MRVL, within 10% of bear** — Ordinary daily moves (+2.0%, +3.4%, +3.4%); no negative catalysts found. Proximity-only triggers, unchanged in character from recent sessions.

**MU standing alert — data-quality flag** — MU.md shows the bear case was re-underwritten from $900 to $800 on 2026-07-07 (same date as the Decisions Log entry the standing alert cites), and today's tape is constructive: a Seeking Alpha upgrade to Buy, and Motley Fool/Investopedia/247 Wall Street all covering Morgan Stanley's Joseph Moore calling last week's memory selloff a buying opportunity. MU closed +2.0% at $866.28. Against the current $800 bear this is a routine 7.7% proximity read, not a breach. Against the $900 figure hardcoded in the standing-alert instruction, it technically still fires — but that $900 threshold appears superseded by the same-day $800 re-underwrite and may need to be updated in the monitor's standing rules.

## Flag for Review

- CCJ: bear case breached at the close for a fifth straight hourly read with no negative catalyst identified — worth a thesis check on whether $85 still holds, per the re-underwrite protocol already armed in CCJ.md.
- MU: standing-alert threshold ($900) looks stale versus the vault's own $800 re-underwritten bear case (both dated 2026-07-07) — recommend updating the standing rule to $800, or confirming $900 was intentional.
- BE: −8.2% close with no adverse company-specific catalyst found; monitor for a name-specific driver if the move persists into tomorrow.
- Separately, VST.md's frontmatter (`bear_price: 145`) is stale — the note body explicitly retired that figure on 2026-06-23 in favor of $105. This alert used $105. VST would show as within-10%-of-bear ($145 basis) if the frontmatter is used instead of the note text; worth reconciling frontmatter to avoid inconsistent reads across tools.
- APLD / AVGO / FN / MRVL: no action implied — sector-wide rebound and proximity-only triggers respectively.

No ratings or trades changed. This is a flag for analyst review only.

---
Prices and bear-case distances only — no position data included.
