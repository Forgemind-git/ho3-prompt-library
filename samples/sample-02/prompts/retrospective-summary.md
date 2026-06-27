# Prompt 04 — Retrospective Summary

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Synthesise raw retrospective notes (sticky notes, FigJam comments, Miro boards) into a structured summary with clear themes, voted actions, owners, and sprint-over-sprint tracking — so the retro produces change, not just conversation.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Sprint [N] retrospective for [project/team]. Format used: [Start/Stop/Continue / 4Ls / Mad-Sad-Glad]. Number of participants: [N]. Raw notes pasted below. |
| **Role** | You are a Scrum Master who turns retrospective sessions into durable improvement actions — not just a feel-good summary that gets forgotten by next sprint. |
| **Instruction** | Synthesise the raw notes into: top 3 themes per category, one "headline" insight, a voted action list (max 3 actions for next sprint), and a satisfaction score check. |
| **Spec** | Retrospective report format. Themes as grouped bullet points. Actions in a table with owner, success metric, and review sprint. 300–350 words. |
| **Performance** | The 3 actions can be turned into Jira tickets today. Each action has a measurable success criterion. The headline insight is one sentence a VP could quote. |

---

## Full Prompt

```
Context: I'm the Scrum Master for [Team Name / Project Name]. We just completed Sprint [N] retrospective with [N] participants. We used the [Start/Stop/Continue / Mad-Sad-Glad / 4Ls] format. Raw retrospective notes are pasted below.

Role: Act as a Scrum Master who synthesises retrospective notes into clear, action-oriented summaries that produce sprint-over-sprint improvement — not just documentation.

Instruction: Read the raw notes below and produce a retrospective summary with:
1. Headline Insight — one sentence that captures the single most important thing this team learned or confirmed this sprint
2. Key Themes — group the notes into 3–5 themes; for each theme: name, supporting points (2–3 bullets), category (positive / needs improvement)
3. Voted Actions — the top 3 improvements for next sprint, formatted as a table with: action, owner, success metric (how we'll know it worked), review date
4. Team Pulse — a one-sentence summary of overall team sentiment based on the notes
5. Carry Forward — any actions from last retro that were not completed

Spec:
- Retrospective report format
- Bold all section headers
- Actions in a table (not prose)
- Each action must have a measurable success criterion
- 300–350 words
- No corporate jargon — write like a human who was in the room

Performance bar: The 3 actions can be added to Jira as tickets this afternoon. Success metrics are measurable by next retro. The headline insight can be quoted in a team meeting.

--- RAW RETRO NOTES ---
[Paste all sticky notes or comments here, grouped by category if possible]
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Summarise our retrospective notes.

**Output produced:**
> The team discussed what went well and what could be improved. Key themes included communication and processes. The team will work on improving these areas in the next sprint.

**Why it's weak:** No specifics, no actions, no owners, "communication" is not a theme it's a category, "will work on improving" without a plan means nothing changes. This is a waste of the retro session.

---

## After Example (With CRISP)

**Raw notes pasted:**
> Start: Daily async standup in Slack instead of Zoom / Code reviews earlier in sprint / Sharing blockers sooner  
> Stop: Last-minute story additions from PO / Estimation without designs / Skipping QA sign-off to hit deadline  
> Continue: Pair programming on complex tickets / The new testing checklist / Friday demos

**Output produced:**

> **Sprint 14 Retrospective Summary — Team Atlas**
>
> **Headline Insight**  
> The team ships better work when QA is treated as a gate, not an afterthought — three of the last four P2 bugs came from stories where QA was skipped under deadline pressure.
>
> **Key Themes**
>
> *Needs Improvement*
> - **Late scope additions** — PO added 3 stories in week 2 without capacity discussion; disrupted focus for 2 devs for 1.5 days
> - **Estimation without designs** — 4 stories were estimated before designs were ready; all 4 needed re-estimation mid-sprint
> - **Async communication gaps** — blockers surfaced in standup rather than Slack channel; added 8–24h delays
>
> *Positive*
> - **Pair programming** — both tickets handled with pair programming shipped with zero bugs; team wants to expand this
> - **New testing checklist** — all QA-signed stories passed regression; the three bugs came from stories that bypassed it
>
> **Voted Actions**
>
> | Action | Owner | Success Metric | Review |
> |--------|-------|----------------|--------|
> | PO commits: no new stories after Day 3 of sprint without SM approval | Priya (PO) | Zero mid-sprint additions in Sprint 15 | Sprint 15 retro |
> | No story enters estimation without design link attached in Jira | Ravi (Dev Lead) | Zero undesigned stories estimated in Sprint 15 | Sprint 15 retro |
> | All blockers posted in #atlas-blockers within 2h of identification | Whole team | Channel post rate vs standup raise rate | Sprint 15 retro |
>
> **Team Pulse**  
> Energy is good and the team is proud of what shipped — frustration is process friction, not interpersonal, which is healthy and fixable.
>
> **Carry Forward from Sprint 13**  
> - Pair programming expansion (partially done — pair on 2 of 6 complex tickets; target 4 next sprint)
