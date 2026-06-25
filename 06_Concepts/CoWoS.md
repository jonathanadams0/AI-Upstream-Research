---
tags: [concept]
last_updated: 2026-06-03
---

# CoWoS — Chip-on-Wafer-on-Substrate

## What It Is

CoWoS (Chip-on-Wafer-on-Substrate) is TSMC's advanced packaging technology that horizontally integrates multiple chiplets — including compute dies and High Bandwidth Memory stacks — onto a shared silicon interposer, which is then mounted on a substrate. It is the manufacturing process that connects Nvidia's GPU dies to HBM memory stacks in every H100, H200, and B200 GPU.

Without CoWoS, the AI accelerator supply chain does not function. Every frontier AI GPU requires CoWoS or an equivalent advanced packaging step.

## Why It Matters for the Portfolio

**CoWoS capacity = AI GPU supply.** In 2023-2024, CoWoS capacity at TSMC was the primary bottleneck constraining Nvidia H100 supply — not TSMC's N4 wafer starts. The GPU dies existed; the packaging capacity to bind them with HBM did not.

TSMC has been aggressively expanding CoWoS capacity since 2023. Each CoWoS expansion announcement is directly correlated with higher-volume AI GPU delivery, higher Nvidia revenue, and higher equipment orders for TSMC's CoWoS line (which uses etch, deposition, and inspection tools from [[LRCX]], [[AMAT]], and [[KLAC]]).

## How It Works (Simplified)

```
Step 1: GPU die manufactured on N4/N3 process node (TSMC)
Step 2: HBM stacks manufactured at SK Hynix / Samsung / Micron
Step 3: CoWoS interposer — silicon wafer with micro-bumps
Step 4: GPU die + HBM stacks flip-chip bonded onto interposer
Step 5: Interposer mounted on organic substrate
Step 6: Final package: GPU + HBM + interposer + substrate
```

The interposer acts as a high-bandwidth connection between GPU and HBM — enabling the terabytes-per-second bandwidth that AI training requires. Without the interposer, GPU and HBM would communicate through a slower, conventional package connection.

## CoWoS Capacity Bottleneck

CoWoS capacity is measured in wafer starts per month (wspm) at the interposer level. Each CoWoS wafer produces a limited number of interposers (depending on die size). Large dies (B200 is ~814 mm² — one of the largest ever) produce fewer interposers per wafer, making large AI GPUs especially capacity-constrained.

TSMC expanded CoWoS capacity from ~5,000 wspm in early 2023 to an estimated 30,000+ wspm by end of 2025, with continued expansion planned through 2027. Even so, demand outpaces supply for the highest-density configurations.

## Equipment Implications

Every CoWoS interposer wafer requires:
- **Lithography:** DUV immersion (ASML) — interposer patterning
- **Etch:** Plasma etch for through-silicon vias (TSVs) ([[LRCX]] dominates TSV etch)
- **Deposition:** CVD/PVD for metal fill in TSVs ([[AMAT]], [[LRCX]])
- **Metrology:** Inspection of bump planarity, TSV depth, alignment ([[KLAC]])

This is why LRCX explicitly called CoWoS a top growing market and why KLAC disclosed advanced packaging revenue growing from $635M in 2025 to ~$1B in 2026.

## Evolution: CoWoS → SoIC → 3D Integration

TSMC's packaging roadmap extends beyond CoWoS:
- **CoWoS-S:** Silicon interposer (current standard for AI GPUs)
- **CoWoS-L:** Larger format interposer for even bigger die configurations
- **SoIC (System-on-Integrated-Chips):** 3D face-to-face stacking without an interposer; higher density but smaller scale currently
- **N2 node + next-gen packaging:** Each new process node requires updated CoWoS integration

## Key Data Points

- Nvidia H100: 80GB HBM3 + 4 HBM stacks integrated via CoWoS
- Nvidia B200: 192GB HBM3E + more stacks, larger interposer
- TSMC CoWoS wspm: ~5K (2023) → ~30K+ (2025E) → continuing expansion
- KLAC advanced packaging revenue: $635M (2025) → ~$1B (2026E)
- LRCX: "We own the TSV. We do most of the TSV for everybody in the industry." (June 2026 conference)

## Related Concepts

- [[HBM]] — the memory being integrated via CoWoS
- [[SMR]] — unrelated technology (nuclear reactors)

## Related Coverage

- [[LRCX]] — dominant TSV etch and deposition supplier for CoWoS
- [[KLAC]] — advanced packaging process control leader
- [[AMAT]] — CVD/PVD deposition for CoWoS interposer
- [[ASML]] — DUV immersion lithography for interposer patterning
- [[TOELY]] — coater/developer and etch tools used in packaging
