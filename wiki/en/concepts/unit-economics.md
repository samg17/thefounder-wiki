---
title: Unit economics
category: concept
tags: [financial, cac, ltv, margin, payback, saas]
updated: 2024-01-01
sources: []
status: stable
related: [[icp]], [[product-market-fit]]
---

# Unit economics

Metrics that measure the profitability of one unit of the business — typically one customer. Fundamental for knowing whether the business model is sustainable before scaling.

**Golden rule:** Never scale before understanding your unit economics. Growing fast with negative unit economics is burning money faster.

---

## The core metrics

### CAC — Customer Acquisition Cost

How much you spend to acquire one paying customer.

```
CAC = Total spent on sales and marketing (period)
      ÷ Number of new customers acquired (same period)
```

**Include in the numerator:** Salaries of sales and marketing team, tools, ads, events, agencies, content, SEO — everything that goes toward acquisition.

**Period:** Use the same period for numerator and denominator. If there's a lag between investment and conversion (long sales cycle), adjust the period.

**CAC by channel:** Calculate separately per acquisition channel. Blended CAC hides which channel is working.

---

### LTV — Lifetime Value

How much a customer generates in revenue (or margin) over the entire relationship with the company.

**Simple version (revenue):**
```
LTV = Average monthly ticket × Average retention time (months)
```

**More precise version (contribution margin):**
```
LTV = Monthly gross margin per customer × Average retention time
```

Use the margin version to compare with CAC — you want to know if the customer generates enough profit to cover the acquisition cost.

**Churn and LTV:** LTV is extremely sensitive to churn.

| Monthly churn | Average retention time |
|---|---|
| 1% | ~8 years |
| 3% | ~2.8 years |
| 5% | ~1.7 years |
| 10% | ~10 months |

Small reductions in churn have a disproportionate impact on LTV.

---

### Payback period

How many months until the customer pays back the CAC.

```
Payback = CAC ÷ Monthly contribution margin per customer
```

**Why it matters:** It's the period you need capital before a customer becomes profitable. Long payback = more capital needed to grow.

General benchmarks (vary by segment and model):
- Excellent: < 12 months
- Acceptable: 12–24 months
- Concerning: > 24 months

---

### Gross margin

Revenue minus direct product/service delivery costs (COGS).

```
Gross margin = (Revenue - COGS) ÷ Revenue
```

**What goes in COGS:** Hosting, third-party licenses, customer support (if direct), payment processing costs.

**Does not go in COGS:** Sales, marketing, R&D, G&A.

Approximate benchmarks by model:
- Pure SaaS: 70–85%
- SaaS with embedded service: 50–70%
- Marketplace: 60–80%
- E-commerce: 20–50%
- Hardware: 30–60%

**Why it matters:** Gross margin defines the ceiling of LTV and the capacity to invest in growth.

---

## The LTV:CAC ratio

The most cited metric in unit economics.

**Interpretation:**
- LTV:CAC < 1 → you destroy value acquiring customers
- LTV:CAC = 1–3 → you cover CAC but little left over
- LTV:CAC ≈ 3 → benchmark for healthy SaaS (the 3x rule)
- LTV:CAC > 5 → either you're underinvesting in growth or the denominator is underestimated

**Caution:** LTV:CAC of 3x with 36-month payback is very different from LTV:CAC of 3x with 8-month payback. Present both.

---

## Common mistakes

❌ Calculating LTV without correctly discounting churn
✅ Use real monthly churn, not optimistically estimated

❌ Excluding sales team salaries from CAC
✅ CAC must include everything — salary, commission, tools, sales team overhead

❌ Using revenue LTV instead of margin LTV to compare with CAC
✅ Compare CAC with what the customer generates in **margin**, not gross revenue

❌ Calculating blended unit economics when there are multiple segments
✅ Calculate by segment, by channel, by cohort — blended hides what's working

❌ Projecting LTV assuming zero churn or churn that has never been measured
✅ Use real historical churn. If no history, use industry benchmarks as lower bound

❌ Scaling before having positive payback in at least 1 cohort
✅ Validate unit economics in one segment before replicating

---

## How to interpret by stage

**Pre-revenue:** Estimate CAC from industry benchmarks. LTV is hypothesis.

**Early stage (first 10–20 customers):** Unit economics are noisy — small cohorts, artificially high CAC (founder sells directly), unproven LTV. Focus on understanding the structure, not the absolute numbers.

**Growth:** Cohorts start to stabilize. Compare recent cohorts with older ones — unit economics should improve with channel and product learning.

**Scale:** Unit economics should improve with CAC economies of scale (brand, referral, inbound) and LTV (churn reduction, revenue expansion per customer).

---

## Connections

- [[icp]] — unit economics vary significantly by segment. Calculate per ICP.
- [[product-market-fit]] — without PMF, LTV is low and churn is high — unit economics don't work
