# Prompt 04 — Case Study Interview Questions

**Library:** Content Marketer Prompt Library  
**Role:** Content Marketing Manager

---

## Purpose

Generate targeted, open-ended interview questions for a customer case study that surface specific outcomes, memorable quotes, and emotional moments — rather than producing a story full of vague claims like "we saved time" with no proof.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Customer: [company name, industry, size]. What they use your product for: [use case]. Known outcome: [metrics you already know — e.g., "they reduced support tickets by 40%"]. Case study angle: [what story you want to tell]. Intended audience for the case study: [who will read it — prospects, specific role]. |
| **Role** | You are a B2B content writer who has conducted 100+ customer interviews. You know that the best case study quotes come from questions about the before-state, the decision moment, and the specific moment things changed — not from asking "what do you like about our product?" |
| **Instruction** | Generate 15 interview questions organised by phase: before (the problem), the decision, implementation, results, and emotional/personal. Prioritise questions that will surface quotable answers and specific numbers. |
| **Spec** | 15 questions organised into 5 phases (3 questions each). Each question is open-ended (no yes/no). Include a note on what each question is designed to surface. 300 words max for the question set. |
| **Performance** | The interviewer uses these 15 questions and walks away with at least 3 quotable moments and 2 specific metrics. No question can be answered with "yes" or "no." |

---

## Full Prompt

```
Context: I'm conducting a case study interview with [Customer Name/Company] for [Your Company]'s case study program. 
- Customer: [company name], [industry], [company size]
- What they use our product for: [primary use case]
- Known outcomes we want to confirm/expand: [metrics you already know or suspect — e.g., "we know they saved 40% on support costs; we want the story behind it"]
- Angle for this case study: [the narrative hook — e.g., "from reactive to proactive support" / "scaling without hiring" / "migration success story"]
- Intended audience for the case study: [e.g., "VP-level CS leaders at Series B SaaS companies"]
- What the customer has agreed to share: [public name and logo / anonymised / specific metrics only]

Role: Act as an experienced B2B case study interviewer who knows that the best quotes and moments come from asking about the before-state, the turning point, and specific moments — not from asking customers to describe your product's features.

Instruction: Generate 15 interview questions organised into 5 phases:
1. The Before (3 questions) — surface the pain, the workarounds, the cost of not solving it
2. The Decision (3 questions) — the evaluation process, what tipped the decision
3. Implementation (3 questions) — what the rollout was like, surprises, team reaction
4. Results (3 questions) — specific outcomes, what changed, what they measure now
5. Emotional/Personal (3 questions) — moments of pride, recommendation, the human story

Spec:
- 15 questions, 5 phases, 3 per phase
- Each question: open-ended only (no yes/no possible)
- Include one-line note on what each question is designed to surface
- 300 words for the question set
- No question should include your product name (makes answers less authentic)

Performance bar: Interviewer walks away with 3+ quotable moments and 2+ specific metrics. Every question could produce a usable quote. No yes/no answers possible.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write interview questions for a customer case study.

**Output produced:**
> 1. What do you think of our product? 2. What features do you use most? 3. Would you recommend us? 4. What results have you seen? 5. Any other feedback?

**Why it's weak:** Question 1 will get "it's great, we love it." Question 3 is yes/no. Question 4 is so vague the customer won't know where to start. These questions produce generic testimonials, not compelling case studies.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: TechCorp (B2B SaaS, 120 employees)
- Use case: Centralised customer support for a 3-person team handling 500 tickets/week
- Known outcome: 40% ticket reduction, team now handles volume without adding headcount
- Angle: "Scaling support without scaling the team"
- Audience: Ops leaders at fast-growing SaaS companies

**Output produced:**

> **Case Study Interview Guide — TechCorp x Helply**
>
> **Phase 1: The Before (Pain + Context)**
> 1. "Walk me through what your support setup looked like 18 months ago — who was responsible, what tools you were using, and what a typical day looked like." *(Surfaces the before-state in the customer's own words)*
> 2. "What was the thing that was breaking down most often — the thing that made your team feel like they were losing control?" *(Surfaces the emotional cost of the problem, not just the operational one)*
> 3. "Can you put a number on what that was costing — time, team morale, customer complaints, anything that made the impact concrete?" *(Surfaces a specific metric to anchor the story)*
>
> **Phase 2: The Decision**
> 4. "What made you decide to change something at that particular moment — what was the trigger?" *(The decision catalyst — often the most quotable moment)*
> 5. "How did you evaluate your options — what were the 2 or 3 things you had to be confident about before committing?" *(Surfaces evaluation criteria that resonate with prospects in the same position)*
> 6. "What almost stopped you from moving forward?" *(Surfaces the objection every prospect has — and how they overcame it)*
>
> **Phase 3: Implementation**
> 7. "What was the first week of rollout actually like — what surprised you?" *(Authentic, un-polished detail that makes the story real)*
> 8. "How did your team react when they first used it in production?" *(Team adoption story — often very quotable)*
> 9. "What was harder than you expected, and what was easier?" *(Honest balance that builds credibility)*
>
> **Phase 4: Results**
> 10. "When did you first notice something meaningfully different — what did you see or measure?" *(The turning point moment)*
> 11. "What would the numbers look like if you'd stayed with your old approach through today?" *(Forces a concrete comparison)*
> 12. "What's your team able to do now that they simply couldn't do before?" *(Surfaces qualitative outcomes)*
>
> **Phase 5: Emotional / Personal**
> 13. "What's the moment from the last 12 months you'd be most proud to tell your CEO about?" *(Pride quote — often the headline)*
> 14. "If a peer asked why you made this change, what's the one thing you'd want them to know before they decide?" *(The recommendation in their own words)*
> 15. "Is there anything I haven't asked about that you think the next person in your position should know?" *(The thing they've been wanting to say)*
