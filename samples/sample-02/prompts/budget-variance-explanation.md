# Prompt 09 — Budget Variance Explanation

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Explain a project budget variance (overspend or underspend) clearly to non-financial stakeholders — with root cause, impact on project completion, corrective actions, and a revised forecast — without hiding problems or over-engineering the explanation.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Project [name]. Approved budget: $[X]. Actual spend to date: $[Y]. Variance: $[Z] over/under ([%]). Root cause: [what drove the variance]. Phase: [what stage you're at]. |
| **Role** | You are a PM who explains financial variance honestly — you don't minimise overruns or pad underspend explanations. You make financial information accessible to non-financial audiences. |
| **Instruction** | Write a budget variance explanation with: variance summary (numbers upfront), root cause breakdown, impact on project completion, corrective actions (if overspend) or reforecast (if underspend), and revised budget forecast. |
| **Spec** | Written explanation with a summary table at the top. 200–250 words. Numbers first, narrative second. Corrective actions are specific — not "tighten spending." |
| **Performance** | A non-financial stakeholder understands the variance, its cause, and the team's response in under 2 minutes. The revised forecast gives them a number they can report upward. |

---

## Full Prompt

```
Context: I'm the PM for [Project Name]. Our approved budget was $[X]. Actual spend to date (as of [date], end of [phase/week]): $[Y]. Variance: $[Z] [over / under] budget, representing a [%] variance. We are [N%] through the project timeline.

Root cause of variance:
- [Cause 1 and $amount — e.g., "Vendor API integration required 40h extra dev time: +$6,000"]
- [Cause 2 and $amount]
- [Cause 3 if applicable]

Remaining budget needed to complete: $[estimated]
Revised total forecast: $[X + variance needed]

Role: Act as a PM who gives honest, clear budget variance explanations to non-financial stakeholders. You never hide overruns or obscure the numbers in technical language.

Instruction: Write a budget variance explanation with:
1. Variance Summary Table — approved vs actual vs forecast (3 rows, 3 columns)
2. Root Cause — explain each cause in plain language, with the dollar amount
3. Impact on Delivery — will this affect timeline, scope, or quality?
4. Corrective Actions (if overrun) — 2–3 specific actions with owner and expected savings/impact
5. Revised Forecast — the new number to completion, clearly stated

Spec:
- Summary table at the top
- 200–250 words
- Numbers always before narrative
- Corrective actions specific (not "reduce spend")
- One clear revised forecast number

Performance bar: Non-financial stakeholder understands the variance in 2 minutes. Revised forecast is a single specific number. Corrective actions are actionable this week.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Explain why we're over budget on the project.

**Output produced:**
> We have experienced some unexpected costs on the project which have resulted in a budget variance. The team has been working hard to manage costs but there have been some challenges. We will continue to monitor the budget going forward.

**Why it's weak:** No numbers, no root cause, no corrective action, "continue to monitor" is not a plan. A CFO reading this learns nothing and will ask 10 follow-up questions.

---

## After Example (With CRISP)

**Placeholders filled:**
- Project: Atlas CRM Migration | Approved: $180,000 | Actual to date: $156,000
- We are 65% through the project
- Variance: $20,400 over (13.2%) | Due to: extra dev time on data migration + vendor delay costs
- Estimated to complete: $52,000 (vs original remaining of $31,600)
- Revised total forecast: $208,000

**Output produced:**

> **Budget Variance Report — Atlas CRM Migration**  
> As of June 27, 2025 | Reported by: James Reid (PM)
>
> **Summary**
>
> | | Approved | Actual (to date) | Forecast (to completion) |
> |-|----------|-----------------|------------------------|
> | Amount | $180,000 | $156,000 (65% spent) | $208,000 |
> | Variance | — | ($24,400) over plan | ($28,000) over budget |
>
> **Root Cause**
> - **Data migration complexity (+$18,000):** Legacy data contained 4,200 records requiring manual remediation not scoped in the original estimate. This required 120 additional developer hours at $150/h.
> - **Vendor delay costs (+$6,000):** Migrex API delivery was 5 days late; team retained on standby during the delay at a cost of $6,000.
>
> **Impact on Delivery**  
> Timeline is not affected — the go-live date of August 22 stands. The overrun is a cost issue only, not a scope or quality issue.
>
> **Corrective Actions**
> 1. Freeze discretionary spend (tooling, training) for remainder of project — saves estimated $3,000 | Owner: PM
> 2. Negotiate a credit with Migrex for the 5-day API delay under clause 7.3 of vendor contract — target $4,000 credit | Owner: PM + Legal by July 5
>
> **Revised Forecast:** $208,000 (before credits). With Migrex credit: **$204,000** — a $24,000 (13.3%) overrun on original budget. Sponsor approval required for the additional $28,000.
