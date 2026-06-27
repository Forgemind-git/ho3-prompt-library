# Financial Analyst Prompt Library

**Role:** Financial Analyst (corporate finance)  
**Sample:** 05 of 05 — HO3: Prompt Library

---

## Problem Statement

Financial analysts spend significant time producing written outputs that non-finance stakeholders need to understand: board narratives, budget commentaries, variance explanations, investor updates, and audit prep documents. The technical analysis takes skill — but the communication of that analysis to a CFO, board member, or investor often gets rushed, resulting in outputs that are technically correct but hard to act on.

This prompt library gives corporate finance analysts a structured set of AI prompts for every major written finance communication task. Every prompt uses the CRISP framework to ensure the AI understands the financial context, the audience's level of sophistication, and the quality bar before it drafts a single word.

**Important:** These prompts produce written communications about financial data. They do not perform financial modelling or calculations. Always verify any numbers, and have the relevant financial professional review outputs before distribution.

---

## What Is the CRISP Framework?

| Letter | Stands For | What It Does |
|--------|-----------|--------------|
| **C** | Context | Your company, financial data, and communication situation |
| **R** | Role | The financial communication expertise the AI adopts |
| **I** | Instruction | The specific document or communication to produce |
| **S** | Spec | Format, length, audience sophistication level, tone |
| **P** | Performance | What a well-written finance communication looks like |

---

## How to Use This Library

1. **Browse `index.md`** to find the finance communication you need.
2. **Open the prompt file** in `prompts/`.
3. **Copy the full prompt text** and fill in the financial data in the `[BRACKET]` fields.
4. **Paste into Claude** and review the draft.
5. **Edit for accuracy** — check every number, and have a qualified finance professional review before distribution.

### Finance-Specific Notes
- Always populate the financial data fields with your actual numbers before using any output.
- AI outputs should be first drafts — review every number, ratio, and claim.
- For board or investor communications, always have the CFO or finance controller review before sending.
- Do not share confidential financial data with any AI tool without confirming your company's data policy.

---

## Prompt Index

| # | File | Use Case |
|---|------|----------|
| 01 | `variance-analysis-explanation.md` | Explain a budget vs actual variance clearly to non-financial stakeholders |
| 02 | `board-slide-narrative.md` | Write the narrative script for financial board slides |
| 03 | `budget-commentary-draft.md` | Draft a monthly or quarterly budget commentary |
| 04 | `forecast-assumption-doc.md` | Document forecast assumptions in a structured, auditable format |
| 05 | `cost-saving-proposal.md` | Write a cost-saving proposal with ROI and implementation plan |
| 06 | `audit-prep-checklist.md` | Create a structured audit preparation checklist |
| 07 | `kpi-definition-card.md` | Define a KPI with formula, data source, owner, and interpretation guide |
| 08 | `excel-formula-explainer.md` | Explain a complex Excel formula in plain language for a non-technical audience |
| 09 | `investor-update-bullets.md` | Write concise investor update bullet points for a monthly/quarterly update |
| 10 | `financial-model-assumption-check.md` | Review and document financial model assumptions for an audit trail |

---

## Folder Structure

```
sample-05/
├── README.md          <- You are here
├── index.md           <- One-line descriptions of all prompts
└── prompts/
    ├── variance-analysis-explanation.md
    ├── board-slide-narrative.md
    ├── budget-commentary-draft.md
    ├── forecast-assumption-doc.md
    ├── cost-saving-proposal.md
    ├── audit-prep-checklist.md
    ├── kpi-definition-card.md
    ├── excel-formula-explainer.md
    ├── investor-update-bullets.md
    └── financial-model-assumption-check.md
```
