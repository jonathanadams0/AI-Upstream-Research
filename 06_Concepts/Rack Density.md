---
tags: [concept]
last_updated: 2026-06-03
---

# Rack Density

Rack density is the amount of electrical power consumed (and heat produced) per server rack in a data center, measured in kilowatts (kW). It determines what cooling technology is required and sets the physical design parameters for an AI facility.

**Historical density progression:**
| Era | Typical Rack Density | Cooling Method |
|---|---|---|
| Traditional IT (2000s-2010s) | 5-10 kW/rack | Air (CRAC units) |
| Cloud compute (2015-2022) | 10-20 kW/rack | Air (high-efficiency) |
| Early AI (H100 era, 2023) | 30-50 kW/rack | Air + rear-door HEX |
| Current AI (B200/GB200, 2025-26) | 60-120 kW/rack | Direct liquid cooling required |
| Next-gen AI (Rubin+, 2027+) | 120-200+ kW/rack | Advanced liquid/immersion |

**Why it matters for the portfolio:** Every time rack density exceeds the air cooling threshold (~40 kW), it creates new demand for [[Liquid Cooling]] infrastructure. The GB200 NVL72 at 120 kW/rack is the event that made liquid cooling mandatory. Each successive GPU generation pushes density higher, continually expanding [[VRT]] and [[MOD]]'s addressable market.

**The physics:** Power = heat. A 120 kW rack produces 120 kW of heat — equivalent to 41 household clothes dryers running simultaneously in a 7-square-foot footprint.
