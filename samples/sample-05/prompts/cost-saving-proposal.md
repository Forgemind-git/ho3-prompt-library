# Prompt 05 — Cost-Saving Proposal

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Write a cost reduction proposal with a clear business case, quantified savings, implementation plan, and risk assessment — so the decision-maker can approve or reject it based on analysis, not instinct.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Company: [name]. Current annual spend in the category: $[X]. Proposed reduction: $[Y] ([%]). Method: [how the cost will be reduced — vendor renegotiation, process change, automation, headcount restructure, etc.]. Implementation time: [weeks/months]. |
| **Role** | You are a financial analyst making a business case for cost reduction — you present the savings clearly but you also surface the risks and trade-offs, because a proposal that ignores risks loses credibility. |
| **Instruction** | Write a cost-saving proposal with: current state cost analysis, proposed saving and method, implementation plan with timeline, risk assessment, and a recommendation with decision required. |
| **Spec** | Business case format. 350–400 words. Savings quantified as annual run-rate. Implementation plan as a timeline. Risks table with likelihood and mitigation. Decision required clearly stated at the end. |
| **Performance** | Decision-maker can approve or reject in a 15-minute meeting. The risk section is honest — no proposal should ignore downside. One clear decision requested at the end. |

---

## Full Prompt

```
Context: I'm a financial analyst at [Company Name] proposing a cost reduction initiative in [cost category — e.g., "software licencing", "vendor consolidation", "travel and expenses", "headcount restructuring"]. 

Current state:
- Annual spend in this category: $[X]
- Current arrangement: [describe — who we pay, for what, for how long]
- Number of users/beneficiaries: [N]

Proposed saving:
- Annual saving: $[Y] ([%] reduction)
- Method: [describe how — e.g., "renegotiate vendor contract", "consolidate 3 tools into 1", "move to usage-based pricing", "automate process currently requiring 0.5 FTE"]
- Implementation cost (one-time): $[Z or "none"]
- Time to first saving: [immediate / 30 days / 3 months]
- Time to full run-rate saving: [date]

Known risks or trade-offs:
1. [Risk 1 — e.g., "Vendor may not agree to renegotiation — risk: no saving achieved"]
2. [Risk 2 if applicable]

Decision needed from: [CFO / CEO / Procurement / Board]
Decision deadline: [date]

Role: Act as a financial analyst making a cost reduction business case. You are credible because you surface risks honestly — a proposal that ignores trade-offs loses the CFO's trust.

Instruction: Write a cost-saving proposal with:
1. Executive Summary — saving amount, method, timeline (3 sentences)
2. Current State Analysis — what we currently spend and why
3. Proposed Saving — the saving, how it's achieved, and what changes
4. Implementation Timeline — 4–6 milestones from approval to full run-rate saving
5. Risk Assessment — table with 2–3 risks, likelihood, and mitigation
6. ROI Summary — payback period if there is an implementation cost
7. Decision Required — exactly what you need approved, from whom, by when

Spec:
- Business case format
- 350–400 words
- Savings as annual run-rate
- Risk table with likelihood and mitigation
- One specific decision requested at the end
- Not a presentation — a written proposal

Performance bar: CFO can approve or reject in a 15-minute meeting. Risk section is honest. Decision required is specific.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a proposal to save money on software.

**Output produced:**
> We could save money by reviewing our software subscriptions. Many companies pay for tools they don't use. By auditing our tools, we could potentially save significant amounts. I recommend we do a software audit and cancel unused subscriptions.

**Why it's weak:** No numbers, "potentially save significant amounts" is meaningless, "software audit" is the first step not a proposal, no implementation plan, no risk assessment. This is an idea, not a business case.

---

## After Example (With CRISP)

**Placeholders filled:**
- Category: SaaS software consolidation (3 project management tools → 1)
- Current spend: $84,000/year across Asana, Notion, Monday.com (overlapping use cases)
- Proposed: Standardise on Notion ($28,000/year for same user count)
- Implementation cost: $0 (migration by internal ops team)
- Risk: Team resistance to tool change, migration time

**Output produced:**

> **Cost-Saving Proposal — SaaS Software Consolidation**  
> Prepared by: James Reid, Financial Analyst | Date: June 27, 2025  
> Decision Required from: CFO | By: July 10, 2025
>
> **Executive Summary**  
> Helply currently pays **$84,000/year** for three overlapping project management tools with significant user overlap. Consolidating onto Notion (already our second-largest tool by user count) would reduce this to **$28,000/year — a saving of $56,000 annually** (67% reduction). Full run-rate savings would be achieved by September 1, 2025.
>
> **Current State**  
> Helply has three active SaaS project management licences:
> - Asana (Business): $38,000/year — used by 42 users, primarily engineering
> - Monday.com (Pro): $26,000/year — used by 28 users, primarily operations
> - Notion (Plus): $20,000/year — used by 65 users across all teams
>
> User surveys (conducted June 2025) show 61% of Asana users and 73% of Monday users also have active Notion accounts. The three tools are performing overlapping functions.
>
> **Proposed Saving**  
> Upgrade Notion to Business tier ($28,000/year for 120 users) and consolidate all project management onto Notion. Cancel Asana and Monday.com contracts at renewal. Net annual saving: **$56,000**.
>
> **Implementation Timeline**
> - Jul 10: CFO approval
> - Jul 15: IT sets up Notion Business workspace + templates
> - Jul 21–31: Operations migrates Monday.com boards
> - Aug 1–15: Engineering migrates Asana projects
> - Aug 31: Monday.com and Asana contracts cancelled at renewal
> - Sep 1: Full run-rate saving achieved
>
> **Risk Assessment**
>
> | Risk | Likelihood | Mitigation |
> |------|-----------|------------|
> | Team resistance to Notion migration | Medium | Ops team runs 2 training sessions + creates migration templates; Asana/Monday maintained through August as parallel run |
> | Productivity loss during migration | Low | Migration planned in low-volume period (August); team leads set migration schedule |
> | Notion Business tier insufficient for needs | Low | Notion Business supports all current Asana/Monday features used in survey; validated with tool comparison |
>
> **ROI Summary**  
> Implementation cost: $0 (internal ops time estimated 20 hours). Payback: immediate. Annual saving: $56,000 from September 1.
>
> **Decision Required**  
> Approve consolidation plan and authorise Operations team to begin Notion Business upgrade and migration plan by July 15. CFO sign-off required for contract cancellation authority.
