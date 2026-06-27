# Prompt 07 — Competitor Content Gap Analysis

**Library:** Content Marketer Prompt Library  
**Role:** Content Marketing Manager

---

## Purpose

Identify content topics and keywords that competitors rank for (or cover well) that you don't — and prioritise them by estimated traffic potential and conversion relevance to your ICP.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Your company: [name, what you do]. Competitors: [list 2–4 competitors]. Your ICP: [who your ideal customer is]. Your current content strengths: [what topics you already cover well]. |
| **Role** | You are a content strategist who runs gap analyses that produce a prioritised content roadmap — not a list of every topic competitors mention, but the 10 topics worth actually creating. |
| **Instruction** | Analyse the competitor content information provided and produce: top 10 gap topics with search intent, estimated priority (high/medium/low), and a content angle that would differentiate your version from the competitor's. |
| **Spec** | Gap analysis table format. Each topic: keyword or topic, current owner (which competitor), search intent, priority, your differentiated angle. 10 topics, prioritised by high to low. |
| **Performance** | Content team can take this table and start briefing the top 3 pieces this week. Each differentiated angle is specific enough to be a content brief hook. |

---

## Full Prompt

```
Context: I'm running a content gap analysis for [Company Name] ([what you do, 1 sentence]) against these competitors: [list competitor names and URLs]. Our ICP: [describe your ideal customer — industry, role, company size, pain point]. Our existing content strengths (topics we already cover well): [list 3–5 topics or categories].

Competitor content information (paste what you know — from SEMrush, Ahrefs, manual research, or just the topics you've seen them cover):
[Paste competitor blog topics, categories, or keyword data here]

Role: Act as a content strategist who turns gap analysis data into a prioritised content roadmap — not a list of everything competitors do, but the 10 topics most worth creating for your ICP.

Instruction: Based on the competitor information provided, identify the top 10 content gaps — topics or keywords that competitors are covering that you are not. For each:
1. Topic/Keyword — the content gap
2. Who Owns It — which competitor ranks or covers it
3. Search Intent — informational / commercial / comparison
4. Priority — High / Medium / Low based on ICP relevance and estimated traffic
5. Your Angle — how you'd approach this topic differently to create something better or more specific for your ICP (not "write a better version" — what specifically would you do differently)

Spec:
- Table format
- 10 gaps, sorted by priority (High first)
- Your Angle must be specific — not "write a comprehensive guide"
- Note: this analysis is based on the information provided; validate with an SEO tool before investing in production

Performance bar: Content team can brief the top 3 pieces from this table this week. Each "Your Angle" is a real content hook, not a generic suggestion.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> What content should I write that my competitors are doing?

**Output produced:**
> You should look at what your competitors are doing and find topics they cover that you don't. Consider writing about common industry trends, how-to guides, and case studies. You could also do comparison posts and product reviews.

**Why it's weak:** No specifics, no priority, no differentiated angles. "Write how-to guides" is advice you could give to any company in any industry. This adds no value.

---

## After Example (With CRISP)

**Competitor info provided:**
- HelpScout covers: email support best practices, scaling support teams, CSAT benchmarks, customer feedback analysis, help desk comparison posts
- Intercom covers: customer messaging, proactive support, AI in support, product tours, onboarding playbooks
- Zendesk covers: omnichannel support, enterprise SLAs, support analytics, self-service deflection, agent performance

**Output produced:**

> **Content Gap Analysis — Helply vs. HelpScout / Intercom / Zendesk**  
> ICP: Ops leads and founders at B2B SaaS startups (5–50 employees) who are outgrowing informal support
>
> | Priority | Topic/Keyword | Owner | Intent | Your Angle |
> |----------|---------------|-------|--------|------------|
> | High | "customer support for startups" | None ranking well | Commercial | Frame around the 20–50 employee inflection point specifically — when informal email starts breaking. Real story from a startup team, not enterprise advice scaled down |
> | High | "help desk comparison for small teams" | HelpScout | Commercial | Create a comparison that is honest about where Helply wins AND loses — trust-building content that larger vendors won't write |
> | High | "CSAT alternatives" / "better metrics than CSAT" | None | Informational | Own the "CSAT is a lagging indicator" angle — tie to Helply's usage analytics feature. This is a category-creating piece |
> | High | "customer support SLA templates" | Zendesk | Informational | Create free downloadable SLA templates specifically for startups (not enterprise), with a guide on how to set realistic SLAs when you have a 2-person team |
> | Medium | "AI customer support for small teams" | Intercom | Commercial | "AI without the enterprise price tag" angle — focus on what AI automation actually saves a 3-person support team (hours, not percentage abstractions) |
> | Medium | "customer onboarding best practices" | Intercom | Informational | Specific to self-serve SaaS onboarding — with a focus on how support teams reduce onboarding tickets, not just the product team's view |
> | Medium | "support ticket volume reduction" | HelpScout | Informational | Data-driven piece using Helply customer data — specific percentage reductions by use case and team size |
> | Medium | "customer support metrics dashboard" | Zendesk | Commercial | Free Notion or Google Sheets template for CS metrics that small teams can use before they buy a tool |
> | Low | "scaling customer success" | Multiple | Informational | Differentiate: CS for self-serve vs. sales-led SaaS — most content ignores this distinction |
> | Low | "proactive customer support" | Intercom | Informational | Focus specifically on email/ticket-based proactive support (not in-app messaging) — underserved angle for non-Intercom users |
