---
tags: [concept]
---

# HBM — High Bandwidth Memory

**Category:** Semiconductor / Memory

---

## What It Is

Stacked DRAM connected to a logic die (GPU/accelerator) via through-silicon vias (TSVs) and an interposer, providing dramatically higher bandwidth than standard DDR memory. HBM3 / HBM3e are the current generations shipping in AI accelerators (NVIDIA H100/H200/B100/B200, AMD MI300, Google TPU, AWS Trainium).

---

## Why It Matters for AI

AI training/inference is memory-bandwidth bound, not compute-bound, for many workloads. HBM capacity per accelerator and HBM stack count have grown every generation. HBM represents a growing share of the bill of materials and is the key bottleneck for GPU supply.

---

## Supply Chain

- **Producers:** SK Hynix (leader), Samsung, Micron (ramping)
- **Packaging:** TSMC via [[CoWoS]]
- **Equipment beneficiaries:** [[AMAT]], [[LRCX]], bonding tools

---

## Related Notes

- [[CoWoS]]
- [[Advanced Packaging Bottleneck]]
- [[AMAT]], [[LRCX]]
