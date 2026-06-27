# Prompt 09 — Out-of-Office Policy Note

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Write a clear, friendly communication to customers explaining support availability, response-time SLAs by plan tier, escalation paths for urgent issues, and what to do if they need help outside business hours — without making it sound like a legal disclaimer.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Your support team covers [hours]. You are [explaining new hours / communicating holiday coverage / setting expectations for a new customer segment]. SLAs by plan: [list them]. Emergency/urgent path: [describe it]. |
| **Role** | You are a support team lead communicating operationally important information in a way that's clear and reassuring — not defensive or bureaucratic. |
| **Instruction** | Write a policy note that: states availability hours upfront, lists response-time commitments by plan in a scannable format, explains what counts as "urgent" and how to escalate, and closes with a warm reassurance. |
| **Spec** | Email or help-centre format. 180–220 words. Scannable — use a small table for SLA tiers. Plain language, no jargon. Not a legal document. |
| **Performance** | A customer reading this in 30 seconds should know: when to expect a reply, how to escalate something urgent, and that the team is accessible. No anxiety-inducing ambiguity. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. I need to communicate our support availability and response-time SLAs to [new customers / all customers / customers asking about holiday hours]. Our current coverage:
- Support hours: [e.g., Monday–Friday, 9am–6pm UTC]
- Holiday / out-of-office dates: [list any, or "none currently"]
- Response SLAs by plan:
  - Free: [X business days]
  - Pro: [Y business hours]
  - Enterprise: [Z hours, 24/5]
- Urgent/emergency path: [e.g., "mark subject line URGENT for priority triage" or "use in-app emergency chat"]

Role: Act as a support team lead communicating important operational information in a way that's reassuring and human — not a terms-of-service bot.

Instruction: Write a clear availability and SLA communication that:
1. States support hours and timezone upfront
2. Presents response-time commitments in a scannable table by plan
3. Explains what qualifies as "urgent" and how to escalate it
4. Reassures customers on lower-tier plans that they still matter
5. Closes warmly

Spec:
- Email or help-centre article format
- 180–220 words
- SLA commitments in a small table (not buried in prose)
- Plain language — no legal/compliance tone
- Warm, accessible close

Performance bar: Customer reads this in 30 seconds and knows exactly when to expect a reply and how to escalate something urgent. No ambiguity.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Explain our support hours policy.

**Output produced:**
> Our support team is available during business hours. We aim to respond as quickly as possible. Please note that response times may vary. For urgent issues, please contact us and we will do our best to prioritise your request. Thank you for your patience.

**Why it's weak:** No actual hours, no SLAs, "as quickly as possible" is meaningless, "we will do our best" is not a commitment. A customer reading this is more anxious afterwards than before.

---

## After Example (With CRISP)

**Placeholders filled:**
- Hours: Monday–Friday, 9am–6pm UTC
- No current holidays
- Free: 2 business days / Pro: 8 business hours / Enterprise: 4 hours, 24/5
- Urgent path: Mark subject line with [URGENT] and reply received within 2 hours during business hours

**Output produced:**

> **Subject: When to expect a reply from Helply Support**
>
> Hi there,
>
> Here's a clear picture of our support availability so you always know what to expect.
>
> **Support Hours:** Monday – Friday, 9am – 6pm UTC
>
> **Response Times by Plan:**
>
> | Plan | First Response | Coverage |
> |------|---------------|----------|
> | Free | 2 business days | Mon–Fri |
> | Pro | 8 business hours | Mon–Fri |
> | Enterprise | 4 hours | Mon–Fri, 24/5 |
>
> **For something urgent:** Add `[URGENT]` to your email subject line. Our queue monitors for this tag and we'll respond within 2 hours during business hours. Urgent means: system down, data loss risk, or blocking more than 5 users.
>
> If you're on the Free plan and have an urgent issue, please use [URGENT] — we prioritise these regardless of plan.
>
> Outside business hours, our [Help Centre](https://helply.io/help) covers the most common issues with step-by-step guides.
>
> We aim to give you a complete answer on the first reply — not just an acknowledgement.
>
> James  
> Customer Support Lead, Helply
