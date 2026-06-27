# Prompt 06 — Audit Prep Checklist

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Build a structured audit preparation checklist with task owners, evidence requirements, and deadlines — so the finance team walks into audit fieldwork with everything ready, rather than scrambling to produce documents during the audit itself.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Audit type: [statutory annual audit / internal audit / tax audit / SOC 2 / due diligence]. Company: [name, stage]. Audit period: [dates]. Auditor: [firm name]. Fieldwork dates: [start date]. Team: [who is responsible — finance team size and roles]. |
| **Role** | You are a financial controller who has been through multiple audits and knows that audit readiness is won or lost in the preparation phase, not during fieldwork. |
| **Instruction** | Create an audit prep checklist with: categories of documents needed, specific evidence items per category, named owner per item, format required, and deadline (relative to fieldwork start date). |
| **Spec** | Checklist table format. Categories: Financial Statements / Revenue / Costs / Payroll / Fixed Assets / Cash / Compliance / Other. Each item: description, format, owner, deadline. 300–350 words. |
| **Performance** | Finance team enters audit fieldwork with 100% of items on the checklist complete. Auditor does not have to chase for standard documents. No item has "TBD" for owner. |

---

## Full Prompt

```
Context: I'm a financial analyst preparing for [audit type — e.g., "FY2025 statutory annual audit" / "Q2 internal audit" / "Series B due diligence"]. 
- Company: [name, industry, stage]
- Audit period: [dates being audited]
- Auditor: [firm name or "internal audit team"]
- Fieldwork start date: [date]
- Finance team: [list roles available to own tasks — e.g., "Controller, 2 analysts, 1 AP/AR coordinator"]
- Known areas of complexity or risk: [e.g., "revenue recognition for multi-year contracts", "stock options accounting", "intercompany transactions"]

Role: Act as a financial controller who has run 10+ audits and knows that the preparation phase determines audit quality more than anything that happens during fieldwork.

Instruction: Build an audit preparation checklist with:
1. Task Categories — standard categories appropriate to the audit type
2. Specific Tasks — for each category, list the specific documents or evidence items needed
3. Format Required — what the auditor needs (PDF, Excel with formulas, signed copy, etc.)
4. Named Owner — specific role from the team provided (no "TBD")
5. Deadline — expressed as days before fieldwork start (e.g., "D-10" = 10 days before fieldwork)
6. Status Column — for the team to track (Pending / In Progress / Complete)

Also include:
- A pre-audit meeting agenda (15–20 min kick-off)
- Top 3 things most commonly requested during fieldwork that teams forget to prepare

Spec:
- Checklist table format
- Items per category: 3–6
- Every item has an owner (role from provided team)
- Deadlines expressed as D-minus days
- 300–350 words for non-table sections

Performance bar: Finance team enters fieldwork with 100% ready. Auditor doesn't chase for basic documents. No "TBD" owners.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Create an audit preparation checklist.

**Output produced:**
> Audit Prep Checklist: 1. Gather financial statements 2. Prepare trial balance 3. Have bank statements ready 4. Ensure all documents are organized 5. Be ready to answer auditor questions.

**Why it's weak:** No evidence specifics, no owners, no deadlines, "ensure all documents are organized" is meaningless, "be ready to answer questions" is not a preparation task. This checklist would be useless to any finance team.

---

## After Example (With CRISP)

**Placeholders filled:**
- FY2025 statutory annual audit | Helply | Auditor: Grant Thornton
- Fieldwork starts August 4, 2025
- Team: Controller (Sarah), Analyst (James), AP/AR Coordinator (Priya)
- Complex areas: Multi-year Enterprise contracts, employee equity grants

**Output produced:**

> **Audit Preparation Checklist — FY2025 Statutory Audit**  
> Auditor: Grant Thornton | Fieldwork: August 4, 2025 | Prepared: James Reid
>
> **Checklist**
>
> | Category | Item | Format Required | Owner | Deadline | Status |
> |---------|------|----------------|-------|----------|--------|
> | Financial Statements | Signed management accounts (Jan–Dec 2025) | PDF, signed by CFO | Controller (Sarah) | D-15 (Jul 20) | Pending |
> | Financial Statements | Trial balance (Dec 31, 2025) | Excel with formula cells unlocked | Analyst (James) | D-10 (Jul 25) | Pending |
> | Revenue | Revenue recognition schedule for multi-year Enterprise contracts | Excel with contract dates, ACV, recognition schedule | Analyst (James) | D-12 (Jul 23) | Pending |
> | Revenue | Signed contracts for all Enterprise customers (FY2025) | PDF, organised by customer | Controller (Sarah) | D-10 (Jul 25) | Pending |
> | Payroll | Payroll journal reconciliation (all 12 months) | Excel tied to bank statements | Controller (Sarah) | D-10 (Jul 25) | Pending |
> | Payroll | Equity grant schedule (options issued, vesting, exercised) | Excel with Black-Scholes inputs | Controller (Sarah) + CFO | D-7 (Jul 28) | Pending |
> | Cash | Bank statements (all accounts, all 12 months) | PDF from bank, certified | AP/AR (Priya) | D-14 (Jul 21) | Pending |
> | Cash | Bank reconciliations (monthly, all accounts) | Excel | Analyst (James) | D-10 (Jul 25) | Pending |
> | Fixed Assets | Fixed asset register with depreciation schedule | Excel | Analyst (James) | D-12 (Jul 23) | Pending |
> | Compliance | Confirmation of audit representation letter (draft for CFO) | Word doc for CFO signature | Controller (Sarah) | D-3 (Aug 1) | Pending |
> | Tax | Corporation tax workings and prior year correspondence | PDF | Controller (Sarah) | D-10 (Jul 25) | Pending |
>
> ---
>
> **Pre-Audit Team Kick-Off Agenda (30 min, Jul 18)**
> - Review checklist and confirm all owners (10 min)
> - Flag any items at risk of not being ready by deadline (10 min)
> - Review known complexity areas: multi-year contract revenue recognition, equity grants (10 min)
>
> **3 Things Teams Forget to Prepare**
> 1. **Management representation letter** — auditors always need this signed before they can issue the opinion; draft it early, it needs CFO/CEO signature
> 2. **Third-party confirmations** — bank confirmation letters need to be requested by the auditor from the bank with 2+ weeks lead time; flag to auditor on Day 1 of fieldwork prep
> 3. **Prior year audit adjustments** — pull the prior year audit file and list any adjustments made; auditors will check whether prior year issues recurred
