# Prompt 01 — Sprint Planning Agenda

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Build a structured sprint planning meeting agenda with timeboxed sections, pre-read requirements, and facilitator notes — so every participant knows what to prepare and the meeting runs on time.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Sprint [N] planning for [project name]. Team size: [N]. Sprint duration: [2 weeks]. Ceremony duration: [2–4 hours]. Known priorities heading into this sprint: [top 2–3 themes from backlog]. Carryover from last sprint: [items]. |
| **Role** | You are an experienced Scrum Master who runs planning sessions that start on time, stay focused, and end with the team confident in their sprint commitment. |
| **Instruction** | Write a sprint planning agenda with: pre-meeting prep section, timebox per agenda item, facilitator notes for each section, and a clear close that confirms the sprint goal. |
| **Spec** | Agenda format. Each item has: title, timebox, facilitator, pre-read/prep required, and brief notes. Total duration must equal the ceremony duration provided. 300–350 words. |
| **Performance** | A substitute Scrum Master could run this session with no other briefing. Every section has a clear output. The agenda closes with a committed sprint goal statement. |

---

## Full Prompt

```
Context: I'm running Sprint [N] planning for [Project Name]. Team: [N developers, N QA, N designers]. Sprint duration: 2 weeks (starts [date], ends [date]). Ceremony timebox: [2 / 3 / 4 hours]. 

Top backlog priorities coming into this sprint:
1. [Priority 1 — e.g., "Complete user authentication module (4 stories, partially done)"]
2. [Priority 2 — e.g., "Start dashboard MVP (6 stories, designs ready)"]
3. [Priority 3 — e.g., "Bug bash — resolve top 5 open P2 bugs"]

Carryover from last sprint: [describe, or "none"]
Team velocity last sprint: [N story points]
Capacity this sprint: [N — note any leave or constraints]

Role: Act as an experienced Scrum Master who facilitates sprint planning sessions that run on time, keep the team engaged, and close with a clear, confident sprint commitment.

Instruction: Write a sprint planning agenda with:
1. Pre-meeting prep section (what each role needs to bring/prepare)
2. Agenda items with timebox, facilitator, and brief facilitator notes
3. A section for team capacity check
4. Story point estimation round
5. Sprint goal statement section
6. Close and parking lot

Spec:
- Agenda table format (item | timebox | facilitator | notes)
- Total timebox must match the ceremony duration provided
- Pre-meeting prep listed separately at the top
- 300–350 words
- Close must output a draft sprint goal statement

Performance bar: A substitute Scrum Master could run this session with no other context. Every section has a clear output. Agenda closes with a committed sprint goal the team co-owns.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Create a sprint planning agenda for a 2-week sprint.

**Output produced:**
> Sprint Planning Agenda: 1. Welcome (5 min) 2. Review backlog (30 min) 3. Assign tasks (30 min) 4. Any other business (10 min) 5. Close.

**Why it's weak:** No timeboxes that add up to anything, no facilitator notes, no pre-read prep, no capacity check, no sprint goal, no team size context. A real sprint planning with this agenda would run over by 90 minutes.

---

## After Example (With CRISP)

**Placeholders filled:**
- Sprint 14 | 6 devs, 2 QA, 1 designer | Starts Mon Jun 30 | 3-hour ceremony
- Priorities: Auth module completion, dashboard MVP start, P2 bug bash
- Carryover: 2 auth stories (DEV-441, DEV-443) totalling 8 points
- Last sprint velocity: 42 points | This sprint capacity: 38 (one dev on leave Wed–Fri)

**Output produced:**

> **Sprint 14 Planning — Monday 30 June | 09:00–12:00 UTC**
>
> **Pre-Meeting Prep (complete before 09:00)**
> - **PO:** Top 10 backlog items groomed, acceptance criteria written, designs linked
> - **Dev Lead:** Carryover tickets DEV-441 and DEV-443 re-estimated
> - **Team:** Confirm individual capacity (leave, meetings, on-call) in the capacity sheet
> - **QA:** Flag any stories from last sprint still needing regression sign-off
>
> **Agenda**
>
> | Item | Timebox | Facilitator | Notes |
> |------|---------|-------------|-------|
> | Welcome + Sprint 13 recap (1 slide) | 10 min | Scrum Master | Show velocity, highlight what shipped, acknowledge carryover — no post-mortem here |
> | Capacity check | 10 min | Scrum Master | Fill in team capacity table; confirm 38-point ceiling given leave |
> | Sprint goal draft | 15 min | PO + SM | PO proposes goal; team shapes it together; write it on the board |
> | Backlog walkthrough — Priority 1 (Auth module) | 30 min | PO | PO walks stories; team asks clarifying questions; no estimation yet |
> | Backlog walkthrough — Priority 2 (Dashboard MVP) | 20 min | PO | Same format; designs must be visible for all stories |
> | Backlog walkthrough — Priority 3 (Bug bash) | 15 min | PO | Quick review of 5 P2 bugs; confirm they're reproducible |
> | Story point estimation | 35 min | Scrum Master | Planning poker, 2 rounds per story; skip stories missing acceptance criteria |
> | Sprint backlog commit | 10 min | Scrum Master | Team confirms total points vs capacity; PO acknowledges trade-offs |
> | Sprint goal finalise + close | 10 min | Scrum Master | Read sprint goal aloud; team says yes/no to committing; log in Jira |
> | Parking lot / AoB | 5 min | All | Time-box strictly |
>
> **Draft Sprint Goal:** "Ship a working user authentication flow end-to-end and complete the first two dashboard MVP stories, with all P2 bugs from Sprint 13 resolved and regression-tested."
