# Prompt 03 — Risk Register Entry

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Document a newly identified project risk with structured impact assessment, likelihood rating, risk score, mitigation plan, contingency plan, and a named owner — so the risk register is actionable, not just a list of worries.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Project [name] has a new risk: [describe the risk]. Current project phase: [planning / development / testing / go-live]. If this risk materialises, the impact would be [describe]. |
| **Role** | You are a PM with a PMI/PRINCE2 background who writes risk register entries that are specific enough to act on — not vague enough to ignore. |
| **Instruction** | Create a risk register entry with: risk ID, category, description, likelihood score (1–5), impact score (1–5), risk score (L x I), mitigation plan, contingency plan, owner, and review date. |
| **Spec** | Risk register row format — use a table for the structured fields, followed by narrative sections for mitigation and contingency. Risk scoring must follow a standard 1–5 scale with definitions provided. |
| **Performance** | The risk owner should be able to start the mitigation this week using only this entry. The contingency plan is specific enough to execute if the risk materialises. |

---

## Full Prompt

```
Context: I'm the PM for [Project Name], currently in [phase: planning / development / testing / go-live]. A new risk has been identified: [describe the risk in one sentence]. If this risk occurs, the impact would be: [describe — e.g., "delay go-live by 3–4 weeks and increase costs by approximately $15,000"]. Known early warning signs: [describe any signals that suggest this risk is starting to materialise, or "none identified yet"].

Role: Act as a PM with a PMI/PRINCE2 background who writes risk register entries that are specific, action-oriented, and immediately usable by the risk owner.

Instruction: Write a full risk register entry with:
1. Risk ID (generate a placeholder: RISK-XXX)
2. Risk Category (schedule / budget / resource / technical / external / compliance)
3. Risk Description — 2–3 sentences with full context
4. Likelihood Score — rate 1–5 with brief justification (1=rare, 3=possible, 5=almost certain)
5. Impact Score — rate 1–5 with brief justification (1=negligible, 3=significant, 5=project-threatening)
6. Risk Score — Likelihood x Impact (with severity label: Low 1–8 / Medium 9–15 / High 16–25)
7. Mitigation Plan — 3 specific actions to reduce likelihood or impact, with owner per action
8. Contingency Plan — what we do if the risk materialises despite mitigation
9. Risk Owner — named individual responsible for monitoring and mitigation
10. Review Date — next checkpoint to re-assess

Spec:
- Structured fields in a table
- Mitigation and Contingency as numbered lists
- Each mitigation action has a named owner
- 300–350 words
- No vague language ("monitor the situation" without specifics)

Performance bar: The risk owner can start mitigation this week. The contingency plan is executable as-written if the risk fires. A PMO audit would not flag this entry as incomplete.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Add a risk to our risk register about the third-party vendor being late.

**Output produced:**
> Risk: Third-party vendor may be late. Likelihood: Medium. Impact: High. Mitigation: Follow up with vendor regularly. Owner: PM.

**Why it's weak:** No scoring definitions, no risk score, "follow up regularly" is not a mitigation plan, "PM" as owner for everything removes accountability, no contingency. This is a worry list, not a risk register.

---

## After Example (With CRISP)

**Placeholders filled:**
- Project: Atlas CRM Migration
- Phase: Development
- Risk: The vendor providing the data migration API may not complete their endpoint by the Jul 5 deadline
- Impact: Delay go-live by 3 weeks, cost overrun of approximately $8,000
- Early warning signs: Vendor missed last two check-in calls; their test environment has been down for 48 hours

**Output produced:**

> **Risk Register Entry**
>
> | Field | Value |
> |-------|-------|
> | **Risk ID** | RISK-014 |
> | **Category** | External / Technical |
> | **Project** | Atlas CRM Migration |
> | **Phase** | Development |
> | **Date Identified** | 2025-06-27 |
> | **Risk Owner** | Sarah Tan (Technical Lead) |
> | **Review Date** | 2025-07-01 |
>
> **Risk Description**  
> The third-party vendor (Migrex Ltd) is contracted to deliver the data migration API endpoint by July 5. As of June 27, the vendor has missed two scheduled check-in calls and their test environment has been offline for 48+ hours. If the endpoint is not delivered by July 5, data migration cannot begin and go-live will slip from August 15 to approximately September 5.
>
> **Risk Scoring**
>
> | | Score | Justification |
> |-|-------|---------------|
> | **Likelihood** | 4 / 5 | Vendor has already missed two check-ins; test environment down suggests internal delay |
> | **Impact** | 4 / 5 | 3-week go-live delay + ~$8,000 cost overrun from extended team time |
> | **Risk Score** | **16 / 25 — HIGH** | Immediate escalation required |
>
> **Mitigation Plan**
> 1. **Formal written escalation to Migrex account director by Jun 28** — include contractual deadline and late-delivery clause reference | Owner: PM (James Reid)
> 2. **Schedule daily 15-min check-in with Migrex technical lead starting Jun 29** | Owner: Sarah Tan
> 3. **Evaluate open-source migration alternative (Airbyte) as parallel track by Jul 1** | Owner: Dev Lead (Ravi Kumar)
>
> **Contingency Plan**  
> If the Migrex API is not in a testable state by July 3 (48h before deadline): activate Airbyte parallel track; PM to notify sponsor same day and present revised go-live date; procurement to issue formal notice of breach per Section 8.2 of vendor contract.
