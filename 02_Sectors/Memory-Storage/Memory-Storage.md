---
sector: Memory-Storage
last_updated: 2026-06-03
tags: [sector]
---

# Memory & Storage — Sector Primer

> Every AI model starts and ends as data. DRAM holds the computation in-flight; NAND stores the training datasets and model weights; HDDs archive the petabytes of cold data AI pipelines consume. Memory and storage are not adjacent to AI — they are the substrate it runs on.

---

## 1. Industry Overview

Memory and storage sit one layer beneath the compute chip but are often the binding constraint on AI system performance. The GPU is only as fast as its memory bandwidth; the inference cluster is only as efficient as its storage I/O. Three distinct segments make up this sector:

1. **DRAM / HBM** — Volatile, high-speed memory. Conventional DRAM (DDR5, LPDDR5) fills server memory; High Bandwidth Memory (HBM) is stacked on-package directly adjacent to AI GPUs for maximum bandwidth. Every AI accelerator from Nvidia, AMD, and Google TPU requires HBM.

2. **NAND Flash / SSDs** — Non-volatile, persistent storage. AI training datasets are stored on NAND SSDs in the hot tier. AI inference clusters need low-latency NAND for model weight loading and KV cache storage. NAND capacity requirements grow with each new model generation (larger models, longer context windows, more training data).

3. **Hard Disk Drives (HDD)** — Magnetic spinning media. Vastly cheaper per TB than NAND, making HDDs indispensable for the cold tier of AI data lakes — storing the raw training corpus, model checkpoints, and long-term archives. Seagate's HAMR (Heat-Assisted Magnetic Recording) drives offer 30-50+ TB per platter, reshaping cost economics.

---

## 2. AI/Memory Linkage

- **HBM is mandatory for frontier AI:** GB200 NVL72 contains 192GB HBM3E per GPU. Each new GPU generation requires more HBM at higher bandwidth. No HBM = no frontier AI GPU.
- **NAND for inference at scale:** A single LLM inference response may require gigabytes of KV cache retrieval from NVMe SSDs. At millions of requests per day, storage I/O becomes a system bottleneck.
- **Cold storage explosion:** AI training datasets now commonly exceed petabytes. OpenAI's GPT-4 training run consumed an estimated 13 trillion tokens. At 2 bytes/token, that's 26TB — compressed. The full uncompressed corpus is orders of magnitude larger. HDDs are the only practical medium at this scale.
- **NAND price cycle:** AI demand has introduced a demand floor that didn't exist before. NAND prices surged 5-10x from their 2023 trough through 2026. Memory OEMs are no longer purely at the mercy of consumer electronics cycles.

---

## 3. Value Chain

```
Silicon wafers → DRAM/NAND wafer processing (SK Hynix, Samsung, Micron) → HBM stacking (TSV)
      ↓                                                                          ↓
  NAND die → SSD controller + packaging → Enterprise SSD                   HBM package → CoWoS → GPU
      ↓
  HDD component manufacturing (Seagate, WDC)
```

**Equipment suppliers feeding this sector:** [[LRCX]] (DRAM/NAND etch + HBM TSV), [[AMAT]] (deposition), [[KLAC]] (inspection). See [[Semi-Materials-Equip]] primer.

---

## 4. Competitive Landscape

| Company | Ticker | Sub-segment | AI Angle |
|---|---|---|---|
| Micron Technology | MU | DRAM + NAND + HBM | Only US-based HBM producer; HBM3E for Nvidia |
| Sandisk | SNDK | NAND flash (spun from WDC Feb 2025) | AI inference/training NAND leader |
| Western Digital | WDC | HDD (post-Sandisk) | AI cold storage; HAMR ramp |
| Seagate Technology | STX | HDD | AI cold storage; HAMR; 5x stock in 1 year |
| SK Hynix | 000660.KS | DRAM + HBM (not in coverage) | HBM3E market leader; primary Nvidia HBM supplier |
| Samsung | SSNLF | DRAM + NAND + HBM (not in coverage) | HBM3E qualification delays; catching up |

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Source |
|---|---|---|
| HBM revenue as % of DRAM (Micron) | Margin and premium-segment mix | Micron quarterly earnings |
| NAND pricing (contract + spot) | Input to SNDK/WDC/Samsung margins | TrendForce weekly |
| HDD exabytes shipped (Seagate, WDC) | Volume vs. pricing mix | Quarterly earnings |
| HAMR qualification progress (Seagate) | Next-gen capacity unlock | STX earnings calls |
| SK Hynix HBM4 qualification | Competitive dynamics with Micron | Industry news |
| Hyperscaler NAND/HDD procurement commentary | Demand signal | AWS, MSFT, GOOGL earnings |

---

## 6. Valuation Context

| Company | Forward P/E | Revenue Growth | AI-Specific Driver | Notes |
|---|---|---|---|---|
| MU | ~30-40x | ~50%+ | HBM3E premium pricing | Cyclical, but AI adds secular floor |
| SNDK | High (new co.) | Strong NAND recovery | AI inference NAND | Spinoff; limited comp history |
| WDC | ~20-25x | Moderate | AI cold storage | Post-spinoff; HDD-only |
| STX | ~20-25x | High | AI cold storage + HAMR | 500% YoY move |

---

## 7. Key Theses

- [[HBM Supply Constraint]] — HBM cannot be manufactured fast enough; Micron is the US alternative to SK Hynix/Samsung
- [[Advanced Packaging Bottleneck]] — HBM TSV processing is the constraint within the constraint

---

## 8. Risks

1. **Memory cyclicality** — even with AI demand floor, OEMs can overbuild; 2023's severe downturn happened despite AI being hyped
2. **China export controls** — US memory export restrictions could limit Micron's China sales (happened in 2023)
3. **SK Hynix/Samsung cost advantages** — Korean OEMs benefit from government support and scale
4. **HDD secular decline** — NAND continues to penetrate cold storage tiers; HAMR must execute to maintain HDD relevance
5. **Technology transitions** — HBM4, 3D DRAM, and CXL memory architectures create execution risk

---

## 9. Data Sources

- TrendForce — NAND and DRAM pricing, HBM shipment data
- Micron, Seagate, WDC quarterly earnings
- JEDEC standards for HBM generations
- Bigdata.com — earnings transcripts, analyst reports
