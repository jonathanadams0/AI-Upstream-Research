---
tags: [dashboard, review]
last_updated: 2026-07-02
---

# State of the Vault — Comprehensive Review (July 2, 2026)

> Full-vault audit: every dashboard file read, frontmatter extracted from all 75 company files, monitors/reports/models/git inspected, and the Hold-above-PT findings verified against **live July 2 quotes** (market broadly red today). Organized as: what's working → what's broken → prioritized fixes.

---

## 1. Where the vault stands

The vault is close to institutional-grade in **process**: a Decisions Log with same-day entries, methodology-level hit-rate scoring, and codified lessons; ratified pre-committed Catalyst Playbooks; a rules-bound $100k paper book benchmarked to SPY/SMH; and a Verification Worklist that has burned down ~295 unverified-claim flags to roughly 20 low-priority stragglers across 9 notes. Very few individual investors have any of this; almost none have all of it.

The gap to "investment grade" is now concentrated in three places: **(a) coverage-wide rating discipline** — the Lesson #3 error (stale conservative Holds) is being policed on 7 names while at least 7 more sit above their PTs untracked; **(b) data hygiene feeding the automation** — missing `next_earnings` fields, a stale public README, and an over-eager EoD push guard; and **(c) valuation infrastructure** — models and snapshots frozen at June 3–4, before the quarter's biggest rating actions.

**Scoreboard context:** Q2 closed 4 decisions at 25% hit rate (1✓/1~/2✗); the only validated methodology is earnings-driven PT raises (1/1). Model portfolio +4.0% vs inception at last mark (6/26), +5.1pp vs SPY, +0.9pp vs SMH.

---

## 2. Urgent — security and pipeline integrity

**2.1 Git credential handling.** The local git configuration stores authentication in a way the 6/24 hardening session intended to eliminate (details flagged privately — not reproduced here since this repo is public). Action: rotate the credential on GitHub, re-add the remote without embedded auth, and use the macOS keychain (`git config credential.helper osxkeychain`) or a fine-grained deploy token scoped to this one repo. Update the EoD push task accordingly.

**2.2 EoD push guard is blocking on its own disclaimer.** Three of the last five trading days blocked (6/26, 6/29 false-positive, 7/1). The guard mechanically matches "cost basis" — including in the monitor template's *negation* line ("No entry prices, cost basis, or P&L included"). Nine files from 7/1–7/2 sit unpushed right now. Fix either side: reword the monitor disclaimer to avoid trigger phrases (e.g. "Prices only — no position data included"), or make the guard skip lines that match a known-safe allowlist. Then clear the 7/1 blocked push.

**2.3 Repo hygiene.** Stray `.write_test` at root; empty `reports/` directory (duplicate of `07_Reports/`); `XPEL_Interview_Talking_Points.md` and `GEV_Walkthrough_Script.md` at root are personal/interview artifacts in a **public** research repo — move to a private location or a gitignored `_private/` folder.

---

## 3. Rating discipline — the untracked Lesson #3 cohort

[[Hold PT Watch]] exists precisely to catch conservative Holds the market overruns, but its curated table covers only 7 names. Frontmatter + live 7/2 quotes surface these **untracked** Holds at or above PT:

| Ticker | Hold PT | Live 7/2 | vs PT | Note depth | Comment |
|---|---|---|---|---|---|
| **FCEL** | $18 | $28.73 | **+60%** | 71 lines | Worst offender. Closed "~" at $21.82 on 6/23 and left at Hold/$18 — the PT is now decorative. Re-underwrite or explicitly re-log the Hold. |
| **MKSI** | $310 | $384.19 | **+24%** | thin | Never appeared in any watch list. PT reset needed. |
| **SCCO** | $165 | $173.59 | +5.2% | thin | Above PT. |
| **INTC** | $120 | $124.99 | +4.2% | — | Closed ✗ 6/23; PT never reset after scoring. |
| **WDC** | $560 | $574.00 | +2.5% | 41 lines | Was +21% above PT at the 6/26 mark ($675); still above after today's selloff. |
| **CRDO** | $250 | $254.54 | +1.8% | 60 lines | Entered the band. |
| **PWR** | $680 | $687.25 | +1.1% | thin | Entered the band. |
| GLW | $210 | $210.16 | 0% | 58 lines | At PT exactly. |
| STX | $910 | $874.54 | −3.9% | 35 lines | Inside the 5% band (was +13% above at 6/26 mark). |

Actions: add all of these to the Hold PT Watch table; run the Rule-of-the-note decision (reset PT or log the active lean) on FCEL, MKSI, WDC, and INTC first. Note the live Dataview query *would* have caught most of these — the curated table simply hasn't been reconciled against it since 6/29. Make that reconciliation an explicit step in the Friday refresh.

**Also open from the 7/1 scoring pass:**
- **CAT** — Buy/$1,000 from the June 3 batch; traded through PT ($1,020.77 on 7/1; $983.93 today). Still lacks an individual Decisions Log entry. Write it now while the touch of PT is fresh — this is also the first *Buy-PT-hit* from the batch cohort, relevant to Lesson #2's pending test.
- **KLAC** — Hold/$270 was set below market at initiation (~$277); June 30 closed $301.71, today $246.30. The ±20% two-day swing is exactly why the revisit should anchor on a fresh comps pass, not a price snapshot.

**Under Review limbo:** ACM, CORZ, OKLO, WOLF have sat Under Review since early June with no logged resolution path or deadline. Either rate them, drop them from coverage, or add a "resolve by" date to each.

**Thin-note ratings:** 12 company notes are under 50 lines yet carry ratings and PTs (IREN, HUT, STX, ACM, COHR, EQIX, MPWR, OKLO, WDC, CORZ, WOLF, TSEM). Several are the same names now testing their PTs. Suggest tagging these `mode: screening` in frontmatter so dashboards can visually distinguish underwritten ratings from screening-mode placeholders — and prioritize deepening any that enter the Hold PT Watch.

---

## 4. Data hygiene feeding the automation

**4.1 `next_earnings` missing on ~17 names — including LRCX.** The Monday 8 AM earnings-prep automation scans this field; the Upcoming Earnings dashboard query depends on it. Missing: **LRCX (Jul 29 — a ratified playbook event)**, KLAC, AMAT, CCJ, ENTG, ETN, FCX, MKSI, MOD, NVT, OKLO, PWR, SCCO, SMNEY, TOELY, TT, VRT. As it stands the automation will not flag LRCX 14 days out (that window opens ~July 15). Highest-leverage 20-minute fix in this review.

**4.2 README.md coverage table is badly stale** (public-facing, so it's the first thing a repo visitor sees). It still shows: AMAT $520 (→$680), TOELY Buy/$403 (→$270), ENTG Buy/$155 (→Hold, PT under review), MU Hold/$1,100 (→Buy/$1,500), ON Buy/$160 (→Hold/$100), KLAC $1,950 (→$270 post-split), SMNEY $175 (→$38), GLW unrated (→Hold/$210). BW, EME, and XYL are absent entirely; ACM is listed under Semi-Materials. Since every number exists in frontmatter, the durable fix is a small script that regenerates the README tables from frontmatter as part of the EoD push.

**4.3 Static snapshots drifting.** Portfolio Summary (June 4/9) and the Dashboard "Coverage Statistics" table (June 9) both predate BW/EME initiations and five rating actions. Both carry warning banners, which helps — but consider regenerating them at each quarterly review or retiring them in favor of the Dataview tables.

**4.4 PJM playbook needs a date + label fix.** The 7/1 monitor confirmed: Playbook §7's "(2027/2028 delivery year)" is a typo — that BRA cleared 12/17/25 at $333.44/MW-day. The live event is the **2028/2029 BRA: bids close July 7, results July 14 after 4pm ET**, price cap ~$325 ≈ the add-branch threshold. Update §7 and the calendar placeholder (currently a generic July 1 stub) to July 14.

**4.5 Minor:** `04_Models/GEV_DCF.md` is a 0-byte file (delete or populate); Model Portfolio change log has the 7/1 entry inserted out of chronological order; ASML print date appears as both July 15 and July 16 across the vault (frontmatter says 7/15 — verify once and standardize).

---

## 5. Valuation infrastructure — the thinnest layer

This is the biggest structural gap between "great process" and "investment grade research shop":

1. **Models are frozen pre-quarter.** All 4 DCFs (GEV/CEG/VST/NRG) plus Valuation_Snapshots_All30 and Estimates_Tracker_Top10 were last touched June 3–4 — before the MU upgrade to $1,500, AMAT $680, LRCX $450, the KLAC split, the ON downgrade, and the SMNEY reset. Refresh the snapshot workbook and tracker before the July earnings gauntlet.
2. **Model coverage is 4 of ~30 Buys, all in one sector.** Given Lesson #1 (DCF misprices supply-constrained backlog names) and the scoreboard (revised-estimates 1/1, DCF 0/1), don't build more DCFs — build the lightweight thing that's actually winning: a one-tab **NTM-EPS × multiple model per Buy name** with base/bull/bear EPS and the multiple justified against comps. That's ~30 minutes each and makes every PT auditable the way KLAC's and EME's now are.
3. **Estimates tracker covers 10 names.** Expand to all Buy-rated reporters between July 15 and Aug 13 (ASML, GEV, LRCX, VST, CEG, NRG, HUBB, CAT, ANET, DLR, IRM, SPXC, GNRC, XYL, MP, UUUU, APLD, NBIS...) so beats/misses can be scored against your numbers, not just consensus.

---

## 6. Monitors and reports

**Monitor volume.** ~6 intraday alert files/day → 58 files in `08_Monitors/` after one month; at this cadence it's ~120 by September. Adopt a retention policy: keep Catalyst_Reaction, Thesis_Stress_Test, and portfolio monitors forever; roll intraday alerts into monthly archive subfolders (`08_Monitors/archive/2026-06/`) unless they fired an action. The signal (alerts that led to decisions) is drowning in routine no-action snapshots.

**Reports duplication.** `07_Reports/` keeps md+docx or md+html pairs of the same deliverable. Fine, but pick a rule (md is source-of-truth, docx/html are exports) and note it in the folder so future cleanup doesn't delete the wrong one.

**05_Sources is underweight.** Two source notes against 60 covered names. The Verification Worklist did the work of primary-source reading — but the extracted facts live in company-note change logs rather than reusable source notes. For the big July prints, consider one source note per 10-Q/10-K read, per the existing template.

---

## 7. July–August catalyst readiness (the next 6 weeks decide the track record)

| Date | Event | Playbook | Readiness gap |
|---|---|---|---|
| Jul 7 | Samsung Q2 flash (DS OP) | §3 pre-note | — |
| Jul 7→14 | **PJM 2028/29 BRA** bids close → results | §7 | Fix delivery-year label + calendar; CEG/NRG add branches are the book's biggest pre-committed action |
| Jul 15/16 | **ASML Q2** — ratified PT-reset event | §4 | 9 low-priority flags open; standardize the date; PT reset is mandatory on all branches |
| Jul 22 | **GEV Q2** — largest position; harvest band $1,140 | §5 | Prep exists; refresh with 7/x price |
| Jul 24 | SK Hynix Q2 (macro input) | §2 | — |
| Jul 29 | **LRCX Q4 FY26** | §6 | **`next_earnings` missing → automation blind**; fix now |
| Jul 30–31 | Samsung Q2 full; EME Q2 (Jul 30) | §3 | EME upgrade trigger: RPO >$16.5B + EPS ≥$7.50 + guide ≥$31 |
| Aug 7 | VST Q2 + Cogentrix status | §8 | Bear re-underwrite done ($105); adds gated correctly |
| Aug 13 | SNDK Q4 — three-condition upgrade gate | §11 | Stock back to $1,904 (below $2,000 PT) — asymmetry improving toward the gate |

Also live: **EME** $795.91 today, down 14% from the $925 initiation mark and drifting toward the ≤$660 add zone — worth a standing alert. **NAV mark due Friday July 3** — half-day/holiday-adjacent session; handle like the Juneteenth precedent.

**Open queue items confirmed still open:** WMB evaluation (screener 4/5, slipped from Q2), "read latest 10-Q for each Buy" (dashboard to-do), price alerts setup. One stale checkbox: the Dashboard to-do still shows "Decide the hedge question" unchecked — it was decided and logged 6/25 (Option 1, accept asymmetry + Group-1 guardrail). Check it off.

---

## 8. Prioritized action list

**Today / this week**
1. Rotate the GitHub token; move credentials out of the remote URL. (§2.1)
2. Fix the EoD guard false-positive (reword monitor disclaimer); push the blocked 7/1–7/2 files. (§2.2)
3. Backfill `next_earnings` on all 17 names — LRCX first. (§4.1)
4. Write the CAT individual Decisions Log entry (PT touched). (§3)
5. Add FCEL/MKSI/WDC/INTC/CRDO/PWR/SCCO/GLW/STX to Hold PT Watch; run PT resets on FCEL and MKSI. (§3)
6. Update PJM playbook §7 (2028/29 BRA, results Jul 14) + calendar event. (§4.4)

**Before July 15 (earnings gauntlet opens)**
7. Refresh Valuation_Snapshots + Estimates_Tracker; expand tracker to all July/August Buy reporters. (§5)
8. Regenerate README coverage tables from frontmatter (script it into the EoD push). (§4.2)
9. Resolve or deadline the four Under Review names (ACM, CORZ, OKLO, WOLF). (§3)
10. KLAC rating revisit with fresh comps. (§3)

**Structural (quarterly-review scope)**
11. One-tab EPS × multiple model per Buy name; DCFs demoted to bear-case floors per Lesson #1. (§5)
12. Monitor retention policy + archive subfolders. (§6)
13. Tag screening-mode notes in frontmatter; deepen any that hit a watch list. (§3)
14. WMB evaluation; Lesson #2 batch-vs-deliberated test at the September review (CAT close will be its first datapoint). (§7)

---

*Method note: ratings/PTs pulled from YAML frontmatter across all 75 files in `03_Companies/`; "live" prices are July 2, 2026 intraday quotes (broad tape red −1–5%); dashboard/monitor/git findings from direct inspection. Prices move — re-verify §3 gaps before acting.*
