# Prompt 10 — Project Closure Report

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Write a project closure report that formally closes the project, captures what was delivered, documents lessons learned honestly, and gives the organisation something useful for the next similar project — not a self-congratulatory summary that buries the hard truths.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Project [name] is complete. Original objectives: [list]. What was actually delivered: [list]. Timeline: originally planned vs actual. Budget: planned vs actual. Team: [list]. |
| **Role** | You are a PM who writes closure reports that future PMs will actually read — because they are honest, specific, and contain lessons that prevent real mistakes from repeating. |
| **Instruction** | Write a project closure report with: executive summary, deliverables vs original objectives, timeline performance, budget performance, lessons learned (positive and negative), and recommendations for future projects. |
| **Spec** | Formal document format with numbered sections. Lessons learned must include both what went well AND what didn't, with equal space. Recommendations must be actionable by a future PM. 450–500 words. |
| **Performance** | A PM starting a similar project 12 months from now should find at least 3 things in this document that change how they run their project. Lessons learned are honest, not political. |

---

## Full Prompt

```
Context: Project [Name] has reached closure. Please write a project closure report using the following information:

Original Objectives:
1. [Objective 1 with measurable criterion]
2. [Objective 2]
3. [Objective 3]

What Was Actually Delivered:
- [Deliverable 1 — note any gap vs original objective]
- [Deliverable 2]
- [Deliverable 3]

Timeline:
- Planned start: [date] | Actual start: [date]
- Planned go-live: [date] | Actual go-live: [date]
- Variance: [N days over/under]

Budget:
- Approved: $[X] | Actual: $[Y] | Variance: $[Z] ([%])

Team: [list members and roles]
Sponsor: [name]

Lessons Learned (raw notes — you synthesise):
Positive: [what worked well]
Negative: [what didn't work / what you'd do differently]

Role: Act as a PM who writes closure reports that future PMs actually find useful — because they contain honest, specific lessons that prevent real mistakes from repeating, not just a list of accomplishments.

Instruction: Write a project closure report with:
1. Executive Summary — 3 sentences: what was delivered, how it performed vs plan, one headline lesson
2. Deliverables vs Objectives — table comparing original objective to actual delivery
3. Timeline Performance — planned vs actual with brief explanation of variance
4. Budget Performance — planned vs actual with brief explanation
5. What Worked Well — 3 specific lessons (not generic praise)
6. What to Do Differently — 3 honest lessons with specific recommendations for future projects
7. Recommendations for Future Projects — 3 actionable recommendations with the audience who should read them

Spec:
- Formal document format, numbered sections
- 450–500 words
- Lessons must be equally balanced positive and negative
- Recommendations must address a named future audience ("Future PMs should...", "Procurement should...")
- No political softening — write the hard truths

Performance bar: A future PM reads this and changes at least 3 things about how they run their next project. Lessons are specific enough to be actionable, not generic mantras.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a project closure report for our CRM migration.

**Output produced:**
> The CRM migration project has been completed successfully. The team worked hard and delivered the project. We learned many valuable lessons. The project will benefit the organisation going forward. Thank you to all team members.

**Why it's weak:** No specifics, no actual lessons, "worked hard" is filler, "valuable lessons" without stating them is useless. This document would help no future PM with anything.

---

## After Example (With CRISP)

**Output produced:**

> **PROJECT CLOSURE REPORT — Atlas CRM Migration**  
> Prepared by: James Reid (PM) | Date: August 30, 2025 | Sponsor: Raj Patel (CMO)
>
> **1. Executive Summary**  
> Atlas CRM Migration delivered all three primary objectives — 120,000 contacts migrated with zero data loss, sales team operational in HubSpot within 5 days of go-live, and Salesforce licencing costs eliminated from September 1. The project closed 7 days late (August 22 vs planned August 15) and 15.6% over budget ($208,000 vs $180,000), driven by unplanned data remediation and a vendor API delay. The headline lesson: data quality in legacy systems is almost always worse than scoped; future migrations should include a paid discovery phase before finalising estimates.
>
> **2. Deliverables vs Objectives**
>
> | Objective | Target | Achieved |
> |-----------|--------|----------|
> | Migrate contacts with zero data loss | 120,000 records | 120,000 records — 4,200 required manual remediation |
> | Sales team operational post go-live | Within 5 days | Day 3 — exceeded target |
> | Licencing cost reduction | $2,800/month from Sep 1 | $2,800/month — met exactly |
>
> **3. Timeline Performance**  
> Planned go-live: August 15. Actual: August 22. Variance: +7 days. Root cause: data remediation added 5 days; vendor API delay added 2 additional days of standby.
>
> **4. Budget Performance**  
> Approved: $180,000. Actual: $204,000 (after Migrex $4,000 credit). Variance: +$24,000 (+13.3%). Root causes: data remediation ($18,000) and vendor standby costs ($6,000).
>
> **5. What Worked Well**
> - **Pair programming on complex migration scripts:** All paired scripts shipped with zero bugs. Strongly correlated with QA pass rate.
> - **Daily vendor check-ins once delay risk emerged:** Escalation was handled in 48h rather than a week. Early frequency was the differentiator.
> - **In-scope/out-of-scope table in kickoff brief:** Prevented mobile app scope creep from being approved (CMO request rejected at Week 6 cleanly, with documentation).
>
> **6. What to Do Differently**
> - **Conduct a paid 2-week data quality discovery phase before estimating migration work.** We underscoped by $18,000 because we couldn't see legacy data quality until we were inside the project. Future PMs: this is not optional on migrations.
> - **Require vendor API in a testable state 3 weeks before integration — not 1 week.** A 1-week buffer leaves no recovery time. Migrex's delay had no buffer and cost $6,000.
> - **Assign a dedicated data remediation resource, not a shared developer.** Using the main dev team for remediation blocked sprint progress twice.
>
> **7. Recommendations for Future Projects**
> - **Future PMs running migrations:** Budget a data quality discovery phase (2 weeks, $8,000–12,000) before finalising estimates. Add it to the standard migration project template.
> - **Procurement team:** Add a "testable API by [date]" SLA to all vendor contracts for integration projects. Clause 7.3 in our contract only covered late delivery, not "untestable" delivery.
> - **Portfolio team:** Create a migration project template using this project's RACI, scope table, and risk register as starting points.
