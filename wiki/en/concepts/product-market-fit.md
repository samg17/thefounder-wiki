---
title: Product-Market Fit (PMF)
category: concept
tags: [pmf, validation, retention, growth]
updated: 2024-01-01
sources: []
status: stable
related: [[icp]], [[unit-economics]], [[guardrails-market-research]]
---

# Product-Market Fit (PMF)

The point at which a product satisfies a market demand strongly enough to generate sustainable organic growth. Central concept for deciding when to scale.

**Classic definition:** PMF means being in a good market with a product that can satisfy that market.

**Practical definition:** Customers love the product, use it frequently, recommend it spontaneously, and you have difficulty keeping up with demand.

---

## PMF is not binary

PMF is a spectrum, not a switch. You can have weak PMF (enough to survive, not to scale), moderate PMF (growth possible with effort), or strong PMF (growth happens almost by itself).

Most startups that fail try to scale with weak or nonexistent PMF.

---

## How to measure PMF

### Must-have survey method

Ask active users: "How would you feel if you could no longer use [product]?"

- Very disappointed
- Somewhat disappointed
- Not disappointed (not really necessary)
- N/A, I've already stopped using it

**Benchmark:** If ≥40% answer "very disappointed," there's a strong PMF signal. (Popularized by Sean Ellis.)

**Limitation:** Works better for consumer products with many users. In B2B with few customers, the sample may be too small.

### Cohort retention

The most important retention chart: % of active users/customers over time, by acquisition cohort.

**PMF signal:** The retention curve flattens — there's a core of customers who keep using it indefinitely.

**No PMF signal:** The curve keeps falling and tends to zero — customers arrive, try it and leave.

### Net Promoter Score (NPS)

Question: "On a scale of 0–10, how likely are you to recommend [product] to a friend or colleague?"

```
NPS = % Promoters (9–10) - % Detractors (0–6)
```

Approximate benchmarks:
- NPS > 50: excellent, strong PMF signal
- NPS 30–50: good, PMF developing
- NPS < 30: warning signal

**Limitation:** NPS measures declared satisfaction, not real behavior. Combine with retention.

### Organic growth

What % of new customers comes from referral, word of mouth or organic search (without paid)?

- > 30% organic: positive PMF signal
- Growth only with paid, which stops when investment stops: warning signal

---

## Qualitative PMF signals

**Positive signals:**
- Customers get frustrated when the product is down or has bugs
- Customers build critical workflows on top of the product
- Sales gets easier over time (fewer objections, shorter cycles)
- Receiving requests from customers you didn't prospect
- Customers ask for expansion features, not basic features

**Absence of PMF signals:**
- High churn in the first 60–90 days
- Customers "like but don't use frequently"
- Sales is always hard, requires a lot of education effort
- Customers frequently ask for discounts
- Neutral NPS — nobody hates it, nobody loves it

---

## PMF is always relative to a segment

A product can have strong PMF with one ICP and no PMF with another. "We don't have PMF" often means "we don't have PMF with the segment we're pursuing."

Before concluding the product has no PMF, check:
- Is there a subgroup of customers with much better retention than average?
- What do the customers who stay have in common?
- Are you measuring PMF in the right segment?

See [[icp]].

---

## Common mistakes

❌ Scaling before having clear PMF
✅ PMF first, scale after. Growing with weak PMF burns capital and creates retention problems that become harder to fix at scale

❌ Confusing initial interest with PMF ("everyone loved the demo")
✅ PMF is measured in continuous use, not first impression

❌ Measuring PMF only with acquisition metrics (how many signed up)
✅ PMF is about retention — what matters is who stayed, not who arrived

❌ Believing PMF is permanent
✅ Market and competition change. PMF needs to be re-validated periodically

---

## What to do without PMF

1. Go back to customer research — [[guardrails-market-research]]
2. Identify the subgroup with the best retention and focus on them
3. Revisit the ICP — maybe the problem is the segment, not the product
4. Pivot based on real learning, not speculation
5. Don't aggressively hire a sales and marketing team — this amplifies problems, doesn't solve them

---

## Connections

- [[icp]] — PMF is always relative to a specific ICP
- [[unit-economics]] — without PMF, LTV is low and churn is high — unit economics don't work
- [[guardrails-market-research]] — how to research to find where PMF exists
