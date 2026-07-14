---
tags: [monitor, eod-push, failed]
date: 2026-06-25
---

# EoD Push FAILED — 2026-06-25

Git operation blocked by stale lock files that the sandbox cannot remove (bindfs mount permission restriction).

## Error Output

```
fatal: Unable to create '.git/index.lock': File exists.
fatal: Unable to create '.git/index.lock': File exists.
error: update_ref failed for ref 'refs/remotes/origin/main': cannot lock ref 'refs/remotes/origin/main': Unable to create '.git/refs/remotes/origin/main.lock': File exists.
```

## Root Cause

Stale lock files exist at:
- `.git/index.lock`
- `.git/refs/remotes/origin/main.lock`

These appear to be left over from a previous git operation. The sandbox (bindfs FUSE mount) cannot remove them — `rm` returns `Operation not permitted`. No git process was running at the time of this attempt.

## Files That Would Have Been Committed (all passed guard checks)

- `README.md`
- `08_Monitors/Catalyst_Reaction_MU_2026-06-25.md`
- `08_Monitors/Intraday_Alert_2026-06-25_0908.md`
- `08_Monitors/Intraday_Alert_2026-06-25_1005.md`

## To Push Manually After Fixing

```bash
cd "/Users/jono/Desktop/Projects/Upsteam AI Equity Research"
rm .git/index.lock .git/refs/remotes/origin/main.lock
git add -A
git commit -m "manual push 2026-06-25"
git push origin main
```
