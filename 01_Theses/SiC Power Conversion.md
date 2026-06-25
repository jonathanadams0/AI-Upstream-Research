---
status: Active
conviction: Medium-High
last_updated: 2026-06-23
tags: [thesis]
---

# SiC Power Conversion — The Efficiency Imperative

> At 120 kW per AI rack, a 1% improvement in power conversion efficiency saves 1.2 MW per 10,000-rack data center — equivalent to a small power plant. Silicon carbide (SiC) power devices enable this efficiency at higher voltages and temperatures than silicon, making SiC a mandatory upgrade for AI-scale power infrastructure.

---

## The Core Thesis

Power electronics is the unglamorous but essential interface between the grid and the chip. Every watt that enters a data center passes through multiple conversion stages before reaching a GPU. Each stage has conversion losses — typically 2-5% per stage in conventional silicon technology. In a 100 MW data center running conventional silicon, 4-8 MW is wasted as heat in power conversion stages alone.

Silicon carbide (SiC) transistors operate at:
- **Higher voltage** (1,200V vs. 650V for silicon): Fewer conversion stages needed → less total loss
- **Higher temperature** (175°C junction vs. 150°C for silicon): Less cooling required; more compact designs
- **Higher switching frequency** (100kHz+ vs. 20kHz for silicon): Smaller passive components (inductors, capacitors); more compact power supplies
- **Lower on-resistance**: Less heat dissipation at equivalent current levels

For AI data centers:
- **120 kW/rack demands** mean power conversion efficiency matters more than ever — both for energy cost and for cooling load
- **48V bus migration** requires new power conversion stages; SiC optimized for this voltage level
- **UPS systems** for AI clusters benefit enormously from SiC — more efficient, faster response, smaller footprint
- **Data center power density** growth makes SiC not an option but a requirement as rack power exceeds silicon limits

---

## The Two-Market Story

SiC adoption has two large, growing markets feeding the same companies:

**Market 1: Electric Vehicles**
EV inverters (converting DC battery power to AC motor power) were the original SiC killer app. Tesla Model 3 was the first mass-market EV to use SiC (STMicro supplier). By 2026, virtually every premium EV uses SiC. ON Semiconductor, Wolfspeed, Infineon, and STMicro all have major EV SiC design wins.

**Market 2: AI Data Centers**
The new and growing SiC market. UPS systems, power distribution units, AC-DC rectifiers, and DC-DC converters for AI infrastructure are all upgrading to SiC. Wolfspeed explicitly pivoted to this market with its June 2026 Silicon Valley AI data center team launch.

The companies that execute on both markets (ON, Infineon, STMicro) have more diversified demand than pure-play SiC manufacturers (Wolfspeed).

---

## SiC Substrate Chokepoint

The fundamental constraint in SiC supply is the substrate (the SiC crystal wafer on which devices are made). SiC crystals are grown very slowly (Lely method: weeks per ingot) and have higher defect densities than silicon. This makes SiC substrates 10-30x more expensive than silicon wafers and constrains device supply.

Wolfspeed is the world's largest SiC substrate manufacturer — if SiC adoption accelerates broadly, Wolfspeed's substrate position is strategically critical. However, Korean (SK Siltron), Japanese (Showa Denko), and Chinese (SICC) manufacturers are all expanding substrate capacity.

---

## Investment Implications

| Company | SiC Position | Other Exposure | Rating |
|---|---|---|---|
| [[MPWR]] | Power management ICs (not SiC devices, but benefits from SiC migration) | AI server VRMs | Hold/$1,700 |
| [[ON]] | SiC devices + Si power; EV + data center | Broad power semiconductor portfolio | Buy/$160 |
| [[WOLF]] | Pure-play SiC substrates + devices | AI data center pivot; financial risk | Under Review |
| Infineon (IFNNY) | SiC devices; EU leader | Automotive + industrial + data center | Not formally rated |

---

## Timeline

- **2023-2024:** SiC primarily EV-driven; data center SiC nascent
- **2025-2026:** AI data center SiC adoption accelerates (Wolfspeed June 2026 pivot validates)
- **2027-2030:** SiC becomes standard for AI data center UPS and PDU deployments; volume compounds
- **2030+:** GaN potentially displaces SiC in lower-voltage applications; SiC defends high-voltage territory

---

## Risks

1. **GaN leapfrog:** GaN offers higher switching speed; could displace SiC at lower voltages (< 650V) including some data center PSU applications
2. **Chinese SiC competition:** Government-subsidized Chinese SiC makers threaten pricing power
3. **EV adoption pace:** If EV growth disappoints, SiC OEMs' largest existing market shrinks
4. **Wolfspeed execution:** If Wolfspeed fails to convert its substrate position into profitable device sales, the pure-play SiC thesis weakens

---

## Review Note (2026-06-23)

Reviewed against AI capex deceleration scenario. **Dual-market structure provides insulation.** EVs remain the primary current SiC volume driver, entirely independent of AI capex. The data center SiC market (UPS, PDUs, AC-DC rectifiers) is early in adoption — the physics argument (120 kW racks require high-efficiency power conversion) is independent of how many racks are deployed, but the *pace* of new deployments does affect how quickly the data center market ramps.

Net effect: AI capex deceleration delays the data center SiC ramp by 1-2 years but doesn't change the destination. ON Semiconductor and Infineon's diversified SiC portfolios are more resilient than WOLF's pure-play exposure.

**WOLF (Wolfspeed) remains Under Review** — financial risk is the primary concern, compounded if data center SiC adoption slows. GaN competitive risk at lower voltages (<650V) is worth monitoring as data center PSU designs evolve.

**Conviction maintained at Medium-High.**

---

## Change Log
- `2026-06-03` — Thesis created. Evidence base: Wolfspeed June 2026 announcement, ON semiconductor filings, power electronics industry research.
- `2026-06-23` — Reviewed under AI capex deceleration. EV market provides diversified base; data center SiC ramp delayed but not broken. WOLF financial risk flagged. No rating changes.
