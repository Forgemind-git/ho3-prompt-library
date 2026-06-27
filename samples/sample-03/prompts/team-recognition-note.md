# Prompt 04 — Team Recognition Note

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Write a specific, meaningful recognition note for an individual or team that names the exact contribution, explains why it mattered, and makes the person feel genuinely seen — not like they received a generic "great job" that took 30 seconds to write.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Recognising: [name(s) and role(s)]. What they did: [specific contribution or achievement]. Context: [what was difficult about it / what the stakes were]. Impact: [what it meant for the team, project, or customer]. Audience: [private 1:1 / team Slack / all-hands / peer nomination form]. |
| **Role** | You are a manager who knows that recognition lands differently when it is specific. You name what people actually did, not what you appreciate about them as a person. |
| **Instruction** | Write a recognition note that: names the specific achievement, describes what made it difficult or impressive, explains the real-world impact, and lands with genuine warmth — not corporate enthusiasm. |
| **Spec** | Format matches the audience (Slack post / email / spoken note). 100–150 words. The achievement must be named in the first sentence. No hollow openers like "I just wanted to take a moment to..." |
| **Performance** | The person who receives this knows you were paying attention. They could read it to their family and it would make sense. Other team members know what's being celebrated and why. |

---

## Full Prompt

```
Context: I want to recognise [Name(s)] for [brief description of what they did]. Here's the context:
- What they did: [be specific — not "did great work" but what they actually did]
- What made it impressive or difficult: [extra hours, technical challenge, stepping outside their role, crisis situation, etc.]
- The real impact: [what would have happened without their contribution / what it enabled / how it helped the team or customer]
- Audience: [private 1:1 / team Slack message / public all-hands shoutout / peer nomination form / manager feedback to HR]

Role: Act as a manager who gives recognition that lands because it is specific and genuine. You avoid hollow corporate enthusiasm and name what the person actually did.

Instruction: Write a recognition note that:
1. Names the specific achievement in the first sentence — no warm-up
2. Describes what made it impressive or hard (the context gives it meaning)
3. States the real impact (what it enabled or prevented)
4. Closes with genuine warmth appropriate to the relationship and audience
5. Avoids: "I just wanted to...", "amazing", "rockstar", "crushed it" and similar hollow language

Spec:
- Format appropriate to the audience provided
- 100–150 words
- Achievement named in sentence 1
- Impact is concrete, not vague ("the team could ship on time" not "we all benefited")
- Warmth without corporate hollowness

Performance bar: The recipient reads this and knows you were paying attention to their actual work. Other team members understand what's being celebrated. The note would make sense to someone who doesn't work here.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a recognition message for my employee who worked hard last week.

**Output produced:**
> "Shoutout to Sarah for all her hard work last week! You really went above and beyond and the team really appreciates everything you do. Keep up the amazing work! You're a rockstar!"

**Why it's weak:** No specific achievement named, "hard work" is vague, "rockstar" and "amazing" are hollow filler. Someone reading this doesn't know what Sarah did or why it mattered. Sarah doesn't feel genuinely seen.

---

## After Example (With CRISP)

**Placeholders filled:**
- Recognising: Ana Sousa (Senior Developer)
- What she did: Diagnosed and fixed a P1 production outage solo on a Saturday night, in under 2 hours
- Difficult because: Not her on-call rotation, she spotted the alert in personal time and jumped in
- Impact: 40,000 users would have been affected by morning; she prevented it silently while the team slept
- Audience: Team Slack

**Output produced:**

> "@anaSousa I want to call out something that happened Saturday night that most of the team didn't see.
>
> At 11:30pm, Ana noticed a misconfiguration alert in personal time — not her on-call rotation, not her obligation. She diagnosed the root cause, patched it, tested the fix, and had 40,000 user sessions back to normal by 1:15am. Then she wrote up a clear incident summary in #engineering so the Monday team had full context without needing to ask.
>
> Without that, we'd have woken up Monday morning to a full-scale incident.
>
> That kind of reliability — technical and personal — is what makes this team work. Thank you, Ana."
