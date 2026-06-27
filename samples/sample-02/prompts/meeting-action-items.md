# Prompt 05 — Meeting Action Items

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Extract and structure action items from raw meeting notes into a formatted table with clear ownership, deadlines, and dependencies — so nothing falls through the cracks and every attendee leaves knowing exactly what they're responsible for.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Meeting: [type and name]. Date: [date]. Attendees: [list]. Duration: [X minutes]. Raw notes pasted below. |
| **Role** | You are a chief-of-staff-calibre note taker who never lets an action item get lost and always assigns a specific owner — never "the team." |
| **Instruction** | Extract all action items from the notes, assign a specific owner per item, set a deadline based on context clues or urgency, flag dependencies, and surface any decision that was made but not documented. |
| **Spec** | Action items in a table: action | owner | deadline | depends on | status. Decisions in a separate section. 250 words max. One person per action — never "everyone" or "the team." |
| **Performance** | Every person in the meeting can identify their own actions in under 10 seconds. No action is vague enough to be misinterpreted. All decisions made in the meeting are captured. |

---

## Full Prompt

```
Context: I'm documenting the outputs of a [meeting type — e.g., sprint review / project kickoff / vendor call] held on [date] for [project name]. Attendees: [list names and roles]. Meeting duration: [X minutes]. Raw notes are pasted below.

Role: Act as a chief-of-staff-level note taker who produces action item summaries where nothing falls through the cracks. Every action has exactly one named owner — never "the team" or "TBD."

Instruction: Read the raw notes below and:
1. Extract all action items (include any that were implied but not explicitly stated)
2. Assign one named owner per action (use attendee names from the list)
3. Set a deadline for each action — use context clues (e.g., "before the next sprint", "EOD Friday") and flag any items with no clear deadline as [NEEDS DATE]
4. Identify any dependencies between actions
5. Capture all decisions that were made in the meeting (even informal ones)
6. Flag any items where agreement was unclear or deferred

Spec:
- Action items in a table: Action | Owner | Deadline | Depends On | Status (Open)
- Decisions in a separate bulleted list
- Items with unclear ownership: flag as [OWNER NEEDED]
- 250 words maximum
- One person per action, always

Performance bar: Every attendee can find their actions in under 10 seconds. Nothing is vague. All meeting decisions are captured so there's no "I thought we decided..." next week.

--- RAW MEETING NOTES ---
[Paste your raw notes here]
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Extract action items from these meeting notes.

**Output produced:**
> Action items: 1. Follow up on the API issue. 2. Update the stakeholders. 3. Review the timeline. 4. The team should look at the vendor proposal.

**Why it's weak:** No owners, no deadlines, "the team should look at" assigns responsibility to nobody. These four items will all be "in progress" at the next meeting with no progress.

---

## After Example (With CRISP)

**Raw notes pasted:**
> "James said he'd check with the vendor about API rate limits by end of week. Priya will update the project plan once she hears back. We decided to push the UAT start date to July 14. Ravi needs to review the Airbyte docs and give us his assessment — we need it before the next status call on Thursday. Sarah mentioned she hasn't got sign-off from the legal team yet on the data processing agreement; James will chase legal tomorrow. No one picked up the training materials task from last week."

**Output produced:**

> **Meeting Action Items — Atlas CRM Migration | 27 Jun 2025**
> Attendees: James (PM), Priya (PO), Ravi (Dev Lead), Sarah (BA)
>
> **Action Items**
>
> | Action | Owner | Deadline | Depends On | Status |
> |--------|-------|----------|------------|--------|
> | Check with Migrex on API rate limit resolution | James | Fri 28 Jun | — | Open |
> | Update project plan with revised UAT start date (Jul 14) | Priya | Mon 1 Jul | Vendor confirmation from James | Open |
> | Review Airbyte docs and provide technical assessment | Ravi | Thu 3 Jul (before status call) | — | Open |
> | Chase legal team for data processing agreement sign-off | James | Mon 1 Jul | — | Open |
> | Pick up training materials task (carried from last meeting) | [OWNER NEEDED] | [NEEDS DATE] | — | Open |
>
> **Decisions Made**
> - UAT start date moved from July 9 to **July 14** (agreed by all)
> - Airbyte assessment to be presented at Thursday status call before any commitment
>
> **Flags**
> - Training materials task has no owner — assign at next standup
