# Prompt 03 — Bug Report Summary

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Convert a messy, emotional customer email thread into a clean, structured bug report that engineers can immediately act on — with steps to reproduce, environment details, expected vs actual behaviour, and severity.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | A customer reported a bug via support email. The thread contains [N] messages with [description of what customer described]. We have [confirmed / not yet confirmed] the issue. Affected customers: [number or "unknown"]. |
| **Role** | You are a technical support specialist who bridges customer-facing support and engineering teams. You write bug reports that engineers trust because they are precise, complete, and free of fluff. |
| **Instruction** | Convert the customer thread (pasted below) into a structured bug report with: title, severity, summary, steps to reproduce, expected behaviour, actual behaviour, environment, affected customers, and any attached evidence. |
| **Spec** | Engineering ticket format. Use the exact section headers listed. Severity must be one of: P1-Critical / P2-High / P3-Medium / P4-Low with a one-sentence justification. Steps must be numbered. 300 words max. |
| **Performance** | An engineer should be able to start investigating immediately using only this report. No ambiguity in steps to reproduce. Severity is justified. |

---

## Full Prompt

```
Context: I'm a Customer Support agent at [Company Name]. A customer named [Customer Name] reported a bug in our [product/feature name]. Below is the raw customer email thread. I need to convert it into a clean bug report for our engineering team.

Known context:
- Issue confirmed by: [us / not yet / another customer also reported]
- Number of affected customers: [N or "unknown"]
- Environment details if known: [browser, OS, plan type, etc.]

Role: Act as a technical support specialist who writes precise, engineering-ready bug reports from customer emails. Engineers trust your reports because they are unambiguous and complete.

Instruction: Read the thread below and produce a structured bug report with exactly these sections:
1. Title — one-line description (verb + what + where)
2. Severity — P1/P2/P3/P4 with one-sentence justification
3. Summary — 2–3 sentences describing the issue in plain technical language
4. Steps to Reproduce — numbered, starting from a logged-out or clean state
5. Expected Behaviour — what should happen
6. Actual Behaviour — what actually happens
7. Environment — browser, OS, account type, plan, any known conditions
8. Affected Customers — count and tier
9. Evidence Attached — list any screenshots, logs, or recordings mentioned

Spec:
- Engineering ticket format
- No customer-facing language or emotional context
- Steps must be numbered and start from a reproducible state
- 300 words maximum

Performance bar: An engineer can start investigating immediately using only this report. No ambiguity in steps to reproduce. Severity rating is clearly justified.

--- CUSTOMER THREAD ---
[Paste the full customer email thread here]
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Summarise this customer bug report for engineering.

**Output produced:**
> The customer says the export button isn't working. They are frustrated. Please look into this.

**Why it's weak:** No steps to reproduce, no environment, no severity, no expected vs actual behaviour. An engineer receiving this has nothing actionable.

---

## After Example (With CRISP)

**Thread pasted:**
> "Hi, your export to CSV button on the Reports page has been broken for 2 days. When I click it, the page just spins and nothing downloads. I'm on Chrome, Windows 11, Pro plan. I need this for my board meeting on Friday. This is urgent!"

**Output produced:**

> **Title:** Export-to-CSV button fails silently on Reports page (Chrome / Windows 11)
>
> **Severity:** P2-High — Production feature completely non-functional for Pro plan customers; board-level deadline impact reported.
>
> **Summary:**  
> Clicking "Export to CSV" on the Reports page triggers an infinite loading spinner but produces no file download. The issue has persisted for at least 48 hours. Affects Chrome on Windows 11; other environments not yet confirmed.
>
> **Steps to Reproduce**
> 1. Log in as a Pro plan user
> 2. Navigate to Reports > [any report]
> 3. Click the "Export to CSV" button in the top-right toolbar
> 4. Observe: loading spinner appears, no file downloads, no error message
>
> **Expected Behaviour:**  
> A CSV file downloads immediately (or within 5 seconds for large reports).
>
> **Actual Behaviour:**  
> Infinite loading spinner. No file. No error message. No network timeout shown.
>
> **Environment:**  
> Browser: Chrome (version unknown) | OS: Windows 11 | Plan: Pro | Feature: Reports page export
>
> **Affected Customers:**  
> 1 confirmed reporter (Pro plan). Scale unknown — recommend checking error logs for export endpoint failures in last 48h.
>
> **Evidence Attached:**  
> None attached by customer. Request screenshot of spinner + browser console errors if needed.
