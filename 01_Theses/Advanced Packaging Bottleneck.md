---
status: Archived
conviction: Medium
last_updated: 2026-06-23
tags: [thesis]
---

# Advanced Packaging Bottleneck

> Advanced packaging — specifically TSMC's CoWoS technology — is the binding constraint on AI GPU supply. Every Nvidia GPU requires CoWoS to bond the compute die to HBM stacks. TSMC's CoWoS capacity expansion is directly correlated with AI GPU volumes, and the equipment companies serving this expansion (LRCX, AMAT, KLAC) earn revenue on every expansion wafer.

---

## The Core Thesis

In 2023-2024, the Nvidia H100 supply constraint was not about TSMC's N4 process node — it was about CoWoS packaging capacity. The compute dies were being manufactured; there wasn't enough packaging capacity to bond them with HBM and ship complete GPUs.

This bottleneck was poorly understood by many investors who focused on front-end wafer starts (lithography, etch, deposition in the logic fab) while overlooking the back-end packaging step that determines final chip availability. The semi equipment companies that serve CoWoS (especially LRCX for TSV etch and KLAC for packaging inspection) saw order acceleration that was directly tied to AI GPU demand rather than traditional WFE cycle drivers.

The thesis: Advanced packaging capacity is structurally undersupplied relative to AI GPU demand growth, and the expansion investment flows directly through equipment suppliers.

---

## What Makes CoWoS Different from Conventional Packaging

Conventional chip packaging (BGA, flip-chip) is a commodity process done by OSAT (outsourced semiconductor assembly and test) companies like ASE Group, Amkor, and JCET. It uses relatively simple wire bonding or flip-chip bumping.

CoWoS is fundamentally different:
- **Silicon interposer:** An entire additional wafer is processed (lithography, etch, metallization, CMP) to serve as the connection layer between compute die and HBM
- **High-density interconnects:** Micro-bumps with <50μm pitch (vs. ~250μm for conventional flip-chip)
- **Through-silicon vias (TSVs):** Deep holes etched and filled in the HBM die to enable vertical stacking
- **Large die sizes:** GB200 GPU die is ~814 mm² — one of the largest dies ever; requires precision alignment and bonding

This complexity means CoWoS can only be done by leading foundries with the necessary front-end-like process capabilities. TSMC dominates CoWoS; Samsung and Intel Foundry are developing competing technologies.

---

## Equipment Content per CoWoS Wafer

Each CoWoS interposer wafer requires the following key equipment steps:

| Process Step | Equipment | Primary Supplier |
|---|---|---|
| Interposer layer patterning | DUV immersion lithography | ASML |
| Via etching (interposer) | Plasma etch | LRCX |
| Metal deposition (Cu fill) | CVD / PVD | AMAT, LRCX |
| CMP (planarization) | CMP | AMAT |
| TSV etch (HBM die) | Deep silicon etch | LRCX |
| TSV fill | ECD copper | LRCX, AMAT |
| Wafer bonding alignment | Wafer bonders | BE Semiconductor (BESI), EV Group |
| Post-bond inspection | Optical + electron beam | KLAC |
| Bump inspection | Optical metrology | KLAC |

**LRCX's position is particularly strong:** TSV etch is deep silicon etch — a capability where Lam has both the installed base advantage and process recipe lock-in. KLAC's advanced packaging revenue growing from $635M to ~$1B in 2026 confirms inspection intensity is rising.

---

## CoWoS vs. Competing Technologies

| Technology | Developer | Key Feature | Status |
|---|---|---|---|
| **CoWoS-S** | TSMC | Silicon interposer | Current standard for Nvidia GPUs |
| **CoWoS-L** | TSMC | Larger format; more HBM stacks | GB200 NVL72 uses CoWoS-L |
| **SoIC** | TSMC | 3D face-to-face bonding, no interposer | Used for chiplets within compute die; complementary |
| **FOVEROS** | Intel | 3D chip stacking | Used in Intel's own products; not competitive for Nvidia |
| **X-Cube / HBM-in-Package** | Samsung | Samsung's CoWoS equivalent | Used for AMD MI300X |
| **COWOS-on-silicon** | TSMC (future) | Higher density version | Roadmap item |

TSMC's CoWoS is the industry standard for the highest-volume AI GPU programs (Nvidia). Samsung's equivalent serves AMD. Each expansion serves different customers but all drive the same equipment suppliers.

---

## Capacity Timeline and Investment

| Year | Estimated CoWoS wspm | Key Driver |
|---|---|---|
| 2023 | ~5,000 | H100 supply bottleneck visible |
| 2024 | ~12,000 | TSMC rapid expansion; still constrained |
| 2025 | ~25,000 | Continued expansion; H200/B200 ramp |
| 2026E | ~35,000-40,000 | GB200/Rubin preparation; still below demand |
| 2027E | ~50,000+ | TSMC CoWoS-L facilities; industry capacity |

TSMC has guided CoWoS as a multi-billion dollar capital priority. Each wspm expansion requires equipment orders that flow to LRCX, AMAT, KLAC, and ASML.

---

## Investment Implications

| Company | Advanced Packaging Angle | KPI to Watch |
|---|---|---|
| [[LRCX]] | TSV etch dominant supplier; SAM growing as packaging complexity increases | Packaging revenue as % of total; HBM + CoWoS commentary on earnings calls |
| [[KLAC]] | Advanced packaging inspection #1 position; $635M→$1B 2025→2026 | Disclosed packaging revenue tracking |
| [[AMAT]] | CMP, deposition tools for CoWoS interposer; advanced packaging portfolio | Packaging segment commentary |
| [[ASML]] | DUV immersion lithography for interposer patterning | Less direct but serves every CoWoS interposer wafer |
| [[TOELY]] | Coater/developer tools used in interposer patterning | Korean/Japanese customers leading CoWoS adoption |

---

## Key Data Points from Coverage Research

- **LRCX Q3 FY2026:** CEO Tim Archer confirmed Lam's SAM growing from low-30s% to high-30s% of WFE, partly due to advanced packaging (CoWoS, SOIC, HBM packaging)
- **KLAC Q3 FY2026:** Disclosed $1B advanced packaging revenue target for 2026 (up from $635M), achieved #1 position in Process Control for Advanced Wafer-Level Packaging
- **LRCX June 2026 conference:** "We see meaningful revenue increases across some of our more advanced systems as we look at 2026... in terms of CoWoS packaging, but also emerging SOIC packaging as die stack is happening, driving hybrid bonding requirements"

---

## Risks

1. **TSMC CoWoS capacity acceleration surpasses demand:** If TSMC expands faster than AI GPU demand grows, utilization falls and equipment orders slow
2. **Alternative packaging technologies:** SoIC or 3D stacking approaches reduce the interposer-intensive CoWoS step; 5-10 year horizon
3. **Nvidia GPU demand cyclicality:** Any digestion period in AI capex reduces CoWoS demand directly
4. **Samsung/Intel CoWoS competition:** New suppliers (Samsung's CoWoS equivalent, Intel Foundry) could fragment the market

---

## Related Concepts

- [[CoWoS]] — full technical explanation of the packaging process
- [[HBM]] — the memory being integrated via advanced packaging
- [[HBM Supply Constraint]] — companion thesis on memory supply

---

## Archive Note (2026-06-23)

**Thesis played out successfully.** TSMC CoWoS capacity expanded from ~5,000 wspm (2023) to ~35-40,000 wspm (2026E) — the bottleneck that originally defined this thesis has largely resolved. The emergency expansion phase that drove premium equipment orders at LRCX, AMAT, and KLAC is transitioning to a steady-state growth phase.

Ongoing advanced packaging demand growth is now captured within the [[WFE Supercycle]] thesis, which treats CoWoS, SoIC, and hybrid bonding as one of four simultaneous WFE demand vectors. No separate bottleneck premium warranted at current capacity levels.

**Do not resurface unless:** TSMC CoWoS utilization returns above ~95% AND GPU supply is again explicitly gated by packaging, not logic or HBM.

See [[Thesis_Stress_Test_2026-06-23]] for full analysis.

---

## Change Log

- `2026-06-03` — Thesis created. Evidence base: LRCX Q3 FY2026 earnings + June 2026 conferences, KLAC Q3 FY2026 earnings, industry reports.
- `2026-06-23` — **Archived.** Bottleneck resolved by TSMC capacity expansion. Ongoing demand folded into [[WFE Supercycle]].
