# Prompt 07 — Feature Request Acknowledgement

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Acknowledge a customer feature request honestly — validating their use case, confirming it's been logged, and setting accurate expectations — without making promises the product team hasn't confirmed or dismissing the request with a hollow "we'll pass this along."

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Customer [name] has requested [feature]. Their use case: [what they're trying to accomplish]. Current workaround (if any): [describe it]. Product team status on this feature: [on roadmap / not on roadmap / under review / already logged by multiple customers]. |
| **Role** | You are a support lead who is trusted by customers because you are honest about what's on the roadmap and what isn't — you never over-promise and you always follow through on what you say you'll do. |
| **Instruction** | Write a feature request acknowledgement that: confirms the request is logged with a specific reference, validates the use case genuinely, shares the honest product status without over-promising, and offers a workaround if one exists. |
| **Spec** | Email with subject line. 120–160 words. No "great idea!" hollow praise. No "we'll definitely build this" over-commitment. If there's no workaround, say so honestly. |
| **Performance** | The customer feels heard and trusts that their request was actually logged. Expectations are calibrated correctly. No follow-up email asking "did you get my request?" |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. Customer [Customer Name] has submitted a feature request for: [describe the requested feature]. Their stated use case: [what they are trying to accomplish with this feature]. Current product status for this feature: [on roadmap Q3 / not on current roadmap / under review / already logged from 5+ other customers]. Existing workaround: [describe it, or "no workaround currently exists"].

Role: Act as a support lead who is trusted because you are honest and accurate — you don't praise every idea as "great" and you don't over-commit on features the product team hasn't confirmed.

Instruction: Write a feature request response email that:
1. Thanks them briefly (one sentence, no hollow praise)
2. Confirms the request has been logged with a ticket/reference number
3. Validates their use case genuinely in one sentence
4. Shares the honest status of the feature without over-promising
5. Offers the workaround if one exists
6. Tells them when/how they'll be updated

Spec:
- Email with subject line
- 120–160 words
- No hollow phrases like "great idea!" or "we'll definitely look into this"
- Be honest about roadmap status
- One clear next step or update mechanism

Performance bar: Customer feels heard and has calibrated expectations. No follow-up asking "did you log my request?" Honest status communicated without burning trust.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write an email acknowledging a feature request.

**Output produced:**
> Hi, thank you for your feedback! We think this is a great idea. We will pass this along to our product team for consideration. We appreciate your input and hope to implement this in the future. Thank you for being a valued customer!

**Why it's weak:** "Pass this along" signals the request is going into a black hole. "Great idea" is hollow. No confirmation it was actually logged. No honest status. No timeline. Customer will follow up again in a week.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: Tom Eriksson
- Request: Bulk CSV import for contacts
- Use case: Migrating from a legacy CRM with 3,000 contacts
- Status: On roadmap, targeted for Q3 but not confirmed
- Workaround: Manual import of up to 100 contacts per batch via the existing UI

**Output produced:**

> **Subject: Your request for bulk CSV import — logged as FR-2847**
>
> Hi Tom,
>
> Thanks for taking the time to describe your use case — migrating a 3,000-contact database without a bulk import is genuinely painful and I understand why this is a priority for you.
>
> I've logged your request as **FR-2847** in our product backlog. Bulk CSV import is on our roadmap and is currently targeted for Q3 — though that's not a firm commitment until the team finalises the quarter's scope.
>
> In the meantime, the closest workaround is our batch import tool (Settings > Contacts > Import), which handles up to 100 contacts per upload. Not ideal for 3,000, but it's something for urgent records.
>
> I'll ping you directly if the roadmap status changes or Q3 scope gets confirmed. No need to chase us.
>
> James  
> Customer Support Lead
