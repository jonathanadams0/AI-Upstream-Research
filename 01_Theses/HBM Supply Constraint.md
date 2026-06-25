---
status: Active
conviction: High
last_updated: 2026-06-03
tags: [thesis]
---

# HBM Supply Constraint

> High Bandwidth Memory (HBM) — the on-package DRAM stacked atop every AI accelerator — is structurally supply-constrained. Each new HBM generation requires more etch steps per wafer and a higher die stack height, directly expanding the addressable market for Lam Research and Applied Materials regardless of which AI company wins.

---

## The Core Thesis

Every frontier AI GPU contains HBM. The H100 has 80GB HBM3; the B200 has 192GB HBM3E; future Rubin/next-generation chips will have more. HBM is not a commodity DRAM chip — it is a specialized, 3D-stacked memory architecture that requires dozens of additional manufacturing steps compared to conventional DRAM.

The supply constraint is structural, not cyclical:
1. Only three companies manufacture HBM at scale: SK Hynix, Samsung, Micron
2. Each new HBM generation is more complex and more etch-intensive than its predecessor
3. Capacity expansion requires 18-24 months of construction and qualification — the same supply inelasticity problem as copper mines, but in semiconductor form
4. The demand signal from AI accelerators has a 3-5 year visibility horizon — hyperscalers are signing multi-year agreements with DRAM suppliers

---

## HBM Architecture and Why It's Etch-Intensive

HBM works by stacking multiple DRAM dies vertically and connecting them through thousands of tiny holes called through-silicon vias (TSVs). Each TSV is etched, filled with metal, and polished — a process that Lam Research dominates globally.

| Generation | Stack Height | TSV Depth | Bandwidth | Key User |
|---|---|---|---|---|
| HBM2 | 8 layers | ~50μm | 1 TB/s | A100 |
| HBM3 | 12 layers | ~60μm | 3.2 TB/s | H100 |
| HBM3E | 16 layers | ~70μm | 4.8 TB/s | H200, B200 |
| HBM4 (coming) | 16+ layers | deeper | 6+ TB/s | Rubin+ |

Each increase in stack height adds etch steps per wafer. Going from HBM2 to HBM3E roughly doubled the etch intensity per HBM wafer. This is the structural mechanism by which Lam Research's HBM SAM grows with each GPU generation.

---

## Supply Chain Structure

```
DRAM wafer starts (SK Hynix, Samsung, Micron)
        ↓
Etch + deposition (LRCX dominant for DRAM etch; AMAT for deposition)
        ↓
TSV processing (LRCX dominant — "We own the TSV")
        ↓
Die stacking + bumping (3D packaging; LRCX, AMAT tools)
        ↓
Integration via CoWoS (TSMC) — see [[CoWoS]]
        ↓
Final GPU package → Nvidia / AMD / Google TPU
```

**Key insight:** The bottleneck has historically oscillated between DRAM wafer capacity and CoWoS packaging capacity. Both are now being simultaneously expanded. The equipment suppliers (LRCX, AMAT, KLAC) benefit from both expansions.

---

## The AI Demand Signal

AI training workloads are memory-bandwidth-bound, not compute-bound, at large scale. The H100's 80 GB HBM3 is still a binding constraint for training GPT-4 class models — systems must use multiple GPUs connected by NVLink to get sufficient aggregate memory bandwidth.

Each new AI model generation requires:
- More parameters → more total memory needed
- Larger batch sizes → higher memory bandwidth needed
- Longer context windows → more attention computation → more HBM I/O

This creates a virtuous cycle for HBM demand: better GPUs with more HBM enable larger models, which in turn require even more HBM in the next GPU generation.

---

## Capacity Timeline

**2024:** HBM3 supply constrained; Nvidia H100 allocation limited by SK Hynix HBM capacity
**2025:** SK Hynix ramped HBM3E for H200/B200; Samsung and Micron qualified HBM3E; supply tightened again
**2026-2027:** HBM4 qualification at SK Hynix; Samsung and Micron racing to qualify; capacity still below demand
**2028+:** Micron US HBM facility (Idaho) begins volume production; first domestic US HBM capacity at scale

Even with aggressive expansion, HBM capacity is expected to remain below AI demand through 2027 based on current customer bookings and disclosed capital expenditure plans.

---

## Investment Implications

| Company | HBM Angle | Conviction |
|---|---|---|
| [[LRCX]] | Dominant DRAM etch + TSV processing. SAM growing from low-30s% to high-30s% of WFE. CEO: "We own the TSV." | Buy — highest HBM leverage |
| [[AMAT]] | CVD/PVD deposition for DRAM and HBM; packaging deposition tools | Buy — broad portfolio |
| [[KLAC]] | Inspection/metrology for HBM stack alignment, TSV depth, yield optimization | Hold — expensive but process control intensity growing |
| [[TOELY]] | Etch and coater/developer tools; memory-focused equipment | Buy — direct HBM exposure through Korean/Japanese customers |
| [[ASML]] | EUV/DUV for HBM base-layer patterning; less direct than etch/deposition | Hold — less HBM-specific than equipment names |

---

## NAND Connection

The HBM supply constraint thesis has a companion in NAND: AI inference deployments require massive NAND storage (training data, model weights, key-value caches for context). NAND demand from AI has driven:
- NAND prices up 5-10x YTD (as of June 2026, per CFRA analyst note)
- Accelerated conversion to 200+ layer QLC architectures
- LRCX's $40B NAND upgrade spending forecast pulled forward to end of 2027

This means LRCX benefits from both HBM (DRAM etch) and NAND (high-aspect-ratio etch for 200+ layer 3D NAND) — a double exposure to AI-driven memory capex.

---

## Risks

1. **HBM inventory digestion:** If AI GPU shipments slow, HBM inventory could build, reducing near-term equipment orders
2. **Samsung execution:** Samsung has struggled to qualify HBM3E; a breakthrough could rapidly change competitive dynamics
3. **Alternative memory architectures:** Computational memory (processing-in-memory) or photonic interconnects could theoretically reduce HBM intensity — 10+ year horizon
4. **China export controls:** Lam and AMAT have 25-30% China revenue; escalating controls would reduce their total addressable market

---

## Change Log

- `2026-06-03` — Thesis created. Evidence base: LRCX Q3 FY2026 earnings call, LRCX CEO Bernstein conference (May/June 2026), CFRA analyst note, Bigdata.com search results.
