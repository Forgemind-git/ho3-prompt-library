# Prompt 04 — Forecast Assumption Document

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Document the assumptions underpinning a financial forecast in a structured, auditable format — so anyone who picks up the model in six months can understand why the numbers were set the way they were, and any change to an assumption can be traced back to its owner.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Forecast: [type — annual budget / quarterly reforecast / project model]. Company: [name, stage]. Period covered: [dates]. Key assumptions to document: [list the main drivers]. |
| **Role** | You are a financial planning analyst who knows that undocumented assumptions are a model risk — you document them with the rigour of someone who knows an auditor will review this in 12 months. |
| **Instruction** | Create a forecast assumption document with: assumption name, category, value/range, basis for the assumption, owner, sensitivity (how much does the forecast change if this assumption is wrong by 10%?), and last reviewed date. |
| **Spec** | Assumption register format. Table for structured fields. Brief narrative justification per assumption (2–3 sentences). Sensitivity column is required — not optional. |
| **Performance** | An auditor picks up this document 12 months after the forecast was built and can understand why every major assumption was made without interviewing anyone. Every assumption has an owner. |

---

## Full Prompt

```
Context: I'm documenting the assumptions for [Company Name]'s [forecast type — e.g., "FY2026 Annual Budget" / "Q3 2025 Reforecast" / "3-Year Strategic Plan"]. The forecast covers [period]. 

Key assumptions to document (list each one — the AI will structure them, you provide the inputs):
1. [Assumption 1 — e.g., "Revenue growth rate: 35% YoY"]
2. [Assumption 2 — e.g., "Gross margin: 78%"]
3. [Assumption 3 — e.g., "Headcount additions: 12 FTEs across Sales and Engineering"]
4. [Continue for all major assumptions]

For each assumption, provide where possible:
- The assumption value or range
- The basis for it (historical trend / market data / management decision / contract)
- Who owns it (which team or person is accountable)

Role: Act as a financial planning analyst who documents assumptions with auditor-grade rigour — you treat undocumented assumptions as a model risk, not an administrative task.

Instruction: Create a forecast assumption document with:
1. Document Header — company, forecast name, period, author, date, version
2. Assumption Register — for each assumption provided:
   - Assumption name and category (Revenue / Costs / Headcount / Other)
   - Value / range
   - Basis (2–3 sentences: what data or rationale justifies this number)
   - Owner (team or named individual)
   - Sensitivity: what happens to the forecast if this assumption is 10% higher or lower
   - Last reviewed date
3. Key Risks Section — top 3 assumptions where the sensitivity impact is highest
4. Revision Log — table for tracking future changes to assumptions

Spec:
- Assumption register as a table
- Basis in 2–3 sentences per assumption (not a single word)
- Sensitivity column required for all assumptions
- 300–350 words for the narrative sections
- Formal document format with version control

Performance bar: An auditor 12 months from now understands why every assumption was made without interviewing anyone. Every assumption has an owner. Sensitivity is quantified, not described as "high/low."
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Document the assumptions for our financial forecast.

**Output produced:**
> Forecast Assumptions: Revenue growth rate: 35%. Gross margin: 78%. Headcount: 12 new hires. These assumptions are based on historical performance and management expectations.

**Why it's weak:** No basis, no owner, no sensitivity, "historical performance and management expectations" is a placeholder not an explanation. An auditor asking "why 35%?" would find no answer in this document.

---

## After Example (With CRISP)

**Assumptions provided:**
- Revenue growth: 35% YoY (based on H1 run-rate + Enterprise pipeline)
- Gross margin: 78% (H1 actual 79%, step-down for infra scaling)
- Headcount: +12 FTEs (approved by CEO in May board meeting)
- CAC payback: 14 months (historical average 16 months, improved mix toward Enterprise)

**Output produced:**

> **FORECAST ASSUMPTION DOCUMENT**  
> Company: Helply | Forecast: FY2026 Annual Budget | Period: Jan–Dec 2026  
> Author: James Reid, Financial Analyst | Date: June 27, 2025 | Version: 1.0
>
> ---
>
> **Assumption Register**
>
> | # | Assumption | Category | Value | Basis | Owner | Sensitivity (+/-10%) | Last Reviewed |
> |---|-----------|---------|-------|-------|-------|---------------------|---------------|
> | A01 | Revenue growth rate | Revenue | 35% YoY | H1 2025 run-rate implies 32% growth; Enterprise pipeline adds 3–4 points if 60% of pilots convert. Based on 12 months of actuals and signed Enterprise pilot agreements. | VP Sales | ±$820K in revenue at 10% sensitivity | Jun 2025 |
> | A02 | Gross margin | Revenue/Costs | 78% | H1 2025 actual was 79.2%. Assumed 1.2% step-down to reflect planned infrastructure scaling for Enterprise capacity. Historical range: 76–80%. | VP Engineering + CFO | ±$410K in EBITDA at 1% point sensitivity | Jun 2025 |
> | A03 | Headcount additions | Costs | +12 FTEs | Approved by CEO and board in May 2025 board meeting (minute reference: BM-2025-05-18). Split: 5 Sales, 4 Engineering, 2 Customer Success, 1 Finance. Hiring plan finalized June 15. | People Ops | ±$180K per FTE above/below plan (avg fully-loaded cost) | Jun 2025 |
> | A04 | CAC payback period | Revenue/Commercial | 14 months | Historical CAC payback average: 16 months (FY2024). 14-month assumption reflects shift to Enterprise (higher ACV, longer sales cycle but better unit economics). Based on Enterprise pilot data from Q1–Q2 2025. | VP Sales + CFO | ±2 months has $0 direct P&L impact but affects cash flow timing by ~$200K | Jun 2025 |
>
> ---
>
> **Key Risks**
> 1. **A01 (Revenue growth)** — Highest sensitivity assumption. If Enterprise pilot conversion rate falls below 40% (vs 60% assumed), revenue growth is 30% not 35% — a $820K shortfall.
> 2. **A03 (Headcount)** — If hiring pace lags (common in engineering), cost variance is favorable but revenue growth may be impacted by under-capacity.
> 3. **A02 (Gross margin)** — Infrastructure cost is difficult to predict precisely at scale; 1% margin variance = $410K EBITDA impact.
>
> **Revision Log**
>
> | Date | Assumption | Change | Reason | Author |
> |------|-----------|--------|--------|--------|
> | — | — | — | — | — |
