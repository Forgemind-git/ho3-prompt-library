# Prompt 06 — Scope Change Impact Note

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Document a scope change request with a clear assessment of timeline, cost, and risk implications — so stakeholders can make an informed decision to approve, reject, or defer the change rather than treating scope creep as "just one more thing."

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Project [name], currently [phase]. A scope change has been requested by [requester/stakeholder]. The requested change: [describe it]. The project's original scope, budget, and timeline: [summarise]. |
| **Role** | You are a PM who advocates for project integrity and always presents scope change requests with their full implications — never minimising impact to keep stakeholders happy in the short term. |
| **Instruction** | Write a scope change impact note that: describes the requested change clearly, assesses timeline impact (days/weeks), estimates cost impact, identifies risks introduced, recommends approval/rejection/deferral with rationale, and requests a sign-off decision. |
| **Spec** | Change request document format. 250–300 words. Sections: change description, impact assessment table, risk assessment, recommendation, sign-off required. Do not recommend approval unless the impacts are genuinely acceptable. |
| **Performance** | The decision-maker can approve or reject in a 10-minute meeting with no additional information needed. The impacts are stated precisely, not as ranges wider than 20%. |

---

## Full Prompt

```
Context: I'm the PM for [Project Name], currently in [phase]. A scope change has been requested by [requester — name and role]. Original project parameters: budget $[X], timeline end date [date], team [N people]. 

Change requested: [describe the addition or modification in detail]
Requester's stated reason: [why they want this]
Current project status: [on track / amber / delayed — briefly]

Role: Act as a PM who presents scope change impacts honestly — you never downplay the cost of scope changes to avoid conflict, because you know the project pays for it later.

Instruction: Write a scope change impact assessment with:
1. Change Description — clear restatement of what is being requested and why
2. Impact Assessment — table with: timeline impact (added days), cost impact (estimated $), team impact (who is affected and how), quality/risk impact
3. Risk if Approved — 1–2 risks this change introduces to the existing project
4. Risk if Rejected — 1 risk if the change is NOT made (be fair to the requester)
5. Recommendation — approve / reject / defer to Phase 2 — with a one-paragraph rationale
6. Decision Required — what needs to be signed off, by whom, and by when

Spec:
- Change request document format
- Impact in a table
- 250–300 words
- Recommendation must be clearly stated (not "it depends")
- Sign-off section with named approver

Performance bar: Decision-maker can approve or reject in a 10-minute meeting. No additional analysis needed. Impacts are specific, not vague ranges.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Document a scope change request to add a mobile app to our web project.

**Output produced:**
> The stakeholder has requested adding a mobile app to the project. This will require additional time and resources. The team should evaluate this and provide an estimate. Please review and decide accordingly.

**Why it's weak:** No impact numbers, no risk analysis, no recommendation, "the team should evaluate" defers the work back to the PM. This document helps nobody make a decision.

---

## After Example (With CRISP)

**Placeholders filled:**
- Project: Atlas CRM Migration | Phase: Development (Week 6 of 12)
- Requester: CMO (Raj Patel) — wants a mobile app companion for field sales reps
- Original: Budget $180,000 | Timeline: Aug 15 | Team: 5 devs, 1 QA, 1 designer
- Current status: Amber (data migration 5 days behind)

**Output produced:**

> **Scope Change Request — SCR-007**  
> **Project:** Atlas CRM Migration | **Date:** June 27, 2025 | **Requested by:** Raj Patel (CMO)
>
> **Change Description**  
> Addition of a mobile app (iOS + Android) companion for field sales reps to access CRM data, log calls, and update opportunity status offline. Not included in the original project scope, which covers web CRM only.
>
> **Impact Assessment**
>
> | Dimension | Impact |
> |-----------|--------|
> | Timeline | +10–12 weeks (go-live moves from Aug 15 to Oct 31 at minimum) |
> | Cost | +$42,000–$55,000 (mobile dev resource + app store setup + QA) |
> | Team | Requires 2 additional mobile developers not currently on the project |
> | Quality Risk | Core web CRM testing compressed to accommodate mobile timeline |
>
> **Risk if Approved**  
> Project is already Amber on data migration. Adding mobile scope now puts the entire delivery at High risk. Web go-live becomes a single-point dependency of mobile completion.
>
> **Risk if Rejected**  
> Field sales team lacks mobile access until a Phase 2 can be scoped (estimated Q1 2026). Productivity impact acknowledged but deferred.
>
> **Recommendation: DEFER to Phase 2**  
> The web CRM delivery is at risk even without additional scope. Approving mobile now will almost certainly push go-live past October and may destabilise the core deliverable. Recommend delivering the web CRM on the revised August 22 timeline, then scoping mobile as a funded Phase 2 starting September.
>
> **Decision Required**  
> Approver: CEO + CMO | Deadline: July 1 | Options: Approve (accept Oct 31 go-live + budget increase) / Reject / Defer to Phase 2 (recommended)
