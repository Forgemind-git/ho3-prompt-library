# Prompt 05 — PIP Outline

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Draft a Performance Improvement Plan (PIP) outline that defines the performance gap clearly, sets measurable improvement goals, establishes checkpoints, and documents the support the manager will provide — creating a fair, documented process that gives the employee a genuine opportunity to succeed.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team member: [name, role, tenure]. Performance gap: [describe specifically what is below expectations]. Documentation history: [what has been discussed previously — dates, conversations]. PIP duration: [30 / 60 / 90 days]. HR involvement: [HR reviewed / HR will review before delivery]. |
| **Role** | You are a manager working with HR to create a PIP that is fair, documented, and gives the employee a genuine path to success — not a paper trail for a predetermined outcome. |
| **Instruction** | Write a PIP outline with: performance gap statement, measurable improvement goals, weekly/bi-weekly check-in structure, manager support commitments, consequences if goals are not met, and sign-off section. |
| **Spec** | Formal HR document format. Goals must be SMART (Specific, Measurable, Achievable, Relevant, Time-bound). Consequences clearly stated — no vague "further action." 400–450 words. Note: always have HR review before delivering a PIP. |
| **Performance** | HR can approve this document without material changes. The employee understands exactly what they need to do, by when, and what happens if they don't. The manager's support commitments are concrete. |

---

## Full Prompt

```
Context: I'm a people manager creating a Performance Improvement Plan (PIP) for [Team Member Name], a [role] who has been with the company [tenure]. This document will be reviewed by HR before delivery.

Performance gap (be specific — what is below expectations and for how long):
[Describe the gap with 2–3 specific examples, including dates where possible]

Previous discussions (document the history):
[List prior feedback conversations, dates, and what was agreed]

PIP duration: [30 / 60 / 90 days]
Start date: [date]
End date: [date]

Role: Act as a manager working in good faith with HR to create a PIP that is fair and gives the employee a genuine opportunity to improve — not a document designed to make exit easier.

Instruction: Write a PIP outline with:
1. Purpose Statement — why this PIP is being issued and what outcome it aims for
2. Performance Gap — factual description of the gap with 2–3 documented examples
3. Improvement Goals — 3 SMART goals the employee must achieve during the PIP period
4. Check-In Schedule — weekly or bi-weekly check-in structure with what will be reviewed
5. Manager Support Commitments — concrete things you will do to support improvement
6. Consequences — clear statement of what happens if goals are met / partially met / not met
7. Signatures — employee, manager, HR sign-off section

Spec:
- Formal HR document format
- 400–450 words
- SMART goals: specific, measurable, achievable, relevant, time-bound
- Consequences must be explicit (not "further action may be taken")
- Manager commitments must be specific and actionable
- Note at top: "Draft for HR review — do not deliver without HR sign-off"

Performance bar: HR approves without material changes. Employee understands exactly what they need to do, by when, and what happens if they don't. Manager commitments are real.

IMPORTANT: This is a structured planning tool. Always have a qualified HR professional review any PIP before it is delivered to an employee.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a performance improvement plan for an underperforming employee.

**Output produced:**
> Performance Improvement Plan. Employee must improve their performance. Goals: 1. Be more productive. 2. Communicate better. 3. Meet deadlines. Duration: 90 days. Manager will check in regularly. If not improved, further action will be taken.

**Why it's weak:** "Be more productive" and "Communicate better" are not SMART goals. "Further action will be taken" is vague. "Check in regularly" is not a schedule. This document would not survive HR review.

---

## After Example (With CRISP)

**Placeholders filled:**
- Employee: David Kim, Software Developer, 14 months
- Gap: Code reviews consistently incomplete, 4+ missed PR deadlines in 8 weeks, feedback not incorporated
- History: Verbal feedback at 1:1 (Apr 15), written follow-up email (May 2), 1:1 review (Jun 10)
- Duration: 60 days

**Output produced:**

> **DRAFT — FOR HR REVIEW BEFORE DELIVERY**  
> **Performance Improvement Plan**  
> Employee: David Kim | Role: Software Developer | Manager: James Reid | HR: [Name]  
> PIP Period: July 1 – August 29, 2025
>
> **Purpose**  
> This PIP is issued to support David in meeting the performance expectations of the Software Developer role in the areas of code review completion and delivery commitments. The goal is for David to demonstrate sustained improvement in these areas by August 29, 2025.
>
> **Performance Gap**  
> Over the past 8 weeks (May–June 2025), David has:
> - Completed 3 of 11 assigned code reviews within the 24-hour SLA (vs team average of 9 of 11)
> - Missed 4 pull request deadlines by 2+ days without prior notification (PR-312, PR-318, PR-324, PR-331)
> - Received written feedback on code structure in May 2025; the same patterns recurred in June 2025 PRs without documented change
>
> These gaps were discussed verbally on April 15, in writing on May 2, and in a formal 1:1 review on June 10.
>
> **Improvement Goals**
>
> 1. **Code Review Completion:** Complete 90% of assigned code reviews within 24 hours of assignment during the PIP period (baseline: 27%). Measured weekly by team lead report.
>
> 2. **Delivery Commitments:** Zero sprint story misses without prior notification during the PIP period. "Prior notification" defined as flagging a blocker at least 24 hours before deadline in Jira or #dev-blockers Slack channel.
>
> 3. **Feedback Incorporation:** All written code review feedback incorporated within one revision cycle. Tracked by code review audit at 30-day and 60-day check-ins.
>
> **Check-In Schedule**  
> - Weekly 30-minute 1:1 with manager (Fridays) reviewing goal progress
> - Formal mid-PIP review at Day 30 (July 31) — written summary shared with HR
> - Final PIP review at Day 60 (August 29) — outcome decision
>
> **Manager Support Commitments**  
> - Pair David with senior developer for 2 code review sessions per week in July
> - Provide written examples of "acceptable" vs "below standard" code review feedback by July 5
> - Share weekly goal progress data so David can self-monitor
>
> **Consequences**  
> - Goals met by Aug 29: PIP closed; return to standard performance management
> - Partial progress: Extended PIP or role reassignment discussion with HR
> - Goals not met: Employment may be terminated. This decision will involve HR.
>
> **Signatures**  
> Employee: _________________ Date: _______  
> Manager: _________________ Date: _______  
> HR Representative: _________ Date: _______
