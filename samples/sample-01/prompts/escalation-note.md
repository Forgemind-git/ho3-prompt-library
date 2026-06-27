# Prompt 02 — Escalation Note

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Write a structured internal escalation note that hands off a complex or sensitive customer case to a senior agent or manager with full context — so the receiving agent can act immediately without having to read the entire ticket thread.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | You are escalating a case that has [number] of interactions, lasted [X days], and involves [issue type]. The customer's sentiment is [frustrated/threatening to churn/escalating publicly]. Previous resolution attempts: [list what was tried]. |
| **Role** | You are a methodical senior support agent who writes internal escalation notes that are precise, jargon-free, and give the receiving agent everything they need in under 60 seconds of reading. |
| **Instruction** | Write an escalation note with these sections: (1) Case snapshot — one sentence summary, (2) Customer profile — tenure, plan, revenue, (3) Issue timeline — what happened and when, (4) What was tried — previous resolution attempts, (5) Why it's being escalated, (6) Recommended next action with owner. |
| **Spec** | Internal document format. Bullet points for timeline and attempts. 200–250 words total. Bold the section headers. No customer-facing language — this is internal. |
| **Performance** | The receiving agent should be fully briefed in under 60 seconds. No important detail should be buried. The recommended action must be specific and assign a named owner. |

---

## Full Prompt

```
Context: I'm a Customer Support agent escalating a case to [Recipient Name / Senior Agent / Manager]. The case involves customer [Customer Name], [tenure] on [plan], regarding [issue description]. We've had [N] interactions over [X days]. The customer's current sentiment is [frustrated / threatening churn / asking for legal action / escalating on social media]. Previous resolution attempts: [list 2–4 things that were tried and why they didn't resolve the issue].

Role: Act as a methodical senior support agent who writes internal escalation notes that give the receiving agent everything they need in under 60 seconds.

Instruction: Write a structured escalation note with exactly these sections:
1. Case Snapshot — one-sentence summary of the issue and urgency
2. Customer Profile — name, plan, tenure, estimated monthly revenue
3. Issue Timeline — bulleted chronology of what happened and when
4. What Was Tried — bulleted list of resolution attempts and outcomes
5. Reason for Escalation — why this case cannot be resolved at the current level
6. Recommended Next Action — specific action, named owner, and deadline

Spec:
- Internal document only (not customer-facing)
- Bold all section headers
- Bullet points for Timeline and What Was Tried
- 200–250 words total

Performance bar: The receiving agent reads this in under 60 seconds and can act immediately. No critical detail is buried. The recommended action has a clear owner.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write an escalation note for a difficult customer.

**Output produced:**
> Please escalate this ticket. The customer is very upset and we have tried to help but nothing is working. They want to speak to a manager. The issue is related to their account and we have been going back and forth for a few days. Please handle ASAP.

**Why it's weak:** No structure, no specifics, no timeline, no context on what was tried. The receiving agent has to read the entire ticket anyway. This wastes everyone's time.

---

## After Example (With CRISP)

**Placeholders filled:**
- Customer: Priya Mehta, 18 months, Enterprise plan (~$2,400/month)
- Issue: SSO integration broken after our latest update, blocking 200+ team members
- Attempts: checked SAML config, rolled back user settings, issued temp credentials, scheduled call that customer cancelled

**Output produced:**

> **ESCALATION NOTE — Priya Mehta / TechCorp Enterprise**
>
> **Case Snapshot**  
> Enterprise SSO integration broken for 18 months since our v4.2 update — 200+ employees locked out for 72+ hours. Customer threatening to cancel.
>
> **Customer Profile**  
> Priya Mehta, IT Director | 18-month customer | Enterprise plan | ~$2,400/month MRR
>
> **Issue Timeline**
> - Mon 09:00 — Priya reports SSO login failure after v4.2 deploy
> - Mon 14:00 — L1 agent verifies SAML config is unchanged on customer side
> - Tue 10:00 — L1 rolled back user permissions, no change
> - Tue 15:00 — Temp credentials issued; Priya says unacceptable at enterprise scale
> - Wed 09:00 — Scheduled call; customer cancelled, emailed "escalating to your CEO"
>
> **What Was Tried**
> - SAML config review (no issues found on customer side)
> - Permission rollback to pre-update state
> - Temporary credential workaround (rejected)
>
> **Reason for Escalation**  
> Root cause appears to be a server-side SAML parsing bug introduced in v4.2. Requires engineering access. Customer sentiment is critical — churn risk is high.
>
> **Recommended Next Action**  
> Owner: @danieleng (Backend) + @sarahmanager (CS Manager)  
> Action: Engineering hotfix review by EOD today. Sarah to call Priya at 3pm with update.  
> Deadline: Resolution plan communicated by 5pm Wednesday.
