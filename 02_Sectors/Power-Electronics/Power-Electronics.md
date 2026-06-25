---
sector: Power-Electronics
last_updated: 2026-06-03
tags: [sector]
---

# Power Electronics — Sector Primer

> Every watt of electricity entering a data center passes through power conversion stages before reaching a compute chip. Wide-bandgap semiconductors (silicon carbide, gallium nitride) make these conversions dramatically more efficient — reducing heat, cutting energy costs, and enabling the higher power densities that AI infrastructure demands.

---

## 1. Industry Overview

Power electronics is the technology of controlling and converting electrical power. In data centers, this manifests as:

1. **Utility-scale conversion:** High-voltage AC from the grid → medium voltage DC → 480V or 240V bus bar → rack-level power distribution units (PDUs)
2. **UPS (Uninterruptible Power Supply):** Backup power conversion; battery systems that kick in if grid power fails
3. **Server-level PSU:** The power supply unit inside each server that converts rack-level AC/DC to the 12V or 48V that the GPU/CPU requires
4. **On-chip voltage regulation:** Voltage regulator modules (VRMs) and power management ICs that deliver the precise voltages (0.7-1.8V) that modern GPUs require

The key material transition: **silicon → silicon carbide (SiC) → gallium nitride (GaN)**. Traditional silicon power transistors have physical limits on switching frequency, voltage, and temperature. SiC and GaN can operate at higher voltages, higher temperatures, and higher switching frequencies — enabling more efficient, more compact, and more capable power conversion.

---

## 2. AI/Power Electronics Linkage

**Higher power density demands better power conversion:**
- A standard 2024 server rack: ~15-20 kW. Power conversion efficiency of 94-96% is acceptable.
- A GB200 NVL72 AI rack: 120 kW. At 120 kW, a 1% efficiency improvement saves 1.2 kW per rack. At 100,000 racks, that's 120 MW of electricity — more than a nuclear power plant's output.

**AI data centers are SiC's killer app:**
- SiC transistors operate at higher voltages (1,200V+ vs. 650V for Si), reducing the number of conversion stages
- SiC enables bidirectional power flow — essential for battery-backed UPS systems
- SiC runs cooler, reducing cooling requirements (feeding back into [[Cooling-Thermal]])
- SiC switches faster (100kHz+), enabling smaller magnetics and more compact designs

**48V bus migration:**
- Traditional data centers use 12V server rails. AI data centers are migrating to 48V racks, then to rack-level 48V → on-board 12V/5V conversion. This migration requires new power management ICs (Monolithic Power Systems leads here) and new SiC/GaN components.

**Power management ICs for AI chips:**
- Modern AI GPUs have dozens of power domains (different voltage rails for different circuits). Managing these precisely is the job of power management ICs. MPWR's VRMs and power converters are inside every leading AI server from Dell, HPM, Supermicro.

---

## 3. Value Chain

```
Grid power (AC high voltage)
        ↓
SiC/GaN power transistors (Wolfspeed, ON Semi, Infineon, STMicro)
        ↓
Power conversion modules → UPS → PDU
        ↓
Server PSU (48V → 12V)
        ↓
Power management ICs and VRMs (MPWR, Texas Instruments, Renesas)
        ↓
GPU/CPU at precise voltage (0.7-1.8V)
```

---

## 4. Competitive Landscape

| Company | Ticker | Sub-segment | AI Data Center Angle |
|---|---|---|---|
| Monolithic Power Systems | MPWR | Power management ICs + VRMs | Inside every major AI server; 48V migration beneficiary |
| ON Semiconductor | ON | SiC + Si power devices | SiC for data center UPS and power conversion |
| Wolfspeed | WOLF | SiC (pure-play) | Dedicated AI data center power team launched June 2026 |
| Infineon Technologies | IFNNY | SiC + Si + power controllers | Large SiC position; European-listed |
| STMicroelectronics | STM (not in coverage) | SiC + GaN | Apple relationship; strong SiC portfolio |
| Texas Instruments | TXN (not in coverage) | Power management ICs | Broad portfolio; competitive with MPWR |

---

## 5. Key Metrics to Track

| KPI | Why It Matters | Source |
|---|---|---|
| MPWR data center revenue % | Primary indicator of AI server power management adoption | MPWR quarterly |
| ON SiC revenue and growth | Pace of SiC adoption in data center vs. EV | ON quarterly |
| Wolfspeed data center order intake | Validation of AI power market pivot | WOLF earnings + press releases |
| Industry SiC substrate pricing | Supply bottleneck signal | Yole Intelligence reports |
| Data center power conversion efficiency (PUE) | Industry-level demand signal | Uptime Institute surveys |
| 48V rack adoption rate | Migration catalyst for new power ICs | Data center operator announcements |

---

## 6. Valuation Context

| Company | Forward P/E | Key Thesis | Risk Level |
|---|---|---|---|
| MPWR | ~50-60x | Power management monopoly inside AI servers; high margin | Premium valuation; high |
| ON | ~20-25x | SiC leader at reasonable valuation; EV + AI | Moderate; EV execution risk |
| WOLF | High/NM | Distressed SiC pure-play pivoting to AI power | High; financial risk |
| IFNNY | ~20-25x | Diversified SiC/power; EU-listed | Moderate; currency risk |

---

## 7. The SiC Substrate Bottleneck

Silicon carbide wafers are significantly harder to manufacture than silicon wafers. Key constraints:
- SiC boules (the crystal ingots) must be grown very slowly — weeks per ingot vs. hours for silicon
- Defect density in SiC wafers is much higher than silicon, reducing usable die per wafer
- Wolfspeed operates the world's largest SiC substrate manufacturing facility in Durham, NC; a new facility in Siler City, NC (the "Mohawk Valley Fab") is ramping

**Investment implication:** Even if SiC device demand accelerates rapidly, substrate supply limits the pace. Wolfspeed's substrate capacity is the chokepoint for the entire SiC supply chain.

---

## 8. Risks

1. **GaN leapfrog:** Gallium nitride (GaN) offers even higher switching speeds than SiC for lower-voltage applications. Texas Instruments, Navitas, and EPC are developing GaN power devices that could displace SiC in some data center applications.
2. **Wolfspeed financial distress:** Wolfspeed's capital-intensive SiC facility ramp has been expensive; balance sheet risk remains elevated.
3. **Chinese SiC competition:** CREE/Wolfspeed, Infineon, and STM face competition from Chinese SiC makers (SICC, TankeBlue) that benefit from subsidies.
4. **EV demand normalization:** ON and Wolfspeed have significant EV SiC exposure; EV adoption slowdown would reduce that revenue stream.

---

## 9. Data Sources

- Yole Intelligence — SiC and GaN power device market reports
- Omdia — power semiconductor market sizing
- Company quarterly earnings (MPWR, ON, WOLF)
- Bigdata.com — earnings transcripts
