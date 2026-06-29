---
tags: [monitor, eod-push, blocked]
date: 2026-06-26
---

# EoD Push BLOCKED — 2026-06-26

Guard triggered. Review before pushing manually:

- 03_Companies/AMAT.md | [account-number: 10+ consecutive digits]
- 03_Companies/ASML.md | [account-number: 10+ consecutive digits]
- 03_Companies/BW.md | [account-number: 10+ consecutive digits]
- 03_Companies/CCJ.md | [account-number: 10+ consecutive digits]
- 03_Companies/ENTG.md | [account-number: 10+ consecutive digits]
- 03_Companies/KLAC.md | [account-number: 10+ consecutive digits]
- 03_Companies/VST.md | [account-number: 10+ consecutive digits]
- 08_Monitors/Portfolio Monitor 2026-06-26.md | [real-holdings language]

Note: The 10-digit sequences in company files appear to be SEC EDGAR CIK/accession numbers (e.g., 0001628280), not bank account numbers. The Portfolio Monitor flag is due to "Personal Holdings P&L" and "Cost Basis" column headers. Review and push manually after confirming.

To push manually after fixing:
  cd "$VAULT" && git add -A && git commit -m "manual push 2026-06-26" && git push origin main
