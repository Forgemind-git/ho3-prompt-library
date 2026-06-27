# Prompt 07 — KPI Definition Card

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Define a KPI with complete rigour — formula, data source, calculation frequency, owner, target, and interpretation guide — so every person in the organisation calculates it the same way and knows what to do when it moves.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | KPI name: [name]. Business function: [finance / sales / operations / CS]. Why this KPI matters: [what decision does it inform?]. Who uses it: [CFO / sales team / operations]. Current calculation method (if any): [describe or "not formalised"]. |
| **Role** | You are a finance analyst who documents KPIs with the precision of someone who has seen what happens when the same metric is calculated differently by different teams — you eliminate ambiguity before it causes a board meeting argument. |
| **Instruction** | Write a KPI definition card with: name, definition, formula, data source, calculation frequency, owner, target/benchmark, interpretation guide, and example calculation. |
| **Spec** | KPI card format. Each field clearly labelled. Formula in clear notation. Interpretation guide has three scenarios: good / concerning / critical. Example calculation with real numbers. 250–300 words. |
| **Performance** | Two people in different teams calculate this KPI independently and get the same number. When the KPI moves, anyone reading the interpretation guide knows whether to act. |

---

## Full Prompt

```
Context: I'm a financial analyst at [Company Name] formalising the definition of the following KPI: [KPI name]. This metric is used by [who — e.g., "the CFO for board reporting and the Sales VP for pipeline management"]. Currently, [describe how it's being calculated or "it is not formally defined"]. The business decision this KPI informs: [what changes when this number changes — e.g., "hiring decisions", "pricing changes", "board reporting"].

Provide any known information about how this should be calculated:
- Numerator: [what goes on top, or describe what you're measuring]
- Denominator: [what you're dividing by, if applicable]
- Inclusions / Exclusions: [any edge cases — e.g., "exclude trial users", "include churned customers in the base?"]
- Data source: [where the data comes from — CRM, billing system, data warehouse, etc.]

Role: Act as a finance analyst who documents KPIs with the precision needed to eliminate the "we calculate it differently" problem that surfaces in board meetings.

Instruction: Write a complete KPI definition card with:
1. KPI Name and Category
2. Definition — plain language description of what this measures and why it matters
3. Formula — clear notation (e.g., Metric = Numerator / Denominator × 100)
4. Inclusions and Exclusions — what counts and what doesn't (specific, not vague)
5. Data Source — where the data comes from, updated when
6. Calculation Frequency — how often it's calculated and who does it
7. Owner — who is responsible for the number's accuracy
8. Target / Benchmark — current target and, if available, industry benchmark
9. Interpretation Guide — three scenarios: good / concerning / critical with action implication
10. Example Calculation — a worked example with real-seeming numbers

Spec:
- KPI card format with clearly labelled fields
- Formula in explicit notation
- Interpretation: 3 tiers with action implication
- 250–300 words total
- One worked example with numbers

Performance bar: Two people calculate this independently and get the same number. Interpretation guide tells someone whether to act or monitor when the number moves.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Define our Net Revenue Retention KPI.

**Output produced:**
> Net Revenue Retention (NRR) measures how much revenue we retain from existing customers. A high NRR is good. It should be calculated monthly. The target is above 100%.

**Why it's weak:** No formula, no inclusion/exclusion rules, "high is good" is not an interpretation guide, no data source, no worked example. Two analysts will calculate this differently and argue about it in the next review.

---

## After Example (With CRISP)

**Placeholders filled:**
- KPI: Net Revenue Retention (NRR)
- Users: CFO + CS VP + Board
- Data source: Stripe (billing) + Salesforce (customer records)
- Inclusions/exclusions: Include expansion, exclude new logos, include churned customers in base

**Output produced:**

> **KPI DEFINITION CARD**
>
> | Field | Definition |
> |-------|-----------|
> | **KPI Name** | Net Revenue Retention (NRR) |
> | **Category** | Commercial / Customer Success |
> | **Owner** | VP Customer Success (accuracy) | CFO (board reporting) |
>
> **Definition**  
> NRR measures the percentage of recurring revenue retained from the existing customer base over a period, including expansion and contraction, but excluding new logo revenue. An NRR above 100% means existing customers are generating more revenue this period than last, even without any new customers.
>
> **Formula**  
> NRR = (MRR at End of Period from Cohort ÷ MRR at Start of Period from Same Cohort) × 100
>
> Where MRR at End = Opening MRR + Expansion MRR - Contraction MRR - Churn MRR
>
> **Inclusions / Exclusions**
> - Include: All recurring revenue from customers active at the start of the period; seat expansions; plan upgrades; contract renewals
> - Exclude: New logo revenue (customers who did not exist at period start); one-time fees; professional services revenue
> - Churned customers: Included in the denominator (as starting MRR), counted as $0 in the numerator
>
> **Data Source**  
> Stripe (billing data — MRR per customer) | Salesforce (customer cohort classification) | Updated: Monthly, 5th business day
>
> **Calculation Frequency**  
> Monthly (reported to board quarterly)
>
> **Target**  
> Current target: 110%+ | Industry benchmark (B2B SaaS): 100–120% | Best-in-class: 130%+
>
> **Interpretation Guide**
> - **Good (110%+):** Existing customers are expanding — monitor for acceleration; consider price increase evaluation
> - **Concerning (95–109%):** Marginal retention; investigate whether contraction is in specific segments or spread; CS team review required
> - **Critical (<95%):** Net shrinkage from existing customers; immediate churn analysis required; CSM intervention for top 20% of ARR at risk
>
> **Example Calculation**  
> Jan 1 cohort MRR: $300,000 | Feb 1 same cohort MRR: $321,000  
> Expansion: $35,000 | Contraction: $8,000 | Churn: $6,000  
> NRR = ($300K + $35K - $8K - $6K) ÷ $300K × 100 = **107%**
