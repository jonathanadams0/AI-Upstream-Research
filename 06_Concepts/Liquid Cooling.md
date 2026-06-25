---
tags: [concept]
last_updated: 2026-06-03
---

# Liquid Cooling

Liquid cooling is the use of water, glycol mixtures, or dielectric fluids to remove heat from data center computing equipment, as opposed to conventional air cooling using fans and computer room air conditioning (CRAC) units.

**Why it matters:** Air cooling becomes physically inadequate above ~40 kW per rack. AI GPU racks (Nvidia GB200 NVL72) dissipate 120 kW per rack. Liquid cooling is mandatory for frontier AI infrastructure — not a preference.

**Key technologies:**
- **Direct Liquid Cooling (DLC):** Cold plates attached to CPUs/GPUs carry coolant directly; most efficient for AI
- **Rear-door heat exchangers:** Retrofit solution for existing air-cooled facilities
- **Full immersion:** Server submerged in dielectric fluid; highest density, early commercial stage

**The standard threshold:** ASHRAE TC 9.9 defines A3 class at 40 kW/rack as the limit for air cooling. All AI GPU racks exceed this threshold.

**Portfolio link:** [[VRT]] (full-stack DLC leader), [[MOD]] (growing AI thermal), [[TT]] (facility chillers), [[NVT]] (thermal management). See [[Cooling-Thermal]] primer.
