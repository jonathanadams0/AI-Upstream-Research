---
tags: [concept]
last_updated: 2026-06-03
---

# PUE — Power Usage Effectiveness

Power Usage Effectiveness (PUE) is the ratio of total data center energy consumption to the energy consumed by its IT equipment alone. A PUE of 1.0 is perfect efficiency; a PUE of 2.0 means the facility uses as much power on cooling and overhead as on compute.

**Formula:** PUE = Total Facility Power / IT Equipment Power

**Typical values:**
| PUE | Interpretation |
|---|---|
| 1.0 | Perfect — impossible in practice |
| 1.1-1.2 | Excellent (Google, Meta hyperscale) |
| 1.2-1.4 | Good (modern AI facilities target this range) |
| 1.5-2.0 | Average for legacy data centers |
| >2.0 | Inefficient (older colocation facilities) |

**AI data center implication:** AI GPU clusters must run at 90%+ utilization 24/7 — any inefficiency in PUE compounds at scale. A 100 MW facility with PUE 1.5 wastes 50 MW on overhead; at PUE 1.2, that waste is only 20 MW. The 30 MW difference at $0.05/kWh = $13M annually. At scale across thousands of MW, PUE optimization is worth billions.

**Portfolio link:** [[VRT]] liquid cooling systems can achieve PUE <1.2; air cooling systems typically achieve 1.3-1.5. Liquid cooling's PUE advantage is one of the structural arguments for its adoption beyond just thermal capacity.
