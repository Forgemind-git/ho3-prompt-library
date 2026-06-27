# Prompt 01 — Reply to Angry Customer

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Write an empathetic, professional reply to an angry or frustrated customer that acknowledges their pain, owns any mistake on our side, and provides a concrete next step — without being defensive or making promises we can't keep.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | A customer has sent an angry message. They are upset about [specific issue]. They have been a customer for [X months/years] and their account tier is [free/pro/enterprise]. The issue [has been resolved / is still open / is under investigation]. |
| **Role** | You are an experienced customer support specialist known for turning angry customers into loyal ones. You have 7 years of experience in SaaS support and a natural gift for empathy. |
| **Instruction** | Write a reply email to this customer that: (1) opens with genuine acknowledgement of their frustration, (2) takes responsibility where appropriate without over-apologising, (3) explains what happened in plain language, (4) states the concrete next step with a timeline, (5) closes warmly. |
| **Spec** | Email format. 150–200 words. Subject line included. First-person singular ("I" not "we" — it feels more human). No corporate jargon. No passive voice. No hollow phrases like "We apologise for any inconvenience." |
| **Performance** | The customer should feel genuinely heard, not handled. The next step must be specific and time-bound. A senior support manager should approve this without edits. |

---

## Full Prompt

```
Context: I work as a Customer Support Team Lead at [Company Name]. A customer named [Customer Name] has just sent an angry message about [specific issue — e.g., "their account was incorrectly charged twice for the Pro plan"]. They have been with us for [X months/years] and are on our [free/pro/enterprise] plan. The issue [has been resolved / is still active / is under investigation — explain current status].

Role: Act as an experienced SaaS customer support specialist who is exceptional at turning frustrated customers into loyal ones through genuine empathy and clear communication.

Instruction: Write a reply email to [Customer Name] that:
1. Opens with a genuine acknowledgement of their frustration (not a hollow "sorry for the inconvenience")
2. Takes clear responsibility where we made a mistake
3. Explains briefly and plainly what happened
4. States one concrete next step with a specific timeline (e.g., "refund processed within 3–5 business days")
5. Closes warmly and invites them to reply if anything else comes up

Spec:
- Email format with subject line
- 150–200 words
- First person singular (I, not We)
- No corporate jargon or passive voice
- No hollow apology phrases

Performance bar: The customer should feel genuinely heard, not managed. The next step must be specific and time-bound. A support manager should approve this without changes.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a reply to an angry customer about a billing issue.

**Output produced:**
> Dear Customer,
>
> We apologise for any inconvenience this may have caused. We understand your frustration regarding the billing matter. Our team is looking into this and we will get back to you as soon as possible.
>
> Thank you for your patience.
>
> Best regards,  
> Support Team

**Why it's weak:** Generic, passive, no acknowledgement of the specific issue, no timeline, no name, sounds copy-pasted. This output would reduce trust, not build it.

---

## After Example (With CRISP)

**Placeholders filled:**
- Company: Helply
- Customer: Sarah Chen
- Issue: charged twice for Pro plan renewal
- Status: duplicate charge confirmed, refund being processed
- Tenure: 2 years, Pro plan

**Output produced:**

> **Subject: Your duplicate charge — here's exactly what I'm doing about it**
>
> Hi Sarah,
>
> I'm really sorry about this — getting charged twice for your renewal is exactly the kind of thing that should never happen, and I completely understand why you're frustrated.
>
> I've looked into your account and can confirm the duplicate charge was a processing error on our end that affected a small number of renewals yesterday. This was our mistake.
>
> Here's what I've already done: I've flagged your account and submitted the refund for the duplicate $49 charge. You'll see it back on your card within 3–5 business days, depending on your bank.
>
> I'll personally follow up on Thursday to confirm the refund has landed. If you don't hear from me by then, please reply to this email and I'll chase it immediately.
>
> Thanks for your patience, Sarah — and for sticking with us for two years. You deserve better than this.
>
> James  
> Customer Support Lead, Helply

**Why it works:** Named, specific, accountable, concrete timeline, personal follow-up commitment, warm close that honours tenure.
