# Prompt 10 — KB Article Draft

**Library:** Customer Support Prompt Library  
**Role:** Customer Support Team Lead

---

## Purpose

Turn a resolved support thread into a publishable knowledge base article that helps future customers solve the same problem themselves — reducing repeat tickets and improving self-serve deflection rates.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | A support ticket for [issue] was resolved by [solution]. The thread contains [N] messages. The issue appears [frequency — e.g., "3+ times this month"]. Target audience: [all users / Pro plan / technical admins]. |
| **Role** | You are a technical writer who specialises in customer-facing knowledge base content. You write articles that are clear enough for a non-technical user but precise enough for a technical one. |
| **Instruction** | Write a knowledge base article with: a clear title optimised for search, a one-paragraph "What this article covers" intro, prerequisite or conditions, numbered step-by-step resolution instructions, a "Why this happens" explanation, and a "Still having issues?" closing section. |
| **Spec** | KB article format. Use headers. Steps numbered. 350–450 words. Written for the customer, not the support agent. No internal jargon. SEO-friendly title (includes the error or symptom, not the internal ticket description). |
| **Performance** | A customer who finds this article via search should be able to resolve the issue without contacting support. "Still having issues?" section reduces bounce-to-ticket rate. |

---

## Full Prompt

```
Context: I'm a Customer Support Team Lead at [Company Name]. We've resolved a support ticket involving [issue description]. The fix was: [what the solution was]. This issue has come up [N times] in the past [30 days / 3 months]. Target readers: [all users / Pro plan users / workspace admins / developers]. 

The original customer thread is pasted below for reference.

Role: Act as a technical writer who writes knowledge base articles that help customers solve problems without contacting support. Your articles are clear for non-technical users and precise for technical ones.

Instruction: Write a KB article with exactly these sections:
1. Title — SEO-friendly, includes the symptom or error message the customer would search for (not internal ticket language)
2. What This Article Covers — 2–3 sentence intro describing who this is for and what they'll be able to do after reading
3. Before You Start — any prerequisites, required permissions, or conditions
4. Steps to Resolve — numbered steps from the customer's perspective, starting from where they'd naturally begin
5. Why This Happens — a plain-language explanation of the root cause
6. Still Having Issues? — 2–3 options: try X, check Y, contact support at Z

Spec:
- KB article format with bold headers
- 350–450 words
- Written for the customer, not internal agents
- No internal terminology or ticket IDs
- SEO-optimised title (use the words a customer would type into Google)

Performance bar: A customer who finds this via search solves the problem without emailing support. The "Still Having Issues?" section is specific enough to resolve 80% of edge cases without a ticket.

--- SUPPORT THREAD ---
[Paste the resolved support thread here]
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write a help article about the CSV export bug fix.

**Output produced:**
> The CSV export bug has been fixed. To resolve this issue, clear your cache. If you still have problems, contact support.

**Why it's weak:** No steps, no context, no explanation of why it happens, no search-optimised title. "Clear your cache" without instructions helps almost no one. A customer lands on this and immediately opens a new ticket.

---

## After Example (With CRISP)

**Thread pasted:**
> "My export to CSV is stuck on a loading spinner on Chrome/Windows 11. Tried refreshing, didn't help. Pro plan."  
> Support: "Please try clearing your browser cache — Settings > Privacy > Clear Browsing Data, check Cached Images and Files. If that doesn't work, go to your account Settings > Display > Reset Chart Cache."  
> Customer: "The account settings reset worked! Thank you."

**Output produced:**

> ## CSV Export Stuck on Loading Spinner — How to Fix It
>
> **What This Article Covers**  
> If clicking "Export to CSV" shows a loading spinner that never finishes and no file downloads, this guide walks you through two quick fixes. This affects the Reports page export on all plans.
>
> **Before You Start**  
> You need to be logged in to your account. If you're on a shared computer, you may need admin access to clear browser cache.
>
> **Steps to Resolve**
>
> **Fix 1: Clear your browser cache (2 minutes)**
> 1. In Chrome, click the three-dot menu in the top-right corner
> 2. Go to **Settings > Privacy and Security > Clear browsing data**
> 3. Check **"Cached images and files"** and set the time range to "Last 7 days"
> 4. Click **Clear data**
> 5. Return to the Reports page and try the export again
>
> **Fix 2: Reset the chart cache in your account settings (30 seconds)**
> 1. Click your profile icon in the top-right of the app
> 2. Go to **Settings > Display**
> 3. Click **Reset Chart Cache**
> 4. Return to Reports and retry the export
>
> Most users find Fix 2 resolves the issue without needing to clear their browser cache.
>
> **Why This Happens**  
> The export function pulls data from a local chart cache that can become stale after account updates or browser sessions. When the cache and the server's data are out of sync, the export request gets stuck waiting for data that never arrives.
>
> **Still Having Issues?**
> - Try the export in an incognito / private browsing window — this rules out extensions interfering
> - Check you're on the latest version of Chrome (Help > About Google Chrome)
> - If neither fix works, [contact support](mailto:support@helply.io) with your browser version and a screenshot of the spinner — include "CSV Export" in your subject line for fastest triage
