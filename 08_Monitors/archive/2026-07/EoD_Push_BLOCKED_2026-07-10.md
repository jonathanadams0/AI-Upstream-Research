---
tags: [monitor, eod-push, blocked]
date: 2026-07-10
---

# EoD Push BLOCKED (host) — 2026-07-10

Guard triggered. Review before pushing manually:

- .obsidian/graph.json — [account-number: 10+ consecutive digits]
- 03_Companies/GEV_Q2_prep.md — [account-number: 10+ consecutive digits]

---
**RESOLVED 2026-07-13.** Both flags were false positives: `.obsidian/graph.json` = Obsidian force-layout floats (0.518713…, 0.673731…), `GEV_Q2_prep.md` = 10-digit runs inside Bigdata hex document-accession IDs in citation URLs. Fixed by rounding the floats and annotating the citation lines; guard regex updated in `_private/host-push/eod-vault-push-host.sh` (skip `.obsidian/`, exempt Bigdata doc URLs). No account data was ever present.
