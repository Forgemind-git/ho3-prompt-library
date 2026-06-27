# Prompt 03 — Budget Commentary Draft

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Draft a monthly or quarterly budget commentary that gives department heads and senior leadership a clear picture of financial performance, the key drivers of variance, and management's response — written for a business audience, not an accounting one.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Period: [month/quarter]. Company/division: [name]. Overall result: [budget vs actual, $ and %]. Key variance drivers: [list]. Significant events this period: [new hires, contracts, one-offs]. Audience: [leadership team / department heads / board]. |
| **Role** | You are a finance business partner who writes budget commentary that business leaders read — not a finance team memo that gets skimmed for the bottom line. |
| **Instruction** | Write a budget commentary with: executive summary (3 sentences), P&L headline results, key variance explanations by category, year-to-date tracking, and outlook for next period. |
| **Spec** | Management commentary format. 350–400 words. Numbers in bold where significant. Each major variance explained in 2–3 sentences maximum — business language, not accounting. No columns of numbers — this is narrative. |
| **Performance** | A department head reads this in 3 minutes and knows: the overall result, why variance occurred, and what to expect next month. No unexplained acronyms. No tables — pure narrative commentary. |

---

## Full Prompt

```
Context: I'm a financial analyst at [Company / Division Name] preparing the [month / quarter] [year] budget commentary. Audience: [leadership team / department heads / board / investors].

Financial results for [period]:
- Revenue: Budget $[X] | Actual $[Y] | Variance: $[Z] [F/U] ([%])
- Operating costs: Budget $[X] | Actual $[Y] | Variance: $[Z] [F/U] ([%])
- EBITDA / Net income: Budget $[X] | Actual $[Y] | Variance: $[Z] [F/U] ([%])
- YTD revenue: $[X] vs Budget $[Y] (ahead / behind by $[Z])

Key variance drivers (with $):
1. [Driver 1 — e.g., "Revenue: New Enterprise contract signed late — $40K deferred to July"]
2. [Driver 2 — e.g., "Costs: R&D headcount +2 vs plan — $25K unfavorable"]
3. [Driver 3 if applicable]

Significant events this period: [e.g., new product launch, key customer loss, M&A, restructuring, one-off items]
Outlook for next period: [describe expected changes — e.g., "deferred revenue recognises in July; headcount spend stabilises"]

Role: Act as a finance business partner who writes budget commentary that business leaders actually read — narrative that explains performance in business terms, not accounting language.

Instruction: Write a management budget commentary with:
1. Executive Summary — 3 sentences: overall result, headline driver, one forward-looking statement
2. Revenue Commentary — 2–3 sentences on revenue performance and key drivers
3. Cost Commentary — 2–3 sentences on the major cost variances and whether they are structural or one-off
4. EBITDA / Bottom Line — 1–2 sentences on the net result and what it means
5. Year-to-Date Tracking — brief statement of YTD position and whether we're on track for the full year
6. Outlook — 2–3 sentences on what to expect next period and any key decisions or events that will affect performance

Spec:
- Management commentary narrative format (no tables)
- 350–400 words
- Numbers in bold where significant
- Business language — explain "EBITDA" if the audience isn't finance-trained
- No unexplained acronyms

Performance bar: Department head reads this in 3 minutes and knows the overall result, why it happened, and what to expect next month. No financial jargon that a non-finance leader can't follow.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a budget commentary for this month.

**Output produced:**
> June 2025 Budget Commentary. Revenue was $800K vs budget of $850K. Costs were $600K vs budget of $580K. EBITDA was $200K vs budget of $270K. Variances were driven by lower revenue and higher costs. The team will work to improve performance next month.

**Why it's weak:** This is a table summary, not a commentary. No explanation of what drove the variances, "work to improve" is not an outlook, no narrative value for any reader. A CFO reading this learns nothing they didn't know from the spreadsheet.

---

## After Example (With CRISP)

**Placeholders filled:**
- Company: Helply | Period: June 2025
- Revenue: Budget $850K | Actual $800K | ($50K) unfavorable
- Costs: Budget $580K | Actual $600K | $20K unfavorable
- EBITDA: Budget $270K | Actual $200K | ($70K) unfavorable
- Drivers: Revenue — one Enterprise contract delayed signing; Costs — one-off AWS migration spend $20K
- YTD: Revenue $4.8M vs budget $4.9M — $100K behind

**Output produced:**

> **June 2025 Budget Commentary — Helply**
>
> **Executive Summary**  
> June EBITDA came in at **$200K**, **$70K below plan**, driven by a delayed Enterprise contract signing and a one-off infrastructure cost. Both of these factors are timing-related — the Enterprise contract signed on July 3 and the infrastructure cost was a planned migration accelerated into June. Year-to-date we remain on track for the full-year plan.
>
> **Revenue — $800K (Plan: $850K | $50K Unfavorable)**  
> Revenue missed plan by **$50K** primarily because one Enterprise deal (TechCorp, **$50K ARR**) did not sign until after month-end. Contract negotiations were completed by June 28 but legal review extended past June 30 — revenue will be recognised in July. Excluding this timing difference, June performance would have been exactly on plan. SMB and Mid-Market revenue were both in line with budget.
>
> **Costs — $600K (Plan: $580K | $20K Unfavorable)**  
> Operating costs were **$20K over plan**, entirely attributable to a one-off AWS infrastructure migration that the engineering team accelerated to take advantage of a vendor credit window. This cost was planned for Q3 but the timing shift brings forward **$8K in savings** expected in Q3 and Q4 from reduced hosting fees. All other cost lines — headcount, marketing, G&A — were within 2% of plan.
>
> **EBITDA — $200K (Plan: $270K | $70K Unfavorable)**  
> The net EBITDA shortfall of **$70K** reflects the two items above. Both are timing-driven, not structural. Cash generation remains healthy and working capital is not affected.
>
> **Year-to-Date**  
> YTD revenue of **$4.8M** is **$100K (2%) behind plan** — primarily the TechCorp timing difference. Costs are tracking within 1% of plan YTD. Full-year outlook is unchanged; we expect to recover the H1 timing shortfall in H2.
>
> **July Outlook**  
> July revenue will benefit from the TechCorp contract signing (**$50K recognised**) and two additional Enterprise pilots converting to paid agreements (estimated **$80K combined**). Infrastructure savings from the June migration begin in July. We expect July EBITDA to be **above plan** by approximately $30–50K.
