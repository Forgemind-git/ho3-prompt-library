# Prompt 06 — Customer Onboarding Email

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Write a warm, structured welcome email to a new customer that sets clear expectations, surfaces the 3 most important first steps, and makes the customer feel like they made the right decision — without overwhelming them with every feature at once.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | A new customer just signed up for [Plan]. They came from [source: trial / migration / referral]. Their primary use case is [what they signed up to do]. Key resources: [login URL, getting-started guide, support email, community link]. |
| **Role** | You are a customer success specialist writing the very first email a new customer receives. This email sets the tone for the entire relationship. |
| **Instruction** | Write a welcome email that: opens with one sentence of genuine welcome (not a feature list), surfaces exactly 3 first steps in numbered format, sets response-time expectations, and ends with a personal invitation to reach out. |
| **Spec** | Email with subject line. 180–220 words. Warm but professional. Three numbered first steps — no more. One hyperlink per step. Signed by a named human, not "The Team." |
| **Performance** | The customer completes at least one first step within 24 hours of receiving this email. They don't feel overwhelmed. The email feels written by a person. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. A new customer named [Customer Name] just signed up for our [Plan Name] plan. They came via [trial conversion / migration from competitor / referral]. Their primary use case based on their signup form: [what they said they want to use the product for]. 

Key links:
- Login: [URL]
- Getting Started Guide: [URL]
- Help Centre: [URL]
- Support email: [email]

Role: Act as a customer success specialist writing the most important email in the customer relationship — the first one. This sets the tone and determines whether they engage deeply or churn within 30 days.

Instruction: Write a welcome email that:
1. Opens with one genuine welcoming sentence (not a feature list)
2. Lists exactly 3 numbered first steps tailored to their use case
3. Includes one link per step
4. Sets clear response-time expectation for support
5. Closes with a personal, low-pressure invitation to reach out

Spec:
- Email with subject line
- 180–220 words
- Warm but professional — not corporate, not overly casual
- Three first steps only — no feature dumping
- Signed with a named person + title

Performance bar: Customer completes at least one step within 24 hours. They don't feel overwhelmed. The email reads like it was written by a person who knows their use case.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a welcome email for a new customer.

**Output produced:**
> Welcome to [Company]! We are excited to have you on board. You now have access to all our amazing features including dashboards, reports, integrations, automations, and more. Check out our website for tutorials. Our support team is available 24/7. Welcome aboard!

**Why it's weak:** Feature dump, no personalisation, no first steps, no human signature. This is what every SaaS welcome email looks like and why nobody reads them.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: Lena Fischer
- Plan: Pro
- Source: Trial conversion (14-day trial, used reporting features heavily)
- Use case: Track weekly KPIs for a 12-person marketing team
- Links: app.helply.io / helply.io/start / helply.io/help / support@helply.io

**Output produced:**

> **Subject: You're in, Lena — 3 things worth doing in your first 10 minutes**
>
> Hi Lena,
>
> Really glad you decided to stick with us after the trial — welcome to Pro.
>
> Based on what you were building during your trial, here are the three things I'd do first:
>
> **1. Set up your team dashboard** — add your 12 team members and configure the KPIs you want everyone tracking. [Dashboard setup guide →](https://helply.io/start/dashboard)
>
> **2. Connect your data source** — link your marketing tools so your reports populate automatically rather than requiring manual input. [Integration guide →](https://helply.io/start/integrations)
>
> **3. Schedule your first weekly digest** — takes 2 minutes to set up and saves your team 30 minutes of manual reporting every Friday. [Set up digests →](https://helply.io/start/digests)
>
> If you hit a snag at any point, reply to this email and I'll get back to you within a few hours (Monday–Friday, 9am–6pm CET).
>
> Excited to see what you build.
>
> James  
> Customer Support Lead, Helply
