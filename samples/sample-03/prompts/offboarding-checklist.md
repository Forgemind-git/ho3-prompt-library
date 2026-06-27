# Prompt 07 — Offboarding Checklist

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Create a structured, comprehensive offboarding plan for a departing team member that protects knowledge continuity, ensures proper access revocation, and treats the person with dignity — so they leave as an ambassador, not a critic.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team member departing: [name, role, tenure]. Last day: [date]. Notice period: [2 weeks / 1 month]. Reason for departure: [resignation / redundancy / end of contract]. Key knowledge/systems they own: [list]. Replacement plan: [hired / in progress / not yet]. |
| **Role** | You are a manager who runs offboarding as professionally as onboarding — because how you handle departures shapes your team culture and your employer brand. |
| **Instruction** | Create an offboarding checklist with: knowledge transfer tasks, system access revocation list, HR and admin tasks, team communication plan, and a personal appreciation touchpoint. |
| **Spec** | Checklist format with timeline (Day 1–14 or Day 1–30). Each item has: task, owner, due date slot. Grouped by category. 350–400 words. Must include a "how are they leaving?" culture moment. |
| **Performance** | Day 1 of the person's absence, their replacement (or team) has everything they need to continue without disruption. The departing person tells their next employer good things about how they were treated. |

---

## Full Prompt

```
Context: I'm managing the offboarding of [Team Member Name], a [role] who has been with the company [tenure]. Their last day is [date]. Notice period: [2 weeks / 1 month]. Reason for departure: [voluntary resignation / redundancy / end of contract / other]. 

Key knowledge/systems/relationships they own:
- [Item 1 — e.g., "Primary owner of the payment integration codebase"]
- [Item 2 — e.g., "Main contact for Vendor X account"]
- [Item 3 — e.g., "Only person who knows the legacy data migration script"]

Replacement status: [Replacement hired and starts [date] / Hiring underway / Work redistributed to team]

Role: Act as a manager who treats offboarding as seriously as onboarding — because how someone leaves shapes team culture and your employer brand.

Instruction: Create a structured offboarding plan with these sections:
1. Knowledge Transfer — specific sessions, documents, and handover meetings needed; who receives the knowledge
2. System Access Revocation — list of systems to revoke, with IT as owner and a final-day deadline
3. HR and Admin — payroll, benefits, equipment return, reference letter, exit interview
4. Team Communication — how and when to communicate the departure to the team and stakeholders
5. Culture Moment — how you'll mark their departure with genuine appreciation (team farewell, written note, recommendation)

Spec:
- Checklist format with timeline (day-relative, e.g., "Day 1", "Day 5", "Final Day")
- Each item: task | owner | timeline
- Grouped by category with headers
- 350–400 words
- Must include one specific culture/appreciation touchpoint

Performance bar: Day 1 after their departure, the team has what they need. The departing person tells their next employer they were treated well. Nothing falls through the cracks.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Create an offboarding checklist for a departing employee.

**Output produced:**
> 1. Return equipment. 2. Revoke access. 3. Exit interview. 4. Knowledge transfer. 5. Say goodbye.

**Why it's weak:** No ownership, no timeline, "knowledge transfer" is a category not a task, "say goodbye" is not a plan. The payment integration would be orphaned on Day 1 of their absence.

---

## After Example (With CRISP)

**Placeholders filled:**
- Ana Sousa, Senior Developer, 2 years, last day August 15 (1-month notice)
- Owns: payment integration codebase, Migrex vendor relationship, async queue pattern documentation
- Replacement: Kenji (junior dev) absorbing payment work; new senior hire starting September

**Output produced:**

> **Offboarding Plan — Ana Sousa | Last Day: August 15, 2025**
>
> **Knowledge Transfer**
>
> | Task | Owner | Timeline |
> |------|-------|----------|
> | Document payment integration architecture (Confluence) | Ana | By Jul 25 |
> | 2x pair sessions with Kenji on payment codebase | Ana + Kenji | Jul 28 + Aug 4 |
> | Record Loom walkthrough of async queue failure pattern | Ana | By Aug 1 |
> | Intro Migrex account team to James as primary contact | Ana + James | By Aug 8 |
> | Review all open PRs and add documentation comments | Ana | By Aug 12 |
> | Final questions session with full Backend team | Ana | Aug 14 |
>
> **System Access Revocation (Final Day)**
>
> | System | Owner |
> |--------|-------|
> | GitHub org access | IT |
> | AWS IAM roles (prod + staging) | IT + DevOps |
> | Jira + Confluence | IT |
> | Vendor portal (Migrex) | IT + James |
> | Slack workspace | IT |
> | Google Workspace (drive, email) | IT |
>
> **HR and Admin**
>
> | Task | Owner | Timeline |
> |------|-------|----------|
> | Exit interview scheduled | HR | By Aug 8 |
> | Final payslip and benefits close | HR | By Aug 15 |
> | Laptop return | Ana + IT | Aug 15 |
> | Written reference letter | James | By Sep 1 |
>
> **Team Communication**
> - Internal announcement: James shares news with team at next standup (Jul 16) — Ana present, framed positively
> - External stakeholders: Ana sends personal email to Migrex contact with James CC'd (Aug 8)
>
> **Culture Moment**  
> Team farewell lunch Aug 14. James writes a personal LinkedIn recommendation before Ana's last day — no waiting to be asked. Recognition of her P1 fix and payment architecture leadership specifically named in team Slack.
