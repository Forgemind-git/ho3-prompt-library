# Prompt 07 — Project Kickoff Brief

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Write a one-page project kickoff brief that aligns the project team and stakeholders on scope, objectives, team roles, constraints, and success criteria before Day 1 of delivery — eliminating the "I didn't know that was in scope" conversations that derail projects in Week 2.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | New project: [name and description]. Sponsor: [name]. Team: [roles and names]. Budget: [$X]. Timeline: [start – end]. Key constraints or dependencies: [list]. |
| **Role** | You are a PM who has started 20+ projects and knows that a weak kickoff is the leading cause of mid-project confusion. You write briefs that answer every question before it's asked. |
| **Instruction** | Write a project kickoff brief with: project summary, objectives and success criteria, team RACI, in-scope/out-of-scope table, timeline milestones, constraints, and first actions. |
| **Spec** | Single-page brief format. Objectives must have measurable success criteria. RACI must be a table. In/out-of-scope as side-by-side list. 400 words max. |
| **Performance** | A team member joining this project on Day 1 with no prior context should understand what we're building, their role, and what success looks like. No ambiguity in scope or responsibilities. |

---

## Full Prompt

```
Context: I'm the PM kicking off [Project Name] for [Organisation/Department]. 
- Project sponsor: [name and title]
- Project description: [2-sentence summary of what we're building and why]
- Team: [list names and roles]
- Budget: $[X]
- Timeline: Start [date] | Go-live [date] | Total duration: [N weeks/months]
- Key constraints: [e.g., "must use existing vendor contracts", "no new headcount", "launch before Q4 budget freeze"]
- Dependencies: [e.g., "requires IT infrastructure provisioned by Jul 1", "legal sign-off on data agreement"]
- Known risks at kickoff: [list 1–2]

Role: Act as a PM who has led 20+ project kickoffs and knows that clarity at the start saves weeks of rework in the middle. You write briefs that pre-answer every common confusion point.

Instruction: Write a project kickoff brief with exactly these sections:
1. Project Summary — 3 sentences: what, why, when
2. Objectives — 3 bullet points, each with a measurable success criterion
3. Team and Responsibilities — RACI table (Responsible / Accountable / Consulted / Informed) for the top 5 decision types
4. Scope — side-by-side table: In Scope | Out of Scope
5. Key Milestones — 4–5 milestone dates
6. Constraints and Dependencies — bulleted list
7. First Actions — top 3 things that must happen in Week 1, with named owners

Spec:
- Single-page brief format (dense but structured)
- RACI in a table
- In/Out of Scope side-by-side
- Objectives MUST have measurable criteria
- 400 words maximum

Performance bar: Day-1 team member understands what we're building, their role, and success criteria. The "Out of Scope" section prevents the top 3 scope creep conversations.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a project brief for a CRM migration project.

**Output produced:**
> Project Brief: CRM Migration. We will migrate our existing CRM to a new system. The project will involve multiple teams and stakeholders. The goal is to improve efficiency. The project will begin soon and end when complete.

**Why it's weak:** No objectives, no RACI, no scope boundaries, no timeline, no success criteria. "End when complete" is not a milestone. This brief creates more questions than it answers.

---

## After Example (With CRISP)

**Output produced:**

> **PROJECT KICKOFF BRIEF — Atlas CRM Migration**  
> Sponsor: Raj Patel (CMO) | PM: James Reid | Start: June 30, 2025 | Go-live: August 22, 2025
>
> **Project Summary**  
> Atlas CRM Migration replaces the legacy Salesforce instance with HubSpot Enterprise to reduce licencing costs and improve marketing integration. The project runs 8 weeks, from data audit through go-live, for a team of 8. Success means zero data loss, all 120,000 contacts migrated, and sales team operational in HubSpot by August 22.
>
> **Objectives**
> - Migrate 120,000 CRM records with zero data loss (validated by reconciliation report)
> - Sales team fully trained and logging activities in HubSpot within 5 days of go-live
> - Licencing cost reduction of at least $2,800/month from Day 1 (Salesforce contract ends Sep 1)
>
> **RACI**
>
> | Decision | PM | Dev Lead | CMO | Legal | IT |
> |----------|----|----------|-----|-------|-----|
> | Scope changes | A | C | I | I | I |
> | Technical architecture | C | A | I | — | R |
> | Data processing agreement | R | — | I | A | — |
> | Go/No-Go for UAT | A | R | C | — | C |
> | Go-live approval | C | C | A | C | R |
>
> **Scope**
>
> | In Scope | Out of Scope |
> |----------|--------------|
> | Contact + deal migration | Mobile app companion |
> | HubSpot email integration | Custom reporting layer |
> | Sales team training (5 sessions) | Marketing automation rebuild |
> | Data validation report | Legacy Salesforce archiving |
>
> **Key Milestones**
> - Data audit complete: July 7
> - API integration: July 9
> - UAT kick-off: July 14
> - UAT sign-off: August 8
> - Go-live: August 22
>
> **Constraints**
> - Must use existing HubSpot Enterprise contract (no new licences)
> - No additional headcount approved
> - Legal sign-off required before any data transfer begins
>
> **Week 1 Actions**
> 1. IT provisions HubSpot staging environment — Owner: Dev Lead (Ravi) | Due: Jul 1
> 2. Legal signs data processing agreement — Owner: PM chase, Legal sign-off | Due: Jul 2
> 3. Data audit begins — Owner: BA (Sarah) | Due: Jul 1 start
