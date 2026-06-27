# Prompt 02 — Performance Review Draft

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Draft a balanced, specific, evidence-based performance review that fairly reflects the team member's contributions, development areas, and trajectory — giving them something meaningful to read, not a generic evaluation that could apply to anyone.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team member: [name, role, review period]. Review type: [mid-year / annual]. Rating (if applicable): [Exceeds/Meets/Below]. Key contributions this period: [list 3–5 examples with context]. Development areas: [list 1–3 specific behaviours or skills]. Career trajectory: [where they want to go, what's next]. |
| **Role** | You are a manager who writes performance reviews that team members remember — because they are specific, honest, and show that the manager was actually paying attention. |
| **Instruction** | Write a performance review with: overall summary, 3 evidence-based strengths, 2 specific development areas with actionable guidance, and a forward-looking section on next steps. |
| **Spec** | Performance review format. 400–450 words. Each strength backed by a specific example. Development areas framed as "where to focus" not "what's wrong." No vague descriptors like "good communicator." |
| **Performance** | The team member reads this and recognises their own work in it. They are not surprised by anything. The development areas give them something specific to work on. |

---

## Full Prompt

```
Context: I'm writing a [mid-year / annual] performance review for [Team Member Name], a [role] who has been on my team for [tenure]. Review period: [start date – end date]. Their overall rating: [Exceeds Expectations / Meets Expectations / Below Expectations / Developing].

Key contributions this period (be specific):
1. [Example 1 — what they did, what the outcome was]
2. [Example 2]
3. [Example 3]
4. [Optional: Example 4 or 5]

Development areas:
1. [Specific behaviour or skill gap — what you've observed, not a personality judgement]
2. [Second development area if applicable]

Career context: [Where they want to go / what they've expressed about their next step / any levelling or promotion discussion].

Role: Act as a people manager who writes performance reviews that are specific enough that the team member recognises their own work in them — and honest enough that nothing comes as a surprise.

Instruction: Write a full performance review with:
1. Opening Summary — 2–3 sentences: overall rating, one headline strength, one development theme
2. Strengths — 3 paragraphs, each with: specific example, outcome achieved, why this matters for their role
3. Development Areas — 2 paragraphs: specific observation, impact on team/work, concrete guidance on what to do differently
4. Looking Ahead — career trajectory, next quarter priorities, manager commitment

Spec:
- Performance review narrative format
- 400–450 words
- Each strength must reference a specific example (no generic praise)
- Development framed as "where to invest" not "what's wrong with you"
- Looking Ahead section must include one concrete manager commitment

Performance bar: Team member reads this and recognises their work in it. Development areas are specific enough to act on. Manager commitment in Looking Ahead is real, not a platitude.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a performance review for my software developer.

**Output produced:**
> [Name] is a valuable member of the team. They consistently deliver high-quality work and collaborate well with colleagues. They have shown good communication skills. For development, they should continue to improve their technical skills and work on time management. Overall a strong performer.

**Why it's weak:** Could apply to anyone on any team. "Continue to improve technical skills" is not development guidance. No specific examples. "Valuable team member" is noise.

---

## After Example (With CRISP)

**Placeholders filled:**
- Ana Sousa, Senior Developer, 2 years, Annual review, Meets Expectations with Exceeds in one area
- Contributions: Led payment module architecture; fixed weekend production P1 bug solo; mentored two junior devs
- Development: Hesitates to push back on scope creep in planning; could share more in architecture discussions

**Output produced:**

> **Performance Review — Ana Sousa | Annual Review | Jan–Jun 2025**  
> Rating: Meets Expectations (with Exceeds in Technical Leadership)
>
> **Summary**  
> Ana has had a strong first half, with particular standout performance in technical leadership of the payment module. Her development focus for H2 is building more confident influence in planning and cross-team discussions — an area where her technical depth isn't yet translating into impact.
>
> **Strengths**
>
> *Technical Leadership on Payment Module*  
> Ana led the architecture design for our most complex Q1 initiative — the payment processing module migration. She made the call to rebuild the transaction queue rather than patch it, a decision that required significant pushback internally. That call proved right: the module has had zero P1 incidents since launch, compared to four in the prior system in the same period. This was genuine technical leadership, not just execution.
>
> *Reliability Under Pressure*  
> When a misconfiguration caused a P1 outage on Saturday evening in March, Ana diagnosed and fixed the issue solo in under 2 hours, with no escalation needed. What impressed me was not just the technical response but the clear incident summary she posted in #engineering at midnight — giving the team confidence without creating panic.
>
> *Mentoring Junior Developers*  
> Ana has informally taken on mentoring responsibility for two junior developers this half. Both have cited her directly in their own reviews as the person who most helped them grow. This is impact beyond her own output and I want to see it formalised in H2.
>
> **Development Areas**
>
> *Building Influence in Planning Discussions*  
> In sprint planning and architecture reviews, Ana often has a perspective but holds it back unless directly asked. In one instance, she told me after a planning session that she'd had concerns about the scope of Story DEV-441 — but hadn't raised them. The team made a decision that cost two days of rework. Ana's technical instincts are sound; the development area is trusting them enough to surface them in the room.
>
> *Pushing Back on Scope Creep*  
> When scope was added mid-sprint twice in Q2, Ana absorbed it without flagging the capacity impact. This led to two missed stories and additional pressure on QA. In H2, I'd like her to be the person who says "this changes our sprint commitment — let's talk" in the moment rather than after.
>
> **Looking Ahead**  
> Ana is tracking toward a Staff Engineer nomination in H2 if the influence growth comes. I'll sponsor her for the cross-team architecture review group starting September as a concrete development vehicle. My commitment: monthly calibration check-ins on the Staff Engineer criteria, starting August.
