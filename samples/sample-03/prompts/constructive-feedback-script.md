# Prompt 03 — Constructive Feedback Script

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Write a specific, structured feedback script using the SBI (Situation–Behaviour–Impact) framework that prepares you for a real conversation about a behaviour that needs to change — not a script to read verbatim, but a guide that ensures you're clear, fair, and opening a dialogue.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team member: [name, role]. Behaviour to address: [describe the specific behaviour, not the person]. Situation: [when/where this happened]. Impact: [on team, project, stakeholders]. How many times has this happened: [once / a pattern]. |
| **Role** | You are a manager who gives feedback that lands — not because you're harsh, but because you are specific, fair, and give the other person a chance to respond before you draw conclusions. |
| **Instruction** | Write a feedback script using SBI structure: Situation (when/where), Behaviour (what they did — observable, not interpreted), Impact (what happened as a result), followed by a question to invite their perspective. |
| **Spec** | Script format, 200–250 words. Opening line should not start with "So I wanted to talk about..." SBI must be clearly separated. Script must end with an open question, not a demand. |
| **Performance** | You could deliver this script in a 1:1 with minimal prep. The behaviour described is specific enough that the team member cannot say "I don't know what you mean." The question at the end invites dialogue. |

---

## Full Prompt

```
Context: I'm a people manager preparing to give feedback to [Team Member Name], a [role], about [brief description of the behaviour — e.g., "frequently interrupting colleagues in meetings", "not flagging blockers until they become problems", "dismissive responses to junior team members"]. 

Specific incident(s):
- [Incident 1: date, situation, what they did, what happened as a result]
- [Incident 2 if applicable]

Pattern or one-off: [This is the first time I'm addressing it / This is a recurring pattern I've raised before / This is a first observation I want to address early]

My goal for this conversation: [inform them / understand their perspective / agree on a change / document before formal process]

Role: Act as a manager who gives feedback that lands because it is specific, fair, and opens a dialogue rather than delivering a verdict.

Instruction: Write a feedback script that follows the SBI structure:
1. Opening — 1–2 sentences to set the tone and context (not "So I wanted to chat...")
2. Situation — specific, factual description of when/where
3. Behaviour — what the person did, observable and non-judgmental (no "you were rude", instead describe what was said/done)
4. Impact — concrete effect on the team, project, or relationship
5. Check-in Question — an open question that invites their perspective before any conclusion is drawn

Spec:
- Script format (for manager delivery in a 1:1)
- 200–250 words
- Behaviour section: observable facts only, no personality judgements
- Must end with an open question
- Not a script to read verbatim — natural language

Performance bar: Deliverable in a 1:1 with minimal prep. Behaviour specific enough that "I don't know what you mean" is not a valid response. Ends with dialogue, not a verdict.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write feedback for an employee who keeps missing deadlines.

**Output produced:**
> "I've noticed that you have been missing deadlines recently. This is not acceptable and needs to improve. Please make sure to manage your time better and communicate if you are going to be late."

**Why it's weak:** No specific situation, "not acceptable" is a verdict not feedback, "manage your time better" is vague advice that doesn't address root cause. There's no question — just a demand. This script will create defensiveness, not change.

---

## After Example (With CRISP)

**Placeholders filled:**
- Team member: Marcus Webb, Product Designer
- Behaviour: Not raising blockers until they become missed commitments
- Incident 1: Marcus didn't flag that the design tool subscription lapsed until the day before handoff to dev — 2-day delay
- Incident 2: In sprint planning, he committed to 3 designs but didn't mention he hadn't received the content brief — missed all 3
- Pattern: First time addressing explicitly, but third time the pattern has occurred
- Goal: Understand his perspective and agree on a change

**Output produced:**

> **Feedback Script — Marcus Webb | 1:1 June 27**
>
> "Marcus, I wanted to make some time to talk through something I've been noticing — I want to share my perspective and hear yours, because I think there's something useful here for both of us.
>
> **Situation:** In sprint 13, you committed to delivering three UI designs by Friday. When Friday came, none were ready.
>
> **Behaviour:** When I looked back at the week, you hadn't flagged at any point during the sprint that you were missing the content brief those designs depend on. You had that information by Monday, but it didn't surface in standups, messages to the PO, or our 1:1 on Wednesday.
>
> **Impact:** The dev team lost two days waiting for designs. QA had to compress their timeline, and we ended up shipping one story without proper design review. That's the kind of thing that creates technical debt down the road.
>
> This is the third time I've seen a version of this pattern — a blocker you're aware of that doesn't surface until it becomes a missed commitment.
>
> Before I draw any conclusions, I'd really like to understand your experience: **what was going on from your side during that sprint, and what got in the way of flagging the missing brief earlier?**"
