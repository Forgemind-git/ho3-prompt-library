# Prompt 05 — Follow-Up Sequence Draft

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Draft a 3-email post-resolution follow-up sequence that checks in with the customer, drives CSAT survey responses, and reduces churn risk — without feeling spammy or scripted.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | A support issue for customer [name] was resolved [X days ago]. The issue was [brief description]. The customer's sentiment at close was [satisfied / neutral / still slightly frustrated]. Our CSAT survey link: [URL or placeholder]. |
| **Role** | You are a customer success-oriented support lead who understands that the follow-up after a resolution is as important as the resolution itself — it's where loyalty is built. |
| **Instruction** | Write a 3-email sequence: Email 1 (Day 1 post-resolution) — check-in and CSAT ask. Email 2 (Day 4) — soft resurface and value nudge. Email 3 (Day 10) — final check-in with a resource offer. |
| **Spec** | Three separate email drafts with subject lines. Each email 80–120 words. Conversational, human tone — not marketing copy. No email should feel like a mass send. One clear call to action per email. |
| **Performance** | A customer who was frustrated should want to respond to Email 1. Each email feels personal, not automated. CTAs are clear and low-friction. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. We just resolved a support issue for [Customer Name] [N] day(s) ago. The issue was: [brief description of what went wrong and how it was fixed]. The customer's sentiment at close: [satisfied and grateful / neutral / still slightly frustrated but accepted the resolution]. Our CSAT survey link: [URL].

Role: Act as a customer success-oriented support lead who sees the post-resolution follow-up as the moment where loyalty is actually built — not a checkbox task.

Instruction: Write a 3-email follow-up sequence:
- Email 1 (Day 1 after resolution): Warm check-in confirming everything is still working. Ask them to fill in the CSAT survey. One clear CTA.
- Email 2 (Day 4): Resurface gently. Share one relevant tip or resource related to the feature they had trouble with. Soft CTA (reply if anything else comes up).
- Email 3 (Day 10): Final check-in. Offer to schedule a call or connect them with a success resource if they want a deeper orientation.

Spec:
- Three separate emails with subject lines
- Each email 80–120 words
- Conversational, personal tone — not marketing copy
- One clear CTA per email
- No email should feel like a mass-send

Performance bar: A frustrated customer wants to respond to Email 1. Each email feels individually written. CTAs are obvious and low-friction.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write 3 follow-up emails after a support ticket is resolved.

**Output produced:**
> Email 1: Hi, we hope your issue is resolved. Please fill in our survey. Email 2: Hi, just checking in. Let us know if you need anything. Email 3: Hi, we hope you are enjoying the product. Contact us anytime.

**Why it's weak:** Generic, interchangeable. No reference to the specific issue. No personality. Customer wouldn't open Email 2 after receiving Email 1 like this.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: Nina Okafor
- Issue: dashboard charts not loading, fixed by clearing cache + account-level settings reset
- Sentiment at close: neutral, not thrilled but accepted the fix
- CSAT URL: https://helply.io/csat/nina-okafor-june

**Output produced:**

> ---
> **Email 1 — Subject: Quick check-in on your dashboard charts**
>
> Hi Nina,
>
> Wanted to drop a quick note to make sure the dashboard charts are loading properly now — I know that took longer than it should have.
>
> If everything looks good, I'd really appreciate 30 seconds of your time: [How did we do? →](https://helply.io/csat/nina-okafor-june)
>
> And if anything's still off, just reply here and I'll pick it straight back up.
>
> James

> ---
> **Email 2 — Subject: One thing that might save you the headache next time**
>
> Hi Nina,
>
> Hope your dashboards have been running smoothly this week.
>
> One thing worth knowing: if charts ever stop loading again, the fastest fix is Settings > Display > Reset Chart Cache — it's a 10-second self-serve option I should have pointed you to first. Here's the [help article](https://helply.io/kb/chart-cache) if you want the full steps.
>
> Let me know if you run into anything else.
>
> James

> ---
> **Email 3 — Subject: Still here if you need anything**
>
> Hi Nina,
>
> Just a final check-in from my side — it's been about 10 days since we sorted your dashboard issue and I wanted to make sure things have been smooth since then.
>
> If you'd find it useful, I'm happy to set up a 20-minute call to walk through the reporting features — a lot of customers find there's more there than they initially realised. Just reply "call" and I'll send a booking link.
>
> Either way, you know where to find me.
>
> James
