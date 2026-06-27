# Prompt 02 — Board Slide Narrative

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Write the spoken narrative script for financial board slides so the numbers tell a coherent, persuasive story — not a recitation of what's already on the slide. The narrative should answer "so what?" for every number shown.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Board meeting: [date, context — Q2 review / budget approval / fundraising update]. Company stage: [startup / growth / mature]. Key slides to script: [describe what's on each slide]. Target narrative tone: [confident and optimistic / cautious and transparent / turnaround story]. |
| **Role** | You are a CFO-calibre communicator who knows that board members don't need you to read the slides — they need you to tell them what the numbers mean and what management plans to do about them. |
| **Instruction** | Write a spoken narrative script for [N] financial slides, with: an opening statement that sets the financial story for the meeting, one paragraph per slide that adds insight beyond what's visible, and a closing that frames the ask or key decision. |
| **Spec** | Script format. Each slide section clearly numbered. 60–90 seconds of spoken delivery per slide (130–160 words). Total narrative: [N slides x 150 words]. Opening 30 seconds sets the overall financial story. |
| **Performance** | A CFO delivering this script adds no unrehearsed insights — every key point is in the narrative. Board members leave understanding the headline for each slide and the one decision or implication to carry away. |

---

## Full Prompt

```
Context: I'm preparing the narrative script for [N] financial slides for a board meeting on [date]. 
- Company: [name and stage — e.g., "Series B SaaS, 3 years old, $8M ARR"]
- Meeting context: [Q2 financial review / budget approval / investor update / turnaround review]
- Overall financial story for this meeting: [what is the one headline that should define this presentation — e.g., "strong revenue growth with cost discipline" / "Q2 miss explained with clear path to recovery" / "requesting budget for strategic investment with clear ROI"]

Slides to script (describe each one):
Slide 1: [what's on it — e.g., "Revenue: $8.2M ARR, up 38% YoY; chart showing monthly revenue trend"]
Slide 2: [what's on it]
Slide 3: [what's on it]
[Add slides as needed]

Role: Act as a CFO who scripts board presentations. You know board members have already seen the numbers — your script's job is to add the "so what" and the "what we plan to do about it" for each slide.

Instruction: Write a board slide narrative with:
1. Opening Statement (30 seconds / 80 words) — set the overall financial story for this meeting in a single clear narrative
2. Slide Scripts (60–90 seconds each / 130–160 words per slide) — for each slide: state the headline finding, explain what it means for the business, note any risk or nuance, and state management's response or implication
3. Closing (30 seconds / 80 words) — frame the key ask, decision, or takeaway for this board meeting

Spec:
- Script format, slides numbered
- 130–160 words per slide
- Opening and closing at 80 words each
- Narrative adds insight beyond what's visible on the slide
- No "as you can see on this slide..."

Performance bar: Script is deliverable with minimal rehearsal. Board members understand the financial story and key decision without seeing the slides. Every "so what" is answered.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a script for my financial board presentation.

**Output produced:**
> Good morning everyone. Today I'd like to present our financial results. As you can see on Slide 1, our revenue was $8.2 million. This is an increase from last year. On Slide 2, our costs were $6.5 million. We are working to control costs going forward.

**Why it's weak:** Reads the slide, adds no insight, "working to control costs going forward" is not a plan, no "so what" for any number, no narrative thread. This is what happens when analysts prepare slides but not narrative.

---

## After Example (With CRISP)

**Slides described:**
- Slide 1: Revenue: $8.2M ARR, +38% YoY, NRR 114%
- Slide 2: Costs: $6.5M total, 79% gross margin, EBITDA ($1.2M) — in line with plan
- Slide 3: Q3 priorities: profitability path, Enterprise tier launch, hiring plan

**Output produced:**

> **Opening (85 words)**  
> "Good morning. The headline from Q2 is straightforward: we grew revenue 38% year-over-year, our net revenue retention is 114%, and we did it while keeping gross margin at 79%. EBITDA came in at negative $1.2M, exactly in line with the plan we presented in March. The story this quarter is that revenue momentum is strong, we're retaining and expanding customers at the rate we need to be, and cost discipline held even as we invested in the pipeline for Enterprise launch."
>
> ---
>
> **Slide 1 Narrative — Revenue (145 words)**  
> "The $8.2M ARR number is the surface level. What I want to draw your attention to is the NRR at 114%. That means our existing customers are, on net, expanding — for every $100 we had in recurring revenue at the start of the quarter, we ended with $114 from those same customers. That's a leading indicator that our core product-market fit is working, and it reduces our dependence on new logo acquisition to sustain growth. The revenue trend line on the right shows consistent acceleration since February — we've closed seven Enterprise pilots this quarter, and the expansion opportunity in that segment is what the Q3 priorities slide will speak to. The risk I'd flag: our mid-market cohort grew 28%, which is below the 35% we modelled. We're watching that cohort closely."
>
> ---
>
> **Slide 2 Narrative — Costs (140 words)**  
> "EBITDA of negative $1.2M is exactly where we planned to be. I want to be clear about what's driving the loss: 70% of it is planned investment in the Enterprise GTM team we approved in March. Gross margin at 79% is a record for us — up 3 points from Q1 — which reflects the infrastructure efficiency work the team completed. We are not burning cash on operating costs. We're investing it in go-to-market ahead of the Enterprise launch. The question this slide should prompt is whether the Enterprise investment is tracking to plan — and I'll address that directly on Slide 3."
>
> ---
>
> **Slide 3 Narrative and Closing (150 words)**  
> "Q3 has three priorities, and they're sequenced deliberately. The Enterprise tier launches July 15. We have seven pilots converting, with an average ACV of $48,000 — if four of those seven close in Q3, that's $192,000 in new ARR from a single segment that didn't exist six months ago. The hiring plan is intentionally light this quarter: two Enterprise AEs and one Solutions Engineer, all back-weighted to August. Headcount is the lever I'll pull if conversion rates are lower than expected. The profitability path: if Enterprise performs at our base case, we reach EBITDA breakeven in Q1 2026 — six months earlier than the plan we shared in March. The one ask I'd like from the board today is alignment on the Q1 2026 breakeven target as the planning anchor for H2. That gives the team a clear North Star."
