# Prompt 04 — Refund Decision Template

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Draft a refund decision email that communicates the outcome clearly — whether approved, partial, or declined — explains the rationale without being defensive, and preserves customer goodwill regardless of the decision.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Customer [name] requested a refund of [amount] for [reason]. The decision is [approved / partial / declined]. Our refund policy states [key relevant policy point]. The customer's account status: [active / cancelled / considering cancelling]. |
| **Role** | You are a senior customer support agent with authority to communicate refund decisions. You write these with the confidence of someone who owns the decision, not the hesitancy of someone passing on bad news. |
| **Instruction** | Write a refund decision email that: states the decision clearly in the first sentence, explains the rationale in plain language, provides next steps for approved refunds or alternatives for declined ones, and closes in a way that preserves the relationship. |
| **Spec** | Email format with subject line. 150–180 words. Decision in the first sentence — no burying. If declined, offer one concrete alternative. No policy-quoting in legalistic language. |
| **Performance** | The customer knows the decision after the first sentence. The rationale is understandable to a non-technical reader. A declined customer still feels respected. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. Customer [Customer Name] submitted a refund request for [amount] related to [specific reason — e.g., "charged after cancellation", "feature not working as advertised", "accidental annual purchase"]. The decision is: [APPROVED in full / APPROVED partially for $X / DECLINED]. Our refund policy relevant to this case: [state the key policy rule in one sentence]. Customer status: [active / cancelled / at churn risk].

Role: Act as a senior customer support agent who owns refund decisions and communicates them with clarity and confidence — neither defensive nor apologetic, just honest and human.

Instruction: Write a refund decision email that:
1. States the decision clearly in the first sentence (no burying)
2. Explains the rationale in plain, non-legalistic language
3. For approved: gives the refund amount, method, and timeline
4. For declined: offers one concrete alternative (credit, discount, plan downgrade)
5. Closes in a way that preserves the relationship

Spec:
- Email with subject line
- 150–180 words
- Decision in sentence one, always
- No quoting policy in legal language
- One concrete alternative if declined

Performance bar: Customer knows the decision after sentence one. Rationale is understandable to anyone. A declined customer still feels respected and has a clear next option.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write an email telling a customer their refund was declined.

**Output produced:**
> Dear Customer, thank you for contacting us. We have reviewed your refund request. After careful consideration and in accordance with our Terms of Service, we are unable to process a refund at this time. We appreciate your understanding. If you have further questions, please contact support.

**Why it's weak:** Decision is buried in "unable to process." No rationale. No alternative offered. "In accordance with our Terms of Service" sounds threatening. Customer feels dismissed.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: Marcus Webb
- Amount: $299 (annual plan)
- Reason: Purchased annual plan by mistake, meant to buy monthly
- Decision: Partial refund of $249 (12 months minus 1 month already used)
- Customer status: Active, wants to stay monthly

**Output produced:**

> **Subject: Your refund — $249 approved and on its way**
>
> Hi Marcus,
>
> Good news: I've approved a partial refund of $249 for your annual plan.
>
> Here's the situation: you've been on the plan for 30 days, so I've applied our standard pro-rata calculation — that's 11 remaining months refunded at $22.63/month, totalling $249. The original $299 charge will be partially reversed and the $249 should appear on your card within 3–5 business days.
>
> I've also switched your account to the monthly plan ($29/month) starting today, so you won't be billed annually again unless you choose to.
>
> If you have any questions about the refund timeline or your new plan, just reply here and I'll sort it out.
>
> Thanks for sticking with us, Marcus.
>
> James  
> Customer Support Lead
