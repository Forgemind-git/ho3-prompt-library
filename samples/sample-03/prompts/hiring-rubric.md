# Prompt 08 — Hiring Rubric

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Design a structured interview evaluation rubric for a specific role with weighted criteria, 1–4 scoring definitions, and example signals — so every interviewer is evaluating the same things, reducing bias and improving the quality of hiring decisions.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Hiring for: [role and seniority]. Team: [team description and what they'll be working on]. Top 3–4 must-have criteria: [list]. Nice-to-haves: [list]. Interview panel: [N interviewers, each with a focus area]. |
| **Role** | You are a hiring manager who has built structured interview processes from scratch and knows that an unstructured interview predicts performance no better than a coin flip. |
| **Instruction** | Create a hiring rubric with: weighted evaluation criteria, 1–4 score definitions per criterion, example "strong signal" and "weak signal" indicators, and a scoring guide for final decisions. |
| **Spec** | Rubric table format. Criteria must total 100% weight. Scores: 1=below bar, 2=meets partially, 3=meets, 4=exceeds. Each criterion has at least one positive and one negative signal example. |
| **Performance** | Any interviewer on the panel can use this rubric with no additional briefing. Scores from different interviewers are comparable. The rubric reduces "I just liked them" decisions. |

---

## Full Prompt

```
Context: I'm building a hiring rubric for a [role + seniority] position on my [team description] team. They'll be primarily working on [main responsibilities]. 

Must-have criteria (the things someone must demonstrate to pass):
1. [Criterion 1]
2. [Criterion 2]
3. [Criterion 3]
4. [Criterion 4 if applicable]

Nice-to-have criteria (would differentiate candidates at the same level):
1. [Nice-to-have 1]
2. [Nice-to-have 2]

Interview panel: [N interviewers and their areas — e.g., "3 interviewers: technical (2 sessions), values/culture (1 session)"]

Role: Act as a hiring manager who builds structured interview rubrics that make hiring decisions defensible and reduce bias — because you know that without structure, every interviewer is evaluating something different.

Instruction: Create a hiring rubric with:
1. Evaluation Criteria Table — criteria name, weight (must total 100%), and which interview covers it
2. Scoring Guide — for each criterion: score 1/2/3/4 definition + one example signal per level
3. Strong Hire / Lean Hire / No Hire thresholds — based on weighted total score
4. Debrief Instructions — how the panel should discuss scores before making a decision

Spec:
- Rubric table format
- Criteria weights must total 100%
- Score definitions: 1=does not meet, 2=partially meets, 3=meets, 4=exceeds
- At least one positive and one negative example signal per criterion
- 400 words maximum

Performance bar: Any panelist can use this rubric without a briefing call. Scores are comparable across interviewers. Final decision is based on the weighted score, not gut feel alone.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Create an interview rubric for a software developer.

**Output produced:**
> Evaluate candidates on: 1. Technical skills (rate 1–5). 2. Communication (rate 1–5). 3. Culture fit (rate 1–5). 4. Problem solving (rate 1–5). Take notes during the interview.

**Why it's weak:** No weight differentiation, no score definitions, "culture fit" is a bias-prone category with no definition, no signal examples. Four interviewers rating "technical skills 1–5" will produce four incomparable scores.

---

## After Example (With CRISP)

**Placeholders filled:**
- Role: Senior Frontend Developer | Team: 5-person product team building B2B SaaS
- Must-haves: React/TypeScript depth, system design judgment, communication, ownership
- Nice-to-haves: Design system experience, prior B2B SaaS exposure

**Output produced:**

> **Hiring Rubric — Senior Frontend Developer**
>
> **Evaluation Criteria**
>
> | Criterion | Weight | Interview |
> |-----------|--------|-----------|
> | React/TypeScript Technical Depth | 35% | Technical interviews (2x) |
> | System Design Judgment | 25% | Technical interview 2 |
> | Communication and Collaboration | 20% | Values interview |
> | Ownership and Initiative | 20% | Values interview |
>
> **Scoring Guide**
>
> **React/TypeScript Technical Depth (35%)**
> - 4 (Exceeds): Explains trade-offs between approaches unprompted; catches edge cases in code review exercise
> - 3 (Meets): Writes clean, correct TypeScript; explains component architecture clearly
> - 2 (Partial): Works but relies on trial-and-error; can't explain why they made specific choices
> - 1 (Does Not Meet): Struggles with basic React patterns or TypeScript types in the exercise
>
> **System Design Judgment (25%)**
> - 4: Asks clarifying questions about scale and constraints before designing; flags trade-offs explicitly
> - 3: Produces a reasonable design with minor gaps when prompted
> - 2: Jumps to implementation without design; unclear on state management or data flow
> - 1: Design would not scale or has fundamental architectural issues
>
> **Communication and Collaboration (20%)**
> - 4: Explains technical concepts clearly to a non-technical interviewer; gives examples of conflict resolution
> - 3: Clear communicator; shares opinions when asked
> - 2: Responses are vague; struggles to give specific examples of collaboration
> - 1: Difficulty articulating past experiences or technical ideas
>
> **Ownership and Initiative (20%)**
> - 4: Examples of shipping work beyond spec; proactively identified and solved problems
> - 3: Delivers on commitments; escalates when needed
> - 2: Executes when directed but passive; no examples of self-initiated improvement
> - 1: Blames team/tools for failures; difficulty owning outcomes
>
> **Decision Thresholds (weighted total /4)**
> - Strong Hire: 3.4+
> - Lean Hire: 2.8–3.3 (discuss in panel)
> - No Hire: Below 2.8
>
> **Debrief Protocol**  
> Each interviewer submits their scored rubric before the debrief call. Panel shares scores without discussion first. Anyone with a 1 on any criterion must explain it. Final decision requires consensus on Strong Hire; split panels default to a second technical session.
