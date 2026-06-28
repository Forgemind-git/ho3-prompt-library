# Customer Support Prompt Library

**Role:** Customer Support Team Lead  
**Sample:** 01 of 05 — HO3: Prompt Library

---

## Problem Statement

Customer support teams waste hours rewriting the same types of responses from scratch — angry customer replies, escalation notes, refund decisions. Quality is inconsistent across agents, tone drifts under pressure, and onboarding new team members means passing around a messy Google Doc of copy-paste templates.

This prompt library solves that. It gives your team a structured, reusable set of AI prompts that produce high-quality first drafts in seconds — not generic outputs, but context-aware responses shaped by your role, constraints, and quality bar.

---

## Use it with your Claude.ai subscription
No API key needed. Just your normal Claude.ai login.

1. Open the file **`index.html`** from this folder in your web browser (double-click it). You'll see every support prompt as a card.
2. Find the prompt you need (for example, *Reply to an Angry Customer*) and click its **Copy** button.
3. Open **Claude.ai** in another tab and paste the prompt into the chat box.
4. Replace the `[BRACKET]` placeholders (like `[CUSTOMER NAME]` or `[PASTE TICKET]`) with your real details, then press Enter.
5. Read Claude's draft, tweak it, and send. If the tone is off, just tell Claude "warmer" or "shorter".

Prefer reading the prompts as text? Open any file in the **`prompts/`** folder and copy the prompt from its **Full Prompt** section. No API key needed.

## What Is the CRISP Framework?

Every prompt in this library is built on **CRISP** — a five-part structure that removes ambiguity and tells the AI exactly what you need:

| Letter | Stands For | What It Does |
|--------|-----------|--------------|
| **C** | Context | Sets the scene — who you are, what situation you're in |
| **R** | Role | Tells the AI what persona or expertise to adopt |
| **I** | Instruction | The core task — what the AI must actually do |
| **S** | Spec | Output specifications — format, length, tone, constraints |
| **P** | Performance | The quality bar — what "great" looks like for this output |

A weak prompt gives the AI one or two of these. A CRISP prompt gives all five, which is why the outputs are dramatically better.

---

## How to Use This Library

1. **Browse `index.md`** to find the prompt type you need.
2. **Open the relevant `.md` file** in the `prompts/` folder.
3. **Copy the full prompt text** from the "Full Prompt" section.
4. **Replace the `[BRACKET]` placeholders** with your actual situation details.
5. **Paste into Claude** (or your preferred AI) and review the output.
6. **Edit as needed** — the AI gives you a strong first draft, not a final answer.

### Tips for Best Results
- Fill in every `[BRACKET]` — the more specific you are, the better the output.
- If the tone is off, add one sentence: "Warmer," "More direct," "Shorter."
- Chain prompts: use the Bug Report Summary prompt first, then feed that output into the Escalation Note prompt.
- Save your best outputs as local examples to improve future prompts.

---

## Prompt Index

| # | File | Use Case |
|---|------|----------|
| 01 | `reply-to-angry-customer.md` | De-escalate and retain an upset customer |
| 02 | `escalation-note.md` | Hand off a complex case to a senior agent or manager |
| 03 | `bug-report-summary.md` | Distil a messy thread into a clear bug report for engineering |
| 04 | `refund-decision-template.md` | Write a refund decision with clear rationale |
| 05 | `follow-up-sequence.md` | Draft a 3-email follow-up sequence after a support interaction |
| 06 | `customer-onboarding-email.md` | Welcome a new customer and set them up for success |
| 07 | `feature-request-acknowledgement.md` | Acknowledge a feature request without over-promising |
| 08 | `csat-score-analysis.md` | Analyse a batch of CSAT scores and surface themes |
| 09 | `out-of-office-policy-note.md` | Communicate support hours and response-time expectations |
| 10 | `kb-article-draft.md` | Draft a knowledge base article from a resolved support thread |

---

## Folder Structure

```
sample-01/
├── README.md          <- You are here
├── index.md           <- One-line descriptions of all prompts
└── prompts/
    ├── reply-to-angry-customer.md
    ├── escalation-note.md
    ├── bug-report-summary.md
    ├── refund-decision-template.md
    ├── follow-up-sequence.md
    ├── customer-onboarding-email.md
    ├── feature-request-acknowledgement.md
    ├── csat-score-analysis.md
    ├── out-of-office-policy-note.md
    └── kb-article-draft.md
```
