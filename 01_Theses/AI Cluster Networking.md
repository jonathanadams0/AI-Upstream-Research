---
status: Active
conviction: Medium
last_updated: 2026-06-23
tags: [thesis]
split_from: "AI Networking and Custom Silicon"
---

# AI Cluster Networking

> AI clusters at the 100,000-GPU scale require networking infrastructure that simply did not exist before 2023: 800G Ethernet switching (Arista), optical transceivers (Coherent), and active electrical cables (Credo). These are genuine new markets. Growth rate moderates under AI capex deceleration, but existing installed base and the 800G → 1.6T bandwidth upgrade cycle provide durable floor demand.

---

## The Core Thesis

A 100,000-GPU cluster is a fundamentally different networking problem than a conventional data center:
- **All-to-all communication** during training (all-reduce ops) requires every GPU to reach every other GPU simultaneously
- **Scale of switching:** 100,000 GPUs require ~10,000+ 32-port 800G switches in a fat-tree topology
- **Latency sensitivity:** 1ms synchronization lag across a cluster can waste 10%+ of compute time
- **Aggregate bandwidth:** 100,000 GPUs × 800G = 80 Petabits/second — a new class of infrastructure problem

This created entirely new markets that the traditional networking industry was not equipped to serve at the required scale or economics.

---

## AI Ethernet vs. InfiniBand

| Factor | AI Ethernet (Arista/Broadcom) | InfiniBand (Nvidia/Mellanox) |
|---|---|---|
| Ecosystem | Open; commodity economics | Proprietary; Nvidia controls |
| Cost | Lower — standard switching economics | Premium pricing |
| Vendor dependency | Reduces Nvidia dependency | Increases Nvidia dependency |
| Hyperscaler preference | Dominant for large-scale AI clusters | Legacy HPC environments |

Hyperscalers choosing AI Ethernet choose Arista over Nvidia Spectrum — this is a genuine market share shift, not just market growth.

---

## Investment Implications

| Company | Angle | Rating | Notes |
|---|---|---|---|
| [[ANET]] | Dominant 800G AI Ethernet switching; 22% below ATH as of June 23 | Buy | Consensus PT ~$186; current price near that level |
| [[COHR]] | 800G/1.6T optical transceivers; structural bottleneck in transceiver supply | Hold | Record highs post-Computex; real bottleneck but valuation extended |
| [[CRDO]] | Active electrical cables (AEC) for rack-level GPU connectivity | Hold | Revenue +206% YoY but purely tied to new cluster buildout pace |

---

## Why Conviction Is Medium (Not High)

Under AI capex deceleration (20-25% YoY growth vs. prior 75%):
- New cluster additions slow proportionally → new switch and transceiver demand grows more slowly
- CRDO is most exposed — it has no installed base repeat revenue; everything is new-build
- COHR and ANET have more durability via installed base upgrades and the bandwidth upgrade cycle (800G → 1.6T), but the peak-growth narrative is diminished

The thesis isn't broken — AI Ethernet switching and optical transceivers are still genuinely new, growing markets. But the *pace* of that growth moderates, and with it the multiple justified for these stocks.

---

## The Durable Floor

Even under capex deceleration, demand floors exist:
- **Bandwidth upgrade cycle:** Existing 400G clusters upgrade to 800G, then 1.6T — this is driven by per-cluster efficiency economics, not just new builds, and happens on a 2-3 year cycle
- **Installed base management:** ANET in particular has maintenance, software, and services revenue tied to the existing installed base
- **AI inference scaling:** Even if training cluster additions slow, inference infrastructure (which requires lower-bandwidth but high-throughput networking) continues to expand

---

## Risks

1. **Capex deceleration directly reduces new cluster builds** — the primary demand driver
2. **Nvidia AI Ethernet offensive:** Nvidia developing competitive Ethernet switching would threaten Arista's position
3. **Chinese transceiver competition:** Aggressive price competition in optical from Chinese vendors (COHR most exposed)
4. **Credo single-market risk:** CRDO has limited diversification; a pause in GPU cluster buildout hits revenue immediately

---

## Key Signal to Watch

Hyperscaler Q2 2026 capex actuals (late July earnings from MSFT, GOOG, AMZN, META). New cluster guidance drives the demand read-through directly to Arista switch orders, Coherent transceiver pull-through, and Credo AEC volumes.

---

## Change Log

- `2026-06-23` — Split from [[AI Networking and Custom Silicon]] following stress-test analysis. Conviction set at Medium (down from High) reflecting pace-of-growth deceleration under AI capex scenario. Custom silicon sub-thesis moved to [[Custom Silicon]] at High conviction. See [[Thesis_Stress_Test_2026-06-23]].
