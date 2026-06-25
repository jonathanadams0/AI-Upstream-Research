---
status: Archived
conviction: High
last_updated: 2026-06-23
tags: [thesis]
---

> **⚠ ARCHIVED 2026-06-23** — Split into two separate theses with differentiated conviction levels:
> - [[Custom Silicon]] — High conviction (counter-cyclical to capex anxiety; AVGO, MRVL)
> - [[AI Cluster Networking]] — Medium conviction (growth moderates with capex decel; ANET, COHR, CRDO)
>
> Original content preserved below for reference. See [[Thesis_Stress_Test_2026-06-23]].

---

# AI Networking and Custom Silicon

> The hyperscalers are building a parallel AI silicon ecosystem to reduce Nvidia dependency — and Broadcom and Marvell are the pick-and-shovel suppliers of this ecosystem. Simultaneously, AI clusters at the 100,000-GPU scale require networking infrastructure that simply did not exist before 2023: 800G Ethernet switching (Arista), optical transceivers (Coherent), and active electrical cables (Credo). These are genuine new markets, not just share gains.

---

## The Core Thesis

**Part 1: Custom AI Silicon**

Nvidia's AI accelerator monopoly is profitable for Nvidia but expensive for hyperscalers. The H100 carries a list price of ~$25,000-40,000. At 100,000 GPUs, that's $2.5-4B in Nvidia hardware alone — before networking, power, cooling, or real estate. Each hyperscaler is now investing billions to develop custom AI ASICs that offer comparable AI performance at 40-70% lower cost for their specific workloads:

- **Google TPU v5** (designed with Broadcom): Handles Google's vast inference workload; enables Google to offer Gemini inference cheaper than Nvidia-based competitors
- **Amazon Trainium 2** (designed with Marvell): AWS's proprietary AI training chip; reduces cost for Amazon's own internal AI and for AWS customers who choose Trainium instances
- **Microsoft Maia** (designed with Marvell): Microsoft's internal AI chip for Azure; enables Azure to offer AI inference at competitive economics
- **Meta MTIA** (designed with Broadcom): Meta's internal inference chip for recommendations, ranking, and generative AI

Each of these programs represents billions in annual silicon procurement from Broadcom and Marvell — revenue that did not exist 3 years ago.

**Part 2: AI Cluster Networking**

A 100,000-GPU cluster is a fundamentally different networking challenge than a conventional data center:
- **All-to-all communication:** Training requires every GPU to communicate with every other GPU (all-reduce operations). 100,000 GPUs × 800G bandwidth per GPU = 80 Petabits per second of aggregate cluster bandwidth
- **Latency sensitivity:** Synchronization overhead means latency compounds — a 1ms lag across all GPUs in a training step can waste 10%+ of compute time
- **Scale of switching:** 100,000 GPUs require ~10,000+ 32-port 800G switches, connected in a fat-tree topology

Arista Networks is the dominant supplier of the 800G Ethernet switches for AI clusters. Every hyperscaler choosing AI Ethernet over InfiniBand is choosing Arista switches.

Coherent makes the 800G optical transceivers that plug into those switches. Credo makes the active electrical cables that connect GPUs to switches within a rack (1-3 meter distances where optical is overkill).

---

## Why "AI Ethernet" Is Winning Over InfiniBand

| Factor | AI Ethernet (Arista/Broadcom) | InfiniBand (Nvidia/Mellanox) |
|---|---|---|
| Ecosystem | Open; any vendor can participate | Proprietary; Nvidia controls |
| Cost | Commodity switching economics | Premium InfiniBand pricing |
| Management | Standard network tools | Proprietary OFED stack |
| Scalability | Proven at cloud scale | Proven at HPC scale |
| Vendor dependency | Reduces Nvidia dependency | Increases Nvidia dependency |

Hyperscalers choosing AI Ethernet is choosing Arista over Nvidia Spectrum switches — a meaningful market share shift.

---

## Investment Implications

| Company | Exposure | Rating | Notes |
|---|---|---|---|
| [[AVGO]] | Custom silicon (Google, Meta, Apple) + networking ASICs | Buy/$560 | $25B+ AI revenue; premium justified |
| [[MRVL]] | Custom silicon (Amazon, Microsoft) + PAM4 DSPs | Buy/$370 | Early innings of custom silicon ramp |
| [[ANET]] | AI Ethernet switching | Buy/$185 | 22% below ATH; consensus PT $186 |
| [[COHR]] | 800G/1.6T optical transceivers | Hold/$420 | Record high post-Computex; real bottleneck |
| [[CRDO]] | Active electrical cables (AEC) | Hold/$250 | Revenue +206% YoY; premium valuation |

---

## Duration

Custom silicon programs are 3-5 year design cycles. Once a hyperscaler has designed Trainium 2 with Marvell, they commit to Marvell for the next 3-5 years. This is sticky, recurring revenue — the opposite of commodity semiconductor cycles. The networking infrastructure (switches, transceivers) is replaced as bandwidth standards upgrade (400G → 800G → 1.6T), providing recurring demand every 2-3 years.

---

## Risks

1. **In-house silicon:** If a hyperscaler builds internal chip design capability and reduces dependence on Broadcom/Marvell, custom silicon revenue declines
2. **Nvidia AI Ethernet offensive:** Nvidia could develop competitive Ethernet switching solutions
3. **Chinese competition in optical:** Chinese transceiver manufacturers are aggressive on price
4. **Capex normalization:** AI infrastructure spending slowdown would flow through all networking names

---

## Change Log
- `2026-06-03` — Thesis created. Evidence base: AVGO, MRVL, ANET, COHR, CRDO company filings and web research.
