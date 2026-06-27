# Prompt 10 — Difficult Conversation Script

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Write a script for a genuinely difficult management conversation — delivering news the person won't want to hear, addressing a sensitive situation, or navigating a conflict — that is honest, structured, and compassionate without being evasive.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Topic: [describe the difficult conversation — redundancy, not getting a promotion, behaviour pattern, performance, conflict]. Person: [role, tenure, relationship quality]. What they know going in: [nothing / some context / full context]. Desired outcome: [inform / agree on path / get acknowledgement]. |
| **Role** | You are a manager who has learned that difficult conversations done well are an act of respect — and difficult conversations avoided are an act of cowardice. You are honest without being cruel. |
| **Instruction** | Write a conversation script with: an opening that gets to the point within 90 seconds, the core message delivered clearly (no burying), space for the person to respond, and a closing that gives them a clear next step. |
| **Spec** | Script format with stage directions in brackets. 300–350 words. Gets to the point within the first 5 sentences. Includes at least one "pause and listen" marker. Does not use the word "unfortunately." |
| **Performance** | The person leaves the conversation knowing the truth, what it means for them, and what happens next. The manager did not hide behind ambiguity to protect themselves. |

---

## Full Prompt

```
Context: I'm a people manager preparing for a difficult conversation with [Team Member Name], a [role] with [tenure]. The topic: [describe the situation — e.g., "their role is being made redundant", "they did not get the promotion they expected", "I need to address their pattern of dismissive behaviour toward junior team members", "we need to discuss taking a formal performance path"]. 

What they know going in: [they have been given no indication / they may suspect / they have been told to expect this conversation]
Our relationship: [good working relationship / strained / professional but distant]
My desired outcome for this conversation: [inform them of a decision / reach agreement on next steps / get acknowledgement and plan for change]
Support available: [HR present / HR briefed but not present / manager's manager available if needed]

Role: Act as a manager who approaches difficult conversations as an act of respect — honest enough to tell the truth clearly, and compassionate enough to give the person space to process it.

Instruction: Write a conversation script with:
1. Opening — get to the topic within 90 seconds; no false warmup
2. Core Message — deliver the main news or feedback clearly in plain language; no burying
3. Pause Marker — [noted explicitly] where the manager should stop and give the person space
4. Response Handling — 2–3 ways the person might respond, and brief manager guidance for each
5. Closing — what happens next, clearly stated; one specific next step

Spec:
- Script format with stage directions in [brackets]
- 300–350 words
- Main message delivered by sentence 5 maximum
- At least one [PAUSE — WAIT FOR RESPONSE] marker
- Never uses the word "unfortunately"
- Closes with a concrete next step, not "take all the time you need"

Performance bar: The person leaves knowing the truth, what it means, and what happens next. The manager did not protect themselves at the expense of clarity. The script is deliverable by a real human.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a script for telling an employee they didn't get promoted.

**Output produced:**
> "Hi, I wanted to chat with you today. I have some news about the promotion. It was a really difficult decision and the calibration committee had a hard time because there are so many strong candidates. Unfortunately, we decided to go with someone else this time. We really value your contributions and hope you'll understand. There will be other opportunities."

**Why it's weak:** Buried the news in three sentences of warmup, used "unfortunately," vague about what actually happened, "other opportunities" with no specifics, doesn't give the person anything to work with. The person leaves confused and hurt.

---

## After Example (With CRISP)

**Placeholders filled:**
- Topic: Promotion to Staff Engineer not approved this cycle
- Person: Ana Sousa, 2 years, good working relationship
- She expects this conversation to be a decision call
- Outcome: inform her of the decision and agree on path to next cycle

**Output produced:**

> **Conversation Script — Promotion Decision | Ana Sousa**
>
> [Settle in, no small talk beyond "thanks for making time"]
>
> "Ana, I want to get straight to it because I know you've been waiting for this conversation. The promotion to Staff Engineer was not approved for this cycle.
>
> [PAUSE — let that land. Do not fill the silence immediately.]
>
> The calibration committee's decision came down to one gap: the scope of influence piece. Your technical contribution is at Staff level — that was not in question. What the committee couldn't see enough of yet is you shaping technical direction across teams, not just within ours. That's the specific thing that needs to be visible by the next cycle."
>
> [PAUSE — WAIT FOR RESPONSE. Listen fully before continuing.]
>
> **If she's upset or quiet:** "I know this is disappointing — it should be. You've been doing Staff-level work in several areas. I want you to take a moment with this, and I want you to know I'm not going anywhere. I believe this is the right call for this cycle, and I believe you'll meet it next cycle if we're deliberate about it."
>
> **If she pushes back on the decision:** "That's a fair reaction, and I want to hear your perspective. What I can tell you is the specific criteria, and I can walk you through the committee's rationale if that would help. I'm not asking you to agree with it today."
>
> **If she accepts it quietly:** "Your quietness is okay — sit with it. I want you to know I actively advocated for you and will continue to."
>
> [Closing]
>
> "Here's what I'd like to do: let's schedule a focused session next week — just us — where I walk you through exactly what the Staff criteria require and we map the next 6 months against those criteria specifically. Can we put something in the calendar for next Thursday?"
