# Prompt 09 — Investor Update Bullet Points

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Write concise, credible investor update bullet points for a monthly or quarterly report — communicating the financial and operational highlights, low points, and asks in a format that builds investor confidence without overselling or hiding problems.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Company: [name, stage, last raise]. Period: [month/quarter]. Financial highlights: [key metrics]. Operational highlights: [key wins]. Challenges: [honest low points]. Asks: [what you need from investors]. |
| **Role** | You are a CFO who writes investor updates that build trust — because you share the real numbers, acknowledge challenges honestly, and make your asks specific. Investors who receive vague updates stop being helpful investors. |
| **Instruction** | Write a structured investor update with: financial metrics (bullet format with data), operational highlights (3 bullets), challenges section (honest — 2 bullets), and a specific ask section. |
| **Spec** | Investor update format. Financial metrics as a table or structured bullets. Each highlight/challenge bullet: one sentence with a specific outcome or learning. Asks section has 1–3 numbered asks. 300 words max. |
| **Performance** | An investor reads this in 5 minutes and has an accurate picture of where the company is. The challenges section does not read as spin. The asks are specific enough to act on without a follow-up call. |

---

## Full Prompt

```
Context: I'm preparing the [month/quarter] investor update for [Company Name], a [stage — e.g., "Series A B2B SaaS, raised $5M in Jan 2025"]. Update audience: [your investor syndicate or specific investors].

Financial metrics for [period]:
- ARR: $[X] (vs $[Y] last period / $[Z] at raise)
- MRR: $[X]
- Revenue (if recognised differently from ARR): $[X]
- MoM/QoQ growth: [%]
- Gross margin: [%]
- Net burn: $[X]/month
- Cash runway: [N months]
- NRR: [%]
- New logos: [N]

Operational highlights (3–5 key wins or milestones):
1. [e.g., "Enterprise tier launched July 1; 4 paid pilots signed in first 30 days"]
2. [e.g., "Key hire: VP Sales joined from Salesforce (start date Aug 1)"]
3. [Add others]

Challenges (be honest — 2–3 real issues):
1. [e.g., "Mid-market churn rate higher than modelled — 3 customers churned in Q2 totalling $28K ARR"]
2. [e.g., "VP Engineering hire taking longer than expected — 8 candidates, 0 offers accepted"]

Asks from investors (specific, actionable):
1. [e.g., "Introductions to Series A CFOs who've built Enterprise sales motions — particularly looking for SaaS companies that sell to IT leaders"]
2. [Add others]

Role: Act as a CFO who writes investor updates that build long-term trust because they are honest, specific, and make every investor feel like a well-informed partner — not a passive capital provider.

Instruction: Write a structured investor update with:
1. Subject line — month/quarter + one headline number
2. Financial Snapshot — key metrics in a structured format, with brief context for any significant movement
3. Operational Highlights — 3 bullets, each with a specific outcome
4. Challenges — 2 honest bullets with what you're doing about each
5. Asks — 1–3 numbered specific asks
6. Next Update — when the next update will come

Spec:
- Investor update format
- 300 words maximum
- Financial snapshot as structured bullets or table
- Challenges: honest, not spin
- Asks: specific and actionable
- One next update date

Performance bar: Investor reads in 5 minutes and has an accurate picture. Challenges section does not read as minimisation. Asks are actionable without a follow-up call.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a monthly investor update.

**Output produced:**
> Hi investors, we had a great month! Revenue is growing and the team is working hard. We faced some challenges but we are handling them. We will keep you updated. Thanks for your continued support.

**Why it's weak:** No numbers, "great month" without evidence, "facing some challenges" without naming them, "keep you updated" is not a next-update date. This update erodes investor confidence, not builds it.

---

## After Example (With CRISP)

**Placeholders filled:**
- Helply | Series A | Period: Q2 2025
- ARR: $8.2M (+38% YoY) | MRR: $683K | Burn: $380K/month | Runway: 18 months | NRR: 114%
- Highlights: Enterprise launched, VP Sales hired, NRR at record 114%
- Challenges: Mid-market churn $28K in Q2; VP Eng search ongoing (8 rounds, 0 offers)
- Asks: Series A CFO intros, Enterprise legal counsel recommendation

**Output produced:**

> **Subject: Helply Q2 Update — $8.2M ARR | +38% YoY | Enterprise Live**
>
> Hi all,
>
> Q2 summary below. Please flag anything you'd like to discuss before our next call on July 28.
>
> ---
>
> **Financial Snapshot**
> - **ARR:** $8.2M (+38% YoY, +8% QoQ)
> - **MRR:** $683K
> - **NRR:** 114% — record high; existing customers are expanding
> - **Gross Margin:** 79%
> - **Net Burn:** $380K/month
> - **Cash Runway:** 18 months (as of July 1)
>
> ---
>
> **Operational Highlights**
> - **Enterprise tier live July 1** — 4 paid pilots signed in first 30 days, avg ACV $47K. If 3 of 4 convert (our base case), that's $141K in new ARR from a segment that didn't exist in Q1.
> - **VP Sales joined August 1** — Priya Mehta, previously RVP at Salesforce running their SMB/Mid-Market team for 4 years. She has built the Enterprise playbook we need.
> - **NRR at 114%** — driven by upsell from 7 customers expanding seat count. This is the highest it's been and validates the product-led expansion motion we invested in last year.
>
> **Challenges**
> - **Mid-market churn:** 3 customers churned in Q2, totalling $28K ARR. Root cause: all three were <$8K ACV, single-seat users who never expanded. We've added a 60-day usage check-in to our onboarding for this segment. Not catastrophic, but a pattern worth watching.
> - **VP Engineering search:** 8 candidates through the full process, 0 offers accepted — 2 declined (comp), 1 took a competing offer, 5 not progressed by us. We've briefed a specialist recruiter starting next week.
>
> **Asks**
> 1. **Intros to Series A CFOs** at SaaS companies that successfully scaled an Enterprise motion — specifically looking for companies selling to IT leadership at 500–2,000 employee companies.
> 2. **Enterprise SaaS legal counsel recommendation** — we need an attorney experienced with multi-year Enterprise contracts and data DPAs. Current counsel is great for seed-stage but not the right fit.
>
> **Next Update:** July 28 investor call | Written update August 5
>
> James (CFO)
