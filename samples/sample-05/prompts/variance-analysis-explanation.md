# Prompt 01 — Variance Analysis Explanation

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Translate a budget vs actual variance into plain language that a business leader (non-financial) can understand and act on — with root cause, business impact, and a recommended response — without turning it into a spreadsheet lecture.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Report period: [month/quarter]. Budget: $[X]. Actual: $[Y]. Variance: $[Z] ([favorable/unfavorable], [%]). Root cause breakdown: [list the drivers]. Audience: [department head / CEO / board]. |
| **Role** | You are a financial analyst who translates numbers into narrative — you know that a CFO doesn't need the variance explained, but the operations director does, and you adjust accordingly. |
| **Instruction** | Write a variance explanation with: headline finding in one sentence, root cause breakdown (quantified), business impact, and recommended management response. |
| **Spec** | Written explanation, not a table. 200–250 words. Numbers first, narrative second. Audience-calibrated language (adjust jargon level based on audience). Recommended response must be specific. |
| **Performance** | A non-financial department head reads this and understands what happened, why, and what they should do. No financial jargon unexplained. One specific recommendation they can act on this week. |

---

## Full Prompt

```
Context: I'm a financial analyst at [Company Name] preparing a variance analysis explanation for [period — e.g., "Q2 2025" or "June 2025"]. 
- Budget: $[X]
- Actual: $[Y]  
- Variance: $[Z] [favorable (F) / unfavorable (U)]
- Variance %: [X%]
- Root causes of variance (be specific with $ amounts for each cause):
  1. [Cause 1 — e.g., "Higher than budgeted headcount costs: +$45,000 due to 2 unplanned contractor engagements"]
  2. [Cause 2]
  3. [Cause 3 if applicable]
- Audience: [e.g., "Marketing department head with no formal finance background" / "CFO" / "Board of Directors"]
- What decision this analysis is informing: [e.g., "Q3 budget reforecast" / "approving additional headcount" / "board budget review"]

Role: Act as a financial analyst who writes variance explanations for non-financial leaders — you translate numbers into business language without dumbing things down, and you always include a clear "so what" and "what to do about it."

Instruction: Write a variance explanation with:
1. Headline — one sentence: what happened, how big, favorable or not
2. Root Cause Breakdown — explain each driver in plain language, with the $ amount; use business language not accounting language
3. Business Impact — what this variance means for the business (cash, headcount, future quarters)
4. Recommended Response — one specific, actionable recommendation for the audience to consider
5. Watch for Next Period — one thing to monitor that could affect the trend

Spec:
- Written explanation (not a table or slides)
- 200–250 words
- Numbers before narrative in each section
- Adjust jargon level to the audience described
- Recommended response must be specific and actionable

Performance bar: Non-financial audience reads this and understands what happened without asking follow-up questions about the numbers. Recommended response is specific enough to discuss in a meeting.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Explain a budget variance to my manager.

**Output produced:**
> The budget variance for the period was $50,000 unfavorable. This was due to higher than expected costs across several line items. Management should review spending and implement cost controls to ensure future compliance with the budget.

**Why it's weak:** "Several line items" is meaningless, "implement cost controls" is vague, "ensure future compliance" is generic. The manager reading this has no idea what changed or what to do.

---

## After Example (With CRISP)

**Placeholders filled:**
- Period: Q2 2025 | Company: Helply
- Budget: $620,000 | Actual: $688,000 | Variance: $68,000 unfavorable (11.0%)
- Root causes: Headcount costs +$45K (2 contractors for migration project), software +$12K (unplanned Snowflake overage), travel +$11K (two US sales trips)
- Audience: VP Operations, no formal finance background
- Decision: Q3 budget reforecast

**Output produced:**

> **Q2 2025 Cost Variance — Operations Summary**
>
> **Headline**  
> Operations spent $68,000 (11%) over budget in Q2, driven primarily by the CRM migration project and two unplanned US sales trips.
>
> **Root Cause Breakdown**
>
> The biggest driver was **headcount costs** — two software contractors were brought in to support the CRM migration in May and June, adding $45,000 not in the original budget. This was a deliberate decision to accelerate the migration timeline; the cost was not a runaway expense but an unplanned project investment.
>
> **Software costs** came in $12,000 over budget due to higher-than-expected data processing volumes in Snowflake (our cloud data tool). This is directly tied to the migration project's data validation work — it will normalise once migration is complete.
>
> **Travel costs** were $11,000 over budget, reflecting two US sales trips that closed deals worth $180,000 in combined ARR.
>
> **Business Impact**  
> The $68,000 overspend is offset by the migration work now completing 3 weeks ahead of schedule and the $180,000 in new ARR from the sales travel. On a net basis, this is a positive quarter.
>
> **Recommended Response**  
> For the Q3 reforecast, increase the software budget line by $8,000/month through August to reflect actual Snowflake usage, then step it down in September once migration concludes.
>
> **Watch for Q3**  
> If the Snowflake data volumes don't decline after migration closes, the software line needs a permanent budget adjustment in Q4.
