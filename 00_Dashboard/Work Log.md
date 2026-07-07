---
tags: [dashboard]
last_updated: 2026-07-07
---

# Work Log

## 2026-07-07

- **TOELY downgraded Buy→Hold; PT restated $270→$220, bear $110 (FX correction).** The ≤$215 re-eval trigger (6/29) fired on price and failed on asymmetry: USD/JPY ¥161.9 vs the ¥130 PT basis deflates bull ADR EPS to ~$4.82 → 45x ≈ $217; ADR trades ~3% *below* Tokyo parity ($214.55), so no discount cushion. Asym ~0.1x. T4 cash slot (reserved since 6/9) released. Upgrade path: FY27 H1 ¥-EPS ≥¥1,900 or ≤$150. Not a tape cut — FX flag predates the unwind. *(Rating)*
- **EoD push hardened against the sandbox git-lock wedge:** lock-aware Step 0 added to the scheduled task (detect stale locks → try mv → else write BLOCKED note with a paste-ready remediation line and stop). Durable fix staged in `_private/host-push/` — a host-side launchd script (same guard rules, keychain auth, cleans locks) + plist; install is 3 commands, then disable the Cowork eod-vault-push task. *(Process)*
- SMNEY derived price precision-fixed with live FX: $35.37 (ENR €154.74 × 0.2 × EURUSD 1.1427). *(Maintenance)*

## 2026-07-07

- **SMNEY resolved same day — PT $38 REINSTATED.** Went to the primary source: SEC F-6 POS **Amendment No. 1 (May 14, 2026)** to the Jan 30, 2026 Citibank Deposit Agreement, §2.03 — "Each ADS shall represent the right to receive 1/5 of each Share." The 6/29 correction was right; the contradicting $193.96 quote was an un-adjusted FMP vendor line (matches full-share value; SMEGF $183.80 ≈ ENR €154.74 × FX). **Standing rule: price SMNEY only as ENR.DE × 0.2 × EURUSD.** Derived ~$36.2 (ENR −9.2% today). Propagated to note/README/Hold PT Watch. *(Data integrity)*
- **PJM Jul 14 execution staged** → [[PJM_Execution_Prep_2026-07-14]]: branch table with live 7/7 asymmetry (CEG 6.4x, NRG 1.7x — both clear the bar; CEG only 9.2% above bear going in), staged add size (+2% each on a >$325 print, from cash), VST staged no-add (asym ~1.1x), same-day checklist. One open decision flagged: ratify the +2% add size before results. *(Catalyst prep)*
- **Standing level alerts added to the intraday monitor loop:** EME ≤$660 (add zone), MU <$900 and AVGO <$350 (bear floors → re-underwrite protocols). *(Process)*

## 2026-07-07

- **AVGO re-underwrite completed → Buy/$560 reaffirmed** (run proactively; day low $362.07 approached but did not breach the $360 trigger — earlier "trigger fired" language corrected in Market Review/Dashboard). All 3 invalidation triggers clean; **Apple custom-chip partnership extended through 2031** (7/6 filing) inverse-fires the customer-transition bear. New floor protocol: close <$350 → same-week formal re-underwrite. *(Rating)*
- **Valuation_Snapshots_All30.xlsx refreshed** (was frozen Jun 4): all prices re-marked to live 7/7; CAT $1,150, AMAT $680, LRCX $450, TOELY $270 ADR applied; **MU (Buy/$1,500/bear $900) added, replacing exited ENTG; ON re-marked Hold/$100/bear $65**; TOELY row completed (was N/A). Zero formula errors post-recalc. *(Models)*
- **Estimates Tracker expanded — new "Q3 Gauntlet (Jul–Aug)" sheet:** 16 reporters Jul 15–Aug 13 with Robinhood consensus EPS, prior-quarter surprise, price vs PT/bear, playbook triggers. Old Top-10 sheets marked stale (Bigdata.com consensus pending re-auth). *(Models)*
- **Seven report dates corrected from verified earnings data:** CAT Jul 29→**Aug 4**, ANET Jul 29→~Aug 4, NRG Aug 7→**Aug 4**, CEG Aug 7→~Aug 6, **BE Aug 6→Jul 28 (verified)**, NBIS Aug 14→~Aug 6, HUBB Jul 22→~Jul 28. Frontmatter updated; CAT re-underwrite timing moves to Aug 4 accordingly. SNDK gate context: Q4 consensus $33.38 vs the ≥$38 trigger; Q1 FY27 consensus $41.45 >> the ≥$35 guide gate. *(Maintenance)*

## 2026-07-07

- **Market Review written** → [[Market Review 2026-07-07]]: AI-unwind diagnosis (sentiment rotation, not thesis break), live damage assessment (NAV ~$96.7k, alpha vs SPY flipped −4.5pp), bear-proximity table (MU at the $900 floor; AVGO $360 re-underwrite trigger fired), and the 6-week catalyst execution map. *(Review)*
- **Three decisions logged** (see [[Decisions Log]] 7/7): KLAC revisit closed (Hold/$270 maintained, asym 0.79x at $212); SMNEY PT **suspended** on ADR-ratio data-integrity flag (live quote $193.96 implies ~1:1, not the 6/29 "confirmed" 1:5 — re-verify F-6); MU bear-touch re-underwrite protocol armed (close <$900 → formal re-underwrite anchored to SK Hynix Jul 24). *(Rating/Risk)*
- **Security: PAT removed from git remote URL.** Remote reset to a clean HTTPS URL. **Owed by Jonathan: revoke the exposed classic token on GitHub and mint a fine-grained token scoped to this repo only** — automated pushes will fail until re-authenticated (guard will write FAILED notes; expected). Note: the old token also sat in `.git/config` since ≤6/24 — treat as compromised. *(Security)*
- **Personal-holdings scrub:** P&L sections removed from all 9 public monitor files → `_private/Personal_Holdings_history.md` (`_private/` added to .gitignore); XPEL/GEV interview files moved out of the public repo (git rm --cached). History note: old sections remain in prior git commits — full remediation needs a history rewrite; flagged, not executed. *(Security)*
- **Push backlog cleared** — 7/3 + 7/6 guard blocks resolved (both were the Personal-Holdings section in the weekly monitor; root cause fixed by scrubbing + retargeting the weekly-refresh task to write personal P&L to `_private/`); EoD guard filename blocklist retired in favor of content checks. Manual push run this session. *(Maintenance)*
- **Hold PT Watch reconciled to the 7/7 tape** — selloff retired INTC/WDC/GLW/STX from the band; SNDK now 25% *below* stale PT into the Aug 13 gate; Lesson #3 counterpoint logged (anti-momentum Holds validated by −10–25% mean reversion). *(Process)*
- **Hygiene batch:** README coverage tables regenerated from frontmatter (8 stale PTs/ratings fixed, BW/EME/XYL now listed); SMNEY (Aug 6 est.) + TOELY (Jul 31 est.) `next_earnings` backfilled — coverage now 100%; GEV `bear_price: 600` added (DCF-floor re-underwrite due Jul 22); ACM/CORZ/OKLO/WOLF `review_deadline: 2026-07-31` set; 30 June intraday alerts archived to `08_Monitors/archive/2026-06/`; 0-byte GEV_DCF.md populated as model index; ASML print date standardized to **Jul 15** (7/16 references were wrong). *(Maintenance)*

## 2026-07-06

- EoD auto-push **BLOCKED** — guard triggered. See [[EoD_Push_BLOCKED_2026-07-06]]. *(Auto)*

## 2026-07-03

- EoD auto-push **BLOCKED** — guard triggered. See [[EoD_Push_BLOCKED_2026-07-03]]. *(Auto)*

## 2026-07-02

- **Three flagged decisions logged** (see [[Decisions Log]] 7/2): **CAT** batch Buy/$1,000 retro-logged + closed ✓ (first June-3 batch close — first Lesson #2 datapoint), PT raised to $1,150; **FCEL** PT reset $18→$26, Hold kept as explicit anti-momentum lean (Fit Energy 30MW firm < 100MW trigger); **MKSI** PT reset $310→$450, Hold confirmed (asym 0.43x), deep-dive due before Aug 5 print. Propagated to company notes + Model Portfolio (CAT row) + Hold PT Watch same session. FCEL note's stale "T4 maintained" position language corrected (no Model Portfolio position exists). *(Rating)*
- **Full vault review completed** → [[Vault Review 2026-07-02]]: security/pipeline items, untracked Hold-above-PT cohort (verified vs live 7/2 quotes), data-hygiene gaps, valuation-infrastructure roadmap, July catalyst readiness. *(Process)*
- **EoD push guard fixed** — check (c) now excludes negation disclaimers ("No entry prices, cost basis, or P&L included" was blocking mechanically); monitor skill footer wording standardized to a guard-safe phrase. *(Maintenance)*
- **Manual push: 14 files** (7/1 false-positive cleared after re-scan with corrected guard; all files verified clean). Stale `.git` lock files from 6/30 removed; stray `.write_test` deleted. *(Maintenance)*
- **`next_earnings` backfilled** across coverage notes missing it (incl. LRCX Jul 29 — was invisible to the Monday earnings-prep scan). *(Maintenance)*
- **Hold PT Watch expanded** — untracked at/above-PT Holds added (FCEL, MKSI, WDC, INTC, CRDO, PWR, SCCO, GLW, STX). *(Process)*
- **PJM playbook §7 corrected** — 2028/2029 BRA (not 2027/28); bids close Jul 7, results Jul 14 after 4pm ET. *(Maintenance)*

## 2026-07-01

- EoD auto-push **BLOCKED** — guard triggered. See [[EoD_Push_BLOCKED_2026-07-01]]. *(Auto)*

## 2026-06-30

- EoD auto-push: 13 file(s) committed and pushed to GitHub. *(Auto)*

## 2026-06-29

- **BW rated Hold/$18, bear $4.** Q1'26 10-Q reviewed. Going concern resolved; OCF positive for first time; revenue +44%; backlog $2.7B. Hold on asymmetry (0.39x), Dec'26 note maturity, APLD single-counterparty risk, and thin 20.3% gross margins. No position; upgrade gated on 2nd hyperscaler contract or notes refinanced. *(Rating)*
- **AVGO bear proximity check: Buy/$560 confirmed.** At $372.45, 6.4% above $350 bear. Three invalidation triggers not fired. OpenAI "Jalapeño" chip (Broadcom-designed) adds 5th major custom ASIC customer — directly refutes fragmentation bear. Re-underwrite trigger set at $360. *(Thesis check)*
- **GEV harvest band flag.** Closed $1,102.51, within 3.4% of $1,140 harvest trigger. No action — gated on Q2 earnings July 22 (backlog ≥105GW → raise PT; flat → harvest to T3). *(Monitor)*
- **ENTG bear placeholder resolved.** Bear $85 confirmed in §8 from verified adj. EBITDA multiples; dashboard checkbox cleared. *(Cleanup)*
- EoD auto-push: 15 file(s) committed and pushed to GitHub (false-positive guard cleared — all flagged sequences were SEC EDGAR CIK/accession numbers). *(Auto)*

## 2026-06-26

- EoD auto-push **BLOCKED** — guard triggered. See [[EoD_Push_BLOCKED_2026-06-26]]. *(Auto)*

> Dated record of completed work on the vault — research passes, verifications, framework changes, and maintenance. This is the **process** changelog; investment buy/sell/rating decisions live in [[Decisions Log]], and the open queue is tracked on the Work Board. Newest first; substantive items only.

## 2026-06-25

- EoD auto-push: 8 file(s) committed and pushed to GitHub (after manual guard cleanup). *(Auto)*
- **MU upgraded Hold→Buy; post-earnings actions complete.** Q3 FY2026: revenue $41.46B (+346% YoY, beat by $5.87B), non-GAAP EPS $25.11 (beat by $4.51), GM 84.9%. Q4 guide $50.0B ±$1.0B (vs $42B playbook upgrade threshold; cleared by $8B); HBM4 ramping 2x faster than HBM3E; 16 SCAs (~$22B) locked. PT $1,100→$1,500. Added T2 (4%) in Model Portfolio at $1,165.94. FQ4 FY2026 playbook entry added (~Sep 25, 2026). Read-throughs: LRCX/AMAT/ASML all positive; SNDK NAND upgrade deferred. *(Earnings)*
- **Monitor generator hardened** — removed the Model Portfolio cross-reference (entry price / shares / cost-basis P&L) from `upstream-portfolio-monitor/SKILL.md`. Future intraday alert files will report only current price, daily move %, bear-case price, and distance to bear. Entry prices and position sizing belong in Model Portfolio.md, not in monitor outputs. *(Maintenance)*
- EoD auto-push **FAILED** — stale `.git/index.lock` blocking git add/commit; sandbox cannot remove lock files on bindfs mount. See [[EoD_Push_FAILED_2026-06-25]]. *(Auto)*

## 2026-06-24

- **Security & privacy hardening of the public repo.** Removed a real account identifier and all personal-holdings P&L (real positions and entry prices) from the monitor files; cleaned a credential out of the git remote; added `.gitignore`, `DISCLAIMER.md`, and a README disclaimer. The vault now publishes only the hypothetical paper book. *(Maintenance)*
- **MU Q3 FY2026 earnings** reported after the close; read-through reviewed for the held WFE/materials cluster (LRCX / AMAT / ENTG). Post-earnings note and frontmatter update queued on the Work Board. *(Earnings)*

## 2026-06-23

- **Catalyst Playbooks ratified** — six dated decision trees (MU, ASML, GEV, LRCX, PJM, VST) locked against current notes and prices, with three corrections carried through the vault: VST bear $105 / asymmetry ~1.1x, LRCX PT $450, and ASML reframed as a PT-reset event. *(Process)*
- **Model Portfolio reconciliation** — price targets and ratings aligned to the company notes (AMAT $680, LRCX $450; ENTG downgraded to Hold, PT pulled). No position changes. *(Process)*
- **Q3 quarterly screener run** — top find EME (4/5; initiation queued); POWL / CLF / TH added to the watch list. *(Screener)*
- **Thesis stress test / invalidation sweep** across the book — no sell triggers fired. *(Process)*
- Verification round 2 completed for AMAT (10-K), TOELY, LRCX, ENTG, CCJ, KLAC, and ASML. *(Verification)*

## 2026-06-20

- **TOELY price target restated to $270 (ADR)** — corrected a Tokyo-vs-ADR denomination error behind the prior $403 target; rebuilt on FY2027 base-case EPS. *(Verification)*
- Weekly NAV verification (paper book +9.76% vs inception; Juneteenth market holiday handled). *(Process)*

## 2026-06-19

- **First weekly verification pass** — cleared the bulk of unverified-claim flags on the priority Buy names: AMAT (27 flags), plus LRCX, ENTG, CCJ, KLAC, ASML, and SMNEY rounds. Several material corrections logged (e.g., AMAT PT $520→$680; ASML China revenue ~13%→~29%). *(Verification)*
- First NAV mark of the paper book; **MU earnings prep** completed ahead of the June 24 print. *(Process)*

## 2026-06-09

- **Vault inception.** Launched the hypothetical $100,000 Model Portfolio (29 names at tier-midpoint weights), benchmarked against SPY and SMH. Swept 295 unverified-claim flags across the company notes into the [[Verification Worklist]]. *(Process)*

---

*How this stays current: when an item on the Work Board moves to Done, a one-line curated entry is appended here. Micro-tasks are not logged — only work worth a durable, public record.*
