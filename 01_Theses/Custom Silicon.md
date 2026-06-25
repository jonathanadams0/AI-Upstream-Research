---
status: Active
conviction: High
last_updated: 2026-06-23
tags: [thesis]
split_from: "AI Networking and Custom Silicon"
---

# Custom Silicon

> Hyperscalers are building a parallel AI silicon ecosystem to reduce Nvidia dependency — and Broadcom and Marvell are the dominant pick-and-shovel suppliers. These are multi-year design commitments (3-5 year cycles) that create sticky, recurring revenue. The AI capex ROI pressure that weakens other theses *strengthens* this one: the more hyperscalers need to justify AI spending, the more economically compelling 40-70% cost savings vs. Nvidia become.

---

## The Core Thesis

Nvidia's AI accelerator monopoly is expensive for hyperscalers. At ~$25,000-40,000 per H100 and 100,000-GPU cluster sizes, Nvidia hardware alone costs $2.5-4B before networking, power, or real estate. Each major hyperscaler is investing billions in custom AI ASICs designed for their specific workloads:

| Program | Hyperscaler | Partner | Use Case |
|---|---|---|---|
| TPU v5 | Google | Broadcom | Training + inference for Gemini/Search |
| Trainium 2 | Amazon | Marvell | AWS AI training; Titan LLM |
| Maia | Microsoft | Marvell | Azure internal AI + inference |
| MTIA | Meta | Broadcom | Recommendations, ranking, GenAI |

Each program represents billions in annual silicon procurement that did not exist 3 years ago. Once a hyperscaler designs a chip with Broadcom or Marvell, they commit for the next 3-5 years — creating sticky, recurring revenue that behaves nothing like commodity semiconductor cycles.

---

## Why This Is Counter-Cyclical to Capex Anxiety

This is the key variant perception. Most AI infrastructure theses weaken under AI capex deceleration. Custom silicon strengthens:

- **The ROI pressure argument:** When hyperscalers face scrutiny over AI spending returns, switching to custom silicon (40-70% lower cost per inference/training run vs. Nvidia) *increases* in attractiveness. CFOs cutting AI budgets look to Trainium and TPU first.
- **The design commitment lock-in:** A 3-5 year chip design cycle doesn't pause for quarterly sentiment. Programs already in flight continue regardless.
- **The strategic independence argument:** Geopolitical and supply chain concerns reinforce the desire to own silicon rather than depend on a single Nvidia supply chain.

---

## Investment Implications

| Company | Angle | Rating |
|---|---|---|
| [[AVGO]] | Primary partner for Google (TPU) and Meta (MTIA); $25B+ AI revenue in 2026 | Buy |
| [[MRVL]] | Primary partner for Amazon (Trainium 2) and Microsoft (Maia); early innings of multi-year ramp | Buy |

---

## Risks

1. **In-house silicon:** If a hyperscaler builds full internal chip design capability (beyond the ASIC co-design they do today), Broadcom/Marvell exposure decreases
2. **Nvidia competitive response:** Nvidia has begun offering disaggregated silicon (NVLink switches, custom accelerator programs) to retain hyperscaler relationships
3. **Design cycle delays:** A failed chip generation forces a 2-3 year redesign; one bad silicon spin can defer revenue meaningfully

---

## Key Signal to Watch

Broadcom Q3 FY2026 AI revenue vs. $16B guide (reports September 2026). A beat re-establishes the growth trajectory; a miss continues the plateau narrative from Q2.

---

## Change Log

- `2026-06-23` — Split from [[AI Networking and Custom Silicon]] following stress-test analysis. Conviction retained at High; thesis strengthened by capex deceleration scenario. See [[Thesis_Stress_Test_2026-06-23]].
