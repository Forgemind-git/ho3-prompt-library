# Prompt 02 — Stakeholder Status Update

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Write a concise, clearly-structured stakeholder status update that communicates RAG status, progress against milestones, risks on the horizon, and decisions needed — without overwhelming executives with detail or hiding problems in vague language.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Project [name], [week/sprint N]. RAG status: [Red/Amber/Green]. Key milestone status: [on track / delayed by X days / completed]. Risks to surface: [list]. Decisions needed from stakeholders: [list]. |
| **Role** | You are a senior PM who writes stakeholder updates that executives trust — because the updates are honest about risks and never bury bad news in positive framing. |
| **Instruction** | Write a weekly status update with: RAG indicator with one-sentence justification, 3-bullet progress summary, risks and issues section, decisions needed, and next milestones. |
| **Spec** | Email or Confluence update format. 200–250 words. RAG status in the subject line. No more than 5 bullets total. Decisions needed must be specific — not "input required." |
| **Performance** | An executive reads this in 90 seconds and knows: current status, what's at risk, and what they need to do. No follow-up questions about basic status. |

---

## Full Prompt

```
Context: I'm the PM for [Project Name]. This is the Week [N] / Sprint [N] status update. Audience: [executive sponsor / steering committee / department head]. 

Current status:
- RAG: [Red / Amber / Green] because [one-sentence reason]
- Milestone status: [list 2–3 milestones with on-track / delayed / completed]
- Progress this period: [3–4 bullet points of what was completed or advanced]
- Risks on the horizon: [list 1–3 risks with likelihood and impact]
- Blockers: [list any, or "none currently"]
- Decisions needed from stakeholders: [list specific decisions with deadlines]
- Next milestones: [what's coming in the next 2 weeks]

Role: Act as a senior PM who writes executive status updates that are honest, scannable, and always surface bad news clearly rather than burying it.

Instruction: Write a stakeholder status update with these exact sections:
1. Subject line with RAG status indicator
2. Status Summary (2–3 sentences max — the TLDR)
3. Progress This Period (3 bullets max)
4. Risks & Issues (each with: description, likelihood, mitigation owner)
5. Decisions Needed (each with: decision, needed by, consequences of delay)
6. Next Milestones (2–3, with dates)

Spec:
- Email format with subject line
- 200–250 words total
- RAG in subject line (use emoji: green circle, amber circle, red circle)
- 3 bullets max per section — force prioritisation
- Decisions must be specific and actionable

Performance bar: Executive reads this in 90 seconds and knows current status, top risk, and what action they need to take. No follow-up questions needed for basic status.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a project status update.

**Output produced:**
> Hi all, just wanted to give a quick update on the project. Things are progressing well. The team has been working hard on several deliverables. We have encountered some challenges but are working through them. Please let me know if you have any questions. More updates to follow.

**Why it's weak:** No RAG status, no specific progress, "challenges" without naming them, no decisions requested. An executive reading this has no idea if the project is on track. This update wastes everyone's time.

---

## After Example (With CRISP)

**Placeholders filled:**
- Project: Atlas CRM Migration
- Week 6 | Steering committee audience
- RAG: Amber — data migration taking 40% longer than estimated
- Milestones: Data audit complete; API integration delayed 5 days; UAT start on track
- Risks: vendor API rate limits, UAT resource availability, scope creep from marketing team

**Output produced:**

> **Subject: Atlas CRM Migration — Week 6 Status | AMBER**
>
> **Status Summary**  
> The project is AMBER. Data migration is progressing but running 40% slower than estimated due to unplanned data quality issues in the legacy system. API integration has slipped 5 days; UAT start date is not yet affected but will be if we lose another 3 days.
>
> **Progress This Period**
> - Data audit completed: 82,000 of 120,000 records validated; 4,200 flagged for manual remediation
> - API authentication layer built and tested in staging; rate-limit issue identified (see Risks)
> - UAT test plan drafted and signed off by QA lead
>
> **Risks & Issues**
> - **Vendor API rate limits** — vendor's staging API allows only 500 calls/hour vs 2,000 needed; owner: Dev Lead | mitigation: escalated to vendor account team, response expected by Fri
> - **UAT resource availability** — business analyst assigned to UAT is on leave Wk 8; owner: Sponsor | mitigation: identify backup resource by next Tuesday
>
> **Decisions Needed**
> - **Approve 5-day timeline buffer:** Needed by Friday. Without it, UAT start slips and go-live moves from Aug 15 to Aug 22.
>
> **Next Milestones**
> - Data migration complete: Jul 7 (was Jul 4)
> - API integration complete: Jul 9
> - UAT kick-off: Jul 14
