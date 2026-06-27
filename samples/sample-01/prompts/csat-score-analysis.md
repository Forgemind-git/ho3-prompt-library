# Prompt 08 — CSAT Score Analysis

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Analyse a batch of CSAT scores and comments to surface the top 3 actionable themes, identify what's driving low scores, highlight what's working, and produce a summary a manager can present in a team meeting without additional preparation.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | You have [N] CSAT responses from [time period]. Overall score: [X%]. Distribution: [% satisfied / % neutral / % dissatisfied]. The comments are pasted below. |
| **Role** | You are a customer experience analyst who turns raw CSAT data into clear, actionable insight. You don't describe the data — you interpret it and recommend specific actions. |
| **Instruction** | Analyse the CSAT responses and produce: an executive summary (3 sentences), top 3 negative themes with supporting quotes, top 2 positive themes with quotes, one root cause hypothesis for the lowest-scoring area, and 3 prioritised recommended actions. |
| **Spec** | Report format. Use headers. 400 words max. Each theme needs at least one direct quote from the data. Recommendations must be specific and assigned to a team/owner. |
| **Performance** | A team lead can present this in a Monday standup without having read the raw comments. Recommendations are specific enough to be turned into Jira tickets or team OKRs. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. I have [N] CSAT survey responses from [time period, e.g., "June 2025"]. Our overall CSAT score was [X%]. Score distribution: [Y% satisfied (4–5 stars) / Z% neutral (3 stars) / W% dissatisfied (1–2 stars)]. The comments are pasted below.

Role: Act as a customer experience analyst who interprets CSAT data to produce actionable insight — not a description of what the data says, but what it means and what to do about it.

Instruction: Analyse the comments below and produce a CSAT analysis report with these sections:
1. Executive Summary — 3 sentences: overall score, top problem, top strength
2. Top 3 Negative Themes — each with: theme name, number of mentions, one direct quote
3. Top 2 Positive Themes — each with: theme name, number of mentions, one direct quote
4. Root Cause Hypothesis — for the top negative theme, what might be causing it (process / product / people)
5. Recommended Actions — 3 specific actions, each with: action, expected impact, owner, priority

Spec:
- Report format with bold headers
- 400 words maximum
- Each theme must include at least one direct quote from the data
- Recommendations must be specific (not "improve communication") and assigned to a team
- Priority: High / Medium / Low

Performance bar: A team lead can present this in a Monday meeting without reading the raw comments. Recommendations can be turned directly into action items or Jira tickets.

--- CSAT COMMENTS ---
[Paste all CSAT comments here, one per line, with score if available]
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Summarise these customer feedback comments.

**Output produced:**
> Customers are generally happy but some have concerns about response times. Many appreciate the helpfulness of agents. There are also comments about the product. Overall, feedback is mixed.

**Why it's weak:** Vague themes, no quotes, no root cause, no actions. "Mixed feedback" tells a manager nothing. This is word-count filler dressed as analysis.

---

## After Example (With CRISP)

**Comments pasted (sample of 12):**
- "5 stars — James fixed my billing issue in 10 minutes, best support I've ever had"
- "2 stars — waited 3 days for a reply on a critical bug, unacceptable"
- "3 stars — the agent was nice but couldn't actually solve the technical problem, had to wait for engineering"
- "4 stars — quick response, solution worked"
- "1 star — no one acknowledged my ticket for 48 hours"
- "5 stars — clear instructions, patient agent"
- "2 stars — got transferred 3 times and had to repeat my problem each time"
- "4 stars — good follow-up after the issue"
- "2 stars — first response was 4 days later"
- "5 stars — above and beyond, sent a step-by-step Loom video"
- "3 stars — response was friendly but vague, needed 3 more emails to resolve"
- "1 star — still waiting for a response after 5 days"

**Output produced:**

> **CSAT Analysis — June 2025 | 12 responses | Overall: 58% satisfied**
>
> **Executive Summary**  
> June CSAT landed at 58%, driven down primarily by a significant first-response time problem affecting 4 of 12 respondents. Agent quality when customers do connect is a genuine strength — 3 of 4 five-star reviews mention individual agents by name. The core issue is not agent skill but queue throughput and routing.
>
> **Top 3 Negative Themes**
>
> 1. **First-Response Time** (5 mentions) — *"waited 3 days for a reply on a critical bug" / "no one acknowledged my ticket for 48 hours" / "still waiting after 5 days"*
> 2. **Transfer/Routing Friction** (2 mentions) — *"got transferred 3 times and had to repeat my problem each time"*
> 3. **Vague Initial Responses** (2 mentions) — *"response was friendly but vague, needed 3 more emails to resolve"*
>
> **Top 2 Positive Themes**
>
> 1. **Individual Agent Excellence** (3 mentions) — *"best support I've ever had" / "sent a step-by-step Loom video"*
> 2. **Follow-Up Quality** (2 mentions) — *"good follow-up after the issue"*
>
> **Root Cause Hypothesis — First-Response Time**  
> The volume of 1–3 day first-response delays suggests either (a) ticket volume has grown beyond current agent capacity, or (b) triage routing is sending technical tickets to general agents who must then re-queue to engineering — adding 24–48 hours per handoff.
>
> **Recommended Actions**
>
> | Action | Expected Impact | Owner | Priority |
> |--------|----------------|-------|----------|
> | Audit all tickets with >24h first response in June; identify which queue they entered | Pinpoints whether this is a volume or routing problem | Support Lead | High |
> | Add a "Technical — Engineering Required" triage tag to route tech tickets directly | Eliminates one transfer loop, cuts resolution time | Support Ops | High |
> | Create a first-response template library for top 5 ticket types | Reduces vague initial responses; agents reply faster with quality | Support Lead | Medium |
