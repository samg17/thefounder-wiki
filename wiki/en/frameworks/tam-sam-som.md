---
title: TAM / SAM / SOM
category: framework
tags: [market, size, tam, sam, som, validation]
updated: 2024-01-01
sources: []
status: stable
related: [[porter-5-forces]], [[icp]], [[guardrails-market-research]]
---

# TAM / SAM / SOM

Framework for estimating and communicating market size. More important than the number itself is the **methodology** used to arrive at it.

---

## Definitions

| Acronym | Name | Definition |
|---|---|---|
| TAM | Total Addressable Market | The entire market if you had 100% share |
| SAM | Serviceable Addressable Market | The portion of TAM you can serve with your current model |
| SOM | Serviceable Obtainable Market | The portion of SAM you can realistically capture in 3–5 years |

**Analogy:** TAM = everyone who is hungry in the world. SAM = everyone who wants pizza in your city. SOM = who you can reach with your current delivery capacity.

---

## Why it matters

**For you:** Know whether the market is large enough for the business you want to build. A $10M business in a $50M market can be great. In a $100M market it may be hard to finance as a venture.

**For investors:** Validate whether there's room for a large business. Venture investors typically look for TAM of at least $1–10bn to justify their return model.

**Caution:** TAM impresses investors, SOM is what you need to defend with data.

---

## How to calculate — two approaches

### Top-down approach

Takes the total market of a category and funnels down.

```
Global CRM market: $60bn (source: Gartner 2023 report)
→ Target country represents ~X% of global GDP
→ SMB segment (your focus): 30% of market
= TAM: $Xbn
```

**Problem:** Relies on market reports that are often imprecise, outdated or use different market definitions than yours.

**When to use:** For initial investor communication, to establish order of magnitude.

### Bottom-up approach

Builds the number from the ground up from real data.

```
Number of potential customers in the segment: 50,000 companies (source: government registry)
× Estimated annual ticket: $6,000/year
= TAM: $300M
```

**Advantage:** More defensible, based on verifiable data.
**Problem:** Requires market data that doesn't always exist.

**When to use:** To validate and refine the top-down estimate. If both methods arrive at similar numbers, more confidence. If they diverge significantly, understand why.

### Analogy approach

Uses a similar market (another country, adjacent segment) as a reference.

```
USA: market X has 15% penetration with $500/company/year ticket
Target country has 1/X of US GDP → adjust for purchasing power parity
= Estimated TAM: $X
```

**When to use:** In new markets where there's no direct data. Always declare the analogy explicitly and its limitations.

---

## From TAM to SAM to SOM

**TAM → SAM:** Apply filters from your business model
- Geographic (you only operate in one city today)
- Segment (you only serve companies with 10–200 employees)
- Channel (you only sell direct, not through distributors)
- Support capacity (you don't yet have a team for enterprise)

**SAM → SOM:** Base on execution capacity
- How many customers can your team acquire and serve in the next 3 years?
- What is your estimated pipeline conversion?
- What is the capacity of your distribution channel?

SOM is the bridge between market and business plan. If your 3-year SOM implies an impossible growth rate, revise the model.

---

## Common mistakes

❌ Presenting TAM as if it were your real market
✅ Always present all three numbers and how you arrived at each

❌ Using generic TAM irrelevant to your segment ("the software market in Brazil")
✅ Define the market by the job you solve, not the technology category

❌ Not questioning the TAM source ("according to a report by consulting firm X")
✅ Verify: when was it published? How was it calculated? Does the market definition match yours?

❌ Optimistic SOM without basis in execution capacity
✅ SOM should be derivable from your plan: headcount × productivity × conversion

❌ Ignoring market dynamics (growth, seasonality, regulation)
✅ A $1bn TAM growing 30% per year is much more interesting than a stagnant $5bn TAM

---

## Presentation template

For investors, structure it like this:

> "The TAM is $X, calculated from [methodology]. The SAM for our segment [definition] is $Y. Our SOM target for the next 3 years is $Z, which represents [%] of SAM — consistent with [reference/benchmark]."

---

## Connections

- [[icp]] — the ICP definition is what transforms TAM into SAM
- [[porter-5-forces]] — market structure affects how much of the SAM you can capture
- [[guardrails-market-research]] — how to validate TAM assumptions with primary data
