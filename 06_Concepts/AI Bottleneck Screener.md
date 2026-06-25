---
tags: [concept]
last_updated: 2026-06-03
---

# AI Bottleneck Screener — Finding the Next Bloom Energy

> The biggest alpha in the AI infrastructure trade comes from finding companies priced as old-economy industrial businesses that are quietly becoming indispensable AI infrastructure plays — before the market reclassifies them. Bloom Energy ran +1,396% in 12 months. Caterpillar's backlog increased 71% YoY from data center power orders. Seagate was up 500%+ on AI cold storage demand. The pattern is repeatable. Here's the framework to find them systematically.

---

## The Pattern: The "Bloom Energy Trade"

Bloom Energy (BE) is the canonical example. For years it was priced as a speculative fuel cell company — clean energy enthusiast stock, not AI infrastructure. Then Oracle signed a 2.8 GW agreement for Project Jupiter (AI data center). Nebius signed a $2.6B deal for 328 MW. Aschenbrenner's Situational Awareness fund built a ~$900M position. The stock ran 1,396% in 12 months.

**What made Bloom discoverable before the run:**
1. It solved a specific, measurable AI bottleneck: dispatchable power without waiting years for grid interconnection
2. It was priced at utility/industrial multiples (~10-15x) while carrying growing AI order momentum
3. Its first hyperscaler contract validated the thesis (though for most of the run, the market hadn't priced it in)
4. Supply couldn't be quickly replicated: Bloom's solid oxide fuel cell technology takes years to manufacture at scale; competitors don't have equivalent commercial deployments

---

## The Five Screening Criteria

### Criterion 1: Physical Bottleneck Match
**Test:** Does the company supply something that physically limits AI infrastructure? Is it quantifiable?

| Bottleneck Category | Unit of Scarcity | Examples |
|---|---|---|
| Power generation | MW / GW | Bloom Energy, Caterpillar, Generac |
| Grid bypass | Time to power (days vs. years) | Bloom (fuel cells), CAT (generators) |
| Thermal/cooling | kW removed per sq ft | Vertiv, Modine |
| Optical connectivity | Gbps | Coherent, Lumentum, Fabrinet |
| Short-reach interconnect | Gbit/m | Credo (AECs) |
| Compute hosting | MW of GPU capacity | Core Scientific, Applied Digital, IREN |
| Storage | TB at lowest $/TB | Seagate, WDC (HDDs) |
| Specialty materials | Tonnes with no substitutes | Rare earths (MP Materials), SiC substrates (Wolfspeed) |

**Pass:** Company's primary product directly addresses one of these categories.

---

### Criterion 2: Old-Economy Multiple
**Test:** Is the stock priced at industrial/utility/materials multiples rather than tech multiples?

| Sector | Typical Multiple | "Repricing" Trigger |
|---|---|---|
| Industrials | 15-25x P/E | First hyperscaler contract |
| Utilities | 12-20x P/E | Power purchase agreement with tech company |
| Materials | 10-18x P/E | Supply constraint recognition |
| Energy equipment | 15-25x P/E | Data center end market enters earnings narrative |

**Pass:** Forward P/E or EV/EBITDA is below 25x at time of screening.

---

### Criterion 3: Hyperscaler Contract Signal
**Test:** Has at least one hyperscaler (MSFT, GOOG, AMZN, META, Apple, NVDA, Oracle) signed a contract specifically for AI infrastructure with this company in the last 12 months?

Evidence types (in order of strength):
1. Formal purchase agreement disclosed in 8-K or press release (**strongest**)
2. Named customer relationship disclosed in earnings call (**strong**)
3. New "data center" segment or product line announced (**moderate**)
4. Job postings for "hyperscaler partnership" roles (**weak but early signal**)

**Pass:** At least one Type 1 or Type 2 evidence exists, or compelling Type 3 + 4 combination.

---

### Criterion 4: Supply Cannot Be Quickly Replicated
**Test:** Is there a genuine reason competitors cannot respond within 12-18 months?

| Barrier Type | Examples | Time to Replicate |
|---|---|---|
| Manufacturing complexity | SiC crystal growth, fuel cell stack manufacturing | 3-5 years |
| Regulatory | Nuclear permitting, hazardous material permits | 5-15 years |
| Installation timeline | Grid interconnection queue, transformer lead times | 2-4 years |
| Geographic uniqueness | Existing facilities in desired locations | 2-3 years |
| Proprietary technology | Patented processes, trade secrets | Indefinite |
| Network effects | Existing customer relationships, installed base | 2-5 years |

**Pass:** At least one meaningful barrier to rapid supply replication.

---

### Criterion 5: Backlog Growing Faster Than Revenue
**Test:** Is the company's order backlog growing at least 2x faster than trailing revenue?

| Company (Examples) | Revenue Growth | Backlog Growth | Signal |
|---|---|---|---|
| Caterpillar (2025-26) | +10-12% | +71% | Strong |
| Bloom Energy (2025-26) | +130% | Similar | Strong |
| GE Vernova (2025-26) | +16% | +$35B QoQ | Strong |
| Generac (2026) | +12% | $700M DC-specific | Moderate |

**Pass:** Backlog growing ≥2x the rate of reported revenue.

---

## Data Sources for Ongoing Screening

### Primary (monitor weekly)
1. **8-K contract announcements** via SEC EDGAR full-text search for "data center" OR "hyperscaler" filed by Industrials/Utilities/Materials sector companies
2. **13F filings** of AI-focused funds (Aschenbrenner's Situational Awareness, Tiger Global, Coatue, a16z equity) — overlapping positions signal convergent thesis validation
3. **Earnings call transcripts** via Bigdata.com or Quartr — search for "data center" appearing in transcripts of companies that never mentioned it before

### Secondary (monitor monthly)
4. **Industrial backlog disclosures** — quarterly earnings tables showing order backlog by segment
5. **Hyperscaler earnings calls** — when MSFT/GOOG/AMZN/META mention supplier names or "strategic partnerships" with non-tech companies
6. **Job posting analysis** — hyperscalers hiring "Power Procurement Manager", "On-Site Generation Director", "Fuel Cell Operations Lead" signals new supplier categories being developed
7. **Patent filings** — industrial companies filing data-center-specific patents (thermal management, power conversion, modular facilities)

### Tertiary (scan quarterly)
8. **Trade press** — *Data Center Dynamics*, *Data Center Magazine*, *Energy Digital* — for supplier mentions in data center construction stories
9. **Conference presentations** — NVIDIA GTC, AWS re:Invent vendor slides — who is listed as "infrastructure partner"?
10. **Government procurement** — DoD and DOE contracts for AI data center power infrastructure (the US government is also building AI clusters)

---

## Current Screening Candidates (as of June 3, 2026)

### High Conviction — Already Initiating
| Ticker | Bottleneck | Signal | Multiple |
|---|---|---|---|
| BE | Grid-bypass power | Oracle 2.8GW + Nebius $2.6B | ~50x (re-rated) |
| CAT | Gas generator sets | 2GW order from AI Power Corp; MSFT-NVDA deal | ~25x → repricing |
| GNRC | Standby/prime power | $700M DC backlog, hyperscaler approvals | ~20x → repricing |
| LITE | Optical transceiver | S&P 500 #6 performer YTD; AI interconnect | ~40x |
| FN | Transceiver manufacturing | Makes for COHR, LITE — pure demand leverage | ~30x |

### Medium Conviction — Under Research
| Ticker | Bottleneck | Signal | Action |
|---|---|---|---|
| CLS (Celestica) | Electronics mfg | Making AI networking hardware (HPE, Cisco) | Research |
| AECOM/ACM | Data center EPC | Engineering AI campuses globally | Research |
| XYL (Xylem) | Water cooling | AI data centers huge water consumers | Research |
| APD (Air Products) | Specialty gases | Chip fab + data center cooling gases | Research |
| LIN (Linde) | Specialty gases | Largest industrial gas; chip + cooling | Research |
| FCEL (FuelCell Energy) | On-site power gen | Smaller Bloom; similar AI data center pitch | Research |
| OKLO | Micro-reactors | OpenAI/SBF backed; nuclear for AI clusters | Watch |

### The "Miners to Hosts" Basket
| Ticker | Status | AI Contract | Price |
|---|---|---|---|
| CORZ | Being acquired by CoreWeave | 590 MW / $10B over 12 years | $29 |
| APLD | Independent AI host | HPC data centers in ND, TX | $48 |
| IREN | Independent AI host | Growing GPU hosting revenue | $67 |
| CLSK | Still mining-heavy | Pivoting more slowly | $18 |

---

## Pattern Recognition — What to Look For

**The most useful signal: "data center" appearing for the first time in an industrial company's earnings transcript.**

When the Caterpillar CEO says "we're seeing unprecedented demand from data center customers" for the first time in 40 years of earnings calls, that's a signal. When Seagate CFO says "our top customer has ordered three times the historical volume for AI training data archiving," that's a signal.

**The second most useful signal: a company you've never associated with AI signs a contract with a hyperscaler.**

Bloom Energy → Oracle. Core Scientific → CoreWeave (acquisition). These are discontinuous events. Monitor 8-Ks.

**The third most useful signal: Aschenbrenner or other AI-infrastructure-focused funds building a position in an industrial company.**

Their 13F filings lag by 45 days but still provide validation. Situational Awareness LP's $879M Bloom position told you the thesis before most retail investors realized Bloom had become an AI stock.

---

## Anti-Patterns: What Does NOT Pass

1. **"Exposed to AI" is not the same as "bottleneck."** Every company is exposed to AI. Only a subset is a physical constraint on AI expansion.
2. **A press release saying "we serve data centers" does not mean hyperscaler adoption.** Look for specific named customers or specific MW/TB/Gbps commitments.
3. **If analysts have already re-rated the stock to AI multiples, the trade is likely over.** The opportunity is in the gap between industrial multiple and AI multiple.
4. **Single-customer concentration is a risk, not a signal.** Bloom's Oracle deal is great, but if Oracle is 80% of revenue, you're underwriting Oracle's capex continuity too.
