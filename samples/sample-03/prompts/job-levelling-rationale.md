# Prompt 06 — Job Levelling Rationale

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Write a promotion or levelling rationale that makes a compelling, evidence-based case for a team member's advancement — giving the calibration committee enough to make a decision without needing to interview you about it.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team member: [name, current level, proposed level]. Role: [job title]. Calibration date: [date]. Key evidence: [3–5 specific examples that demonstrate next-level criteria]. Levelling criteria for the target level: [list the criteria or describe your company's framework]. |
| **Role** | You are a manager who writes promotion rationales that win in calibration — because they are structured, evidence-heavy, and pre-answer the committee's standard objections. |
| **Instruction** | Write a levelling rationale with: proposed level and summary case, evidence against each promotion criterion, scope and impact statement, and a "why now" argument. |
| **Spec** | Formal rationale document. Each criterion has its own section with a specific evidence example. 400 words max. End with a one-paragraph "Why now" that addresses timing. |
| **Performance** | A calibration committee member who has never met this employee can vote confidently using only this document. The "why now" addresses the most common objection. |

---

## Full Prompt

```
Context: I'm submitting a promotion rationale for [Team Member Name], currently a [Current Level/Title], for promotion to [Target Level/Title]. Calibration committee meeting: [date].

Evidence (be as specific as possible — include outcomes, not just activities):
1. [Example 1 — project, decision, or contribution that demonstrates next-level capability]
2. [Example 2]
3. [Example 3]
4. [Example 4 if available]

Our promotion criteria for [Target Level] (summarise or list the criteria your company uses):
[E.g., "Scope: leads cross-team initiatives independently", "Impact: decisions affect more than their immediate team", "Mentorship: actively develops others", etc.]

Why now vs 6 months later: [Your honest assessment — are they already operating at the next level? Are there any concerns about timing?]

Role: Act as a manager who writes promotion rationales that win in calibration because they are evidence-heavy, structured, and pre-answer the committee's standard objections.

Instruction: Write a levelling rationale with:
1. Proposed Promotion — one sentence summary of who, from what to what, and the headline case
2. Evidence Against Criteria — one section per criterion with a specific evidence example
3. Scope and Impact — paragraph describing the scope at which this person currently operates
4. Why Now — one paragraph addressing timing: why this cycle, what changes if it's delayed

Spec:
- Formal promotion rationale format
- 400 words maximum
- Each criterion section has at least one named, specific example
- "Why now" addresses the most common delay objection
- No filler ("hardworking", "always goes above and beyond") — evidence only

Performance bar: A calibration committee member who doesn't know this employee can vote yes based solely on this document. The "why now" answers the question before it's asked.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a promotion recommendation for my senior developer.

**Output produced:**
> I am pleased to recommend [Name] for promotion to Staff Engineer. She is a talented developer who always delivers high-quality work. She is a great team player and everyone likes working with her. She has shown strong leadership skills and technical excellence. I believe she is ready for the next level.

**Why it's weak:** No specific evidence, no criteria mapping, "everyone likes working with her" is not a promotion criterion, "ready for the next level" is an assertion without support. This rationale would not survive a calibration session.

---

## After Example (With CRISP)

**Placeholders filled:**
- Ana Sousa, Senior Developer II → Staff Engineer
- Criteria: Independent cross-team scope, impact beyond immediate team, technical leadership, mentorship
- Evidence: Payment module architecture decision, P1 solo fix, mentoring two junior devs who cited her in their reviews, caught a data processing compliance issue not in her domain

**Output produced:**

> **Promotion Rationale — Ana Sousa**  
> Proposed: Senior Developer II → Staff Engineer | Submitted by: James Reid | Calibration: July 15, 2025
>
> **Headline Case**  
> Ana is already operating at the Staff Engineer level across scope, impact, and technical leadership. This rationale makes the case that she has been doing the Staff job for 6+ months without the title.
>
> **Evidence Against Criteria**
>
> *Independent Cross-Team Scope*  
> Ana led the payment module architecture for Q1 — a project that required negotiating technical trade-offs with three separate teams (Backend, Infrastructure, Compliance) without direct manager involvement. She made the call to rebuild the transaction queue rather than patch it, defended it against pushback, and proved correct. This is Staff-scope decision-making.
>
> *Impact Beyond Immediate Team*  
> In March, Ana identified a potential data residency compliance issue in the auth module that was not her remit — she was doing a routine code review. She flagged it to Legal and Infrastructure before it became a problem. This prevented a potential GDPR exposure that our Compliance team estimated would have taken 3 weeks to remediate.
>
> *Technical Leadership*  
> Ana set the technical direction for how the team handles asynchronous queue failures — a pattern now used across three other modules. She documented it in the engineering handbook without being asked.
>
> *Mentorship*  
> Two junior developers (Kenji and Yara) independently cited Ana as their most influential mentor in their H1 reviews. Ana has been running informal weekly pair sessions that management did not initiate or fund. Both developers improved measurably in code review quality in H1.
>
> **Scope and Impact**  
> Ana currently operates at a scope that touches Backend, Compliance, and Infrastructure. Her decisions have system-level effects, not just feature-level effects. She is the person other engineers go to before coming to me.
>
> **Why Now**  
> Ana has been at Senior Developer II for 24 months. She has operated at Staff scope for the last 6 of those months. Delaying creates retention risk — she has been approached by two other companies this quarter, and a title + comp alignment is the most credible retention signal available. Waiting for "more time at level" when she is already at the level is the argument we should not make here.
