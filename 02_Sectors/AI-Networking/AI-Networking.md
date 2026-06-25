---
sector: AI-Networking
last_updated: 2026-06-03
tags: [sector]
---

# AI Networking — Sector Primer

> A 100,000-GPU training cluster is useless if the GPUs can't communicate. AI-scale networking — moving terabytes per second between thousands of compute nodes with microsecond latency — is a distinct engineering challenge from conventional data center networking, and the companies solving it (Broadcom, Arista, Marvell, Coherent, Credo) are capturing billions in new revenue.

---

## 1. Industry Overview

AI networking encompasses four distinct layers:

1. **GPU-to-GPU interconnect** — Within a node (NVLink from Nvidia) and between nodes (InfiniBand via Nvidia/Mellanox, or AI Ethernet via Broadcom/Arista). For training, all-to-all communication between GPUs must be low-latency and high-bandwidth; a single slow link degrades the entire cluster.

2. **Network switching** — The switching fabric that routes traffic between compute nodes, storage, and front-end servers. Arista dominates AI data center Ethernet switching; Nvidia's Spectrum series and Broadcom's Tomahawk/Trident ASICs also compete.

3. **Custom AI Silicon** — Broadcom and Marvell design custom ASICs for hyperscalers that want to reduce Nvidia dependency: Google TPU (Broadcom), Meta MTIA (Broadcom), Apple Neural Engine (Broadcom), Amazon Trainium/Inferentia (Marvell), Microsoft Maia (Marvell). These are the "second source" to Nvidia and AMD.

4. **Optical interconnect** — At the scale of modern AI clusters, electrical connections are too slow and too lossy beyond ~3 meters. Optical transceivers (Coherent) and active electrical cables (Credo) solve the "last meter" connection between switches and servers.

---

## 2. AI/Networking Linkage

- **Bandwidth explosion:** Nvidia's NVL72 rack has 1.8 TB/s of aggregate NVLink bandwidth internally and 3.6 Tb/s of external network bandwidth. Cluster-level: a 100K GPU cluster needs 100K+ network ports running at 400G-800G.
- **Latency sensitivity:** Large-scale model training uses all-reduce communication — every GPU must exchange gradient updates with every other GPU after each batch. A 1ms latency increase across 100K GPUs can reduce utilization by 10-20%.
- **AI Ethernet vs. InfiniBand:** Hyperscalers are moving to AI Ethernet (standard TCP/IP with RDMA extensions) to avoid Nvidia's proprietary InfiniBand ecosystem. This benefits Arista (Ethernet switches) and Broadcom (Ethernet ASICs) over Nvidia (InfiniBand).
- **Custom silicon demand:** Google's TPU v5 costs ~70% less per FLOP than Nvidia H100 for inference. Amazon, Microsoft, Meta are all investing in custom silicon to reduce Nvidia dependency and lower total infrastructure cost. Broadcom and Marvell are the primary custom chip designers.
- **Optical transceiver bottleneck:** 800G optical transceivers for AI clusters sold out in 2024-2025. Coherent's recent 17.6% single-day surge on Computex AI announcements reflects the market recognizing optical interconnect as a genuine bottleneck.

---

## 3. Value Chain

```
Custom ASIC design (Broadcom, Marvell)
        ↓
Chip fabrication (TSMC N3/N2)
        ↓
Network switch ASICs (Broadcom Tomahawk)  →  Switch platforms (Arista)  →  Data center fabric
        ↓
Optical transceiver (Coherent COHR)  →  Pluggable into switch/server
        ↓
Active electrical cables (Credo CRDO)  →  Within-rack GPU-to-switch connections
```

---

## 4. Competitive Landscape

| Company | Ticker | Sub-segment | Market Position |
|---|---|---|---|
| Broadcom | AVGO | Custom AI ASICs + networking chips | #1 custom AI chip designer; >$25B AI revenue run-rate est. |
| Marvell Technology | MRVL | Custom AI ASICs + PAM4 DSPs | Amazon/Microsoft custom chips; PAM4 for 100G+ optics |
| Arista Networks | ANET | Ethernet data center switching | #1 in AI data center Ethernet; raised FY revenue guide to $11.5B |
| Coherent Corp | COHR | Optical transceivers + laser components | 800G/1.6T transceivers for AI clusters; record revenue |
| Credo Technology | CRDO | Active electrical cables (AEC) | Short-reach GPU interconnect; revenue +206% YoY |
| Nvidia | NVDA (not in coverage) | NVLink + InfiniBand | Proprietary AI interconnect; competition from Ethernet camp |
| Juniper/HPE | — | Networking (secondary) | Lower exposure to AI-specific networking |

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Source |
|---|---|---|
| Broadcom AI revenue segment | Direct measure of custom silicon + networking AI exposure | AVGO quarterly earnings |
| Marvell custom silicon revenue | Progress on Trainium/Maia ramp | MRVL quarterly earnings |
| Arista data center port shipments + revenue | AI Ethernet adoption pace | ANET quarterly earnings |
| Coherent 800G/1.6T transceiver revenue | Bandwidth upgrade cycle | COHR quarterly earnings |
| Credo AEC revenue | Short-reach AI interconnect adoption | CRDO quarterly earnings |
| Hyperscaler AI capital expenditure | Primary demand driver for all names | MSFT/AMZN/GOOGL/META quarterly |
| AI Ethernet vs. InfiniBand market share | Ecosystem battle; matters for ANET vs. NVDA |  Industry analysts |

---

## 6. Valuation Context

| Company | Forward P/E | Revenue Growth | Notes |
|---|---|---|---|
| AVGO | ~35-40x | ~20-25% | Premium for custom silicon + recurring semiconductor revenue |
| MRVL | ~40-50x | ~40-60% | High growth; custom silicon ramp still early |
| ANET | ~35-40x | ~20-25% | Pulled back 22% from ATH; consensus PT $186; Buy case |
| COHR | ~25-35x | ~30-40% | Record high; optical transceiver bottleneck narrative |
| CRDO | ~70-100x | ~200%+ | Extraordinary growth; premium valuation |

---

## 7. Key Themes

**Custom silicon vs. Nvidia:** Every dollar a hyperscaler spends on Broadcom or Marvell custom silicon is a dollar not spent on Nvidia GPUs. The total addressable market for custom silicon is enormous — Google, Amazon, Microsoft, and Meta collectively have ~$300B+ annual capex. Even modest custom silicon penetration represents tens of billions in silicon demand.

**AI Ethernet consolidation:** The shift from proprietary InfiniBand to standard Ethernet for AI cluster networking is the single largest shift in data center networking architecture in a decade. Arista is the primary beneficiary.

**Transceiver speed race:** 400G → 800G → 1.6T → 3.2T. Each speed doubling tightens the transceiver supply chain (Coherent, Lumentum, II-VI). Coherent is the largest player.

---

## 8. Risks

1. **Nvidia InfiniBand defense:** If Nvidia successfully defends InfiniBand adoption in hyperscale AI, Arista's AI Ethernet opportunity narrows
2. **Custom silicon execution risk:** Hyperscaler custom chips are often 1-2 generations behind Nvidia on capability; if Blackwell/Rubin advantage widens, custom silicon adoption could slow
3. **Transceiver commoditization:** Chinese manufacturers (Innolight, HG Genuine, Accelink) are aggressively competing in optical transceivers — could pressure Coherent margins
4. **Capex normalization:** Any slowdown in hyperscaler AI capex flows directly into AI networking demand

---

## 9. Data Sources

- Broadcom, Marvell, Arista, Coherent, Credo quarterly earnings
- Dell'Oro Group — data center networking market reports
- LightCounting — optical transceiver market research
- Bigdata.com — earnings transcripts, analyst reports
