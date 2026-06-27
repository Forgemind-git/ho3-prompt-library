# Prompt 10 — Financial Model Assumption Check

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Review and document the assumptions in a financial model to identify which ones carry the most risk, which are well-supported vs weakly-justified, and what the sensitivity of the model output is to each key assumption — creating an assumption quality audit trail.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Model: [type and purpose — DCF / 3-year operating model / unit economics model]. Key assumptions to review: [list the main input assumptions]. Model output the assumptions drive: [what number is the final output — valuation, EBITDA, breakeven date]. |
| **Role** | You are a finance analyst conducting a pre-distribution assumption review — you are the last line of quality control before this model goes to a CFO, investor, or board, and you take that seriously. |
| **Instruction** | Review the listed assumptions and produce: an assumption quality assessment (well-supported / partially supported / weakly supported), sensitivity analysis for the top 3 assumptions, and a list of assumptions that need strengthening before the model is distributed. |
| **Spec** | Assumption review table. Quality rating for each assumption with brief rationale. Sensitivity analysis: what happens to the output if the assumption changes by +/- 10%, +/- 20%. Flagged assumptions with recommended improvement. |
| **Performance** | A CFO reviewing this check can see immediately which assumptions are solid and which need more work. The sensitivity table shows which assumptions could sink or transform the model outcome. |

---

## Full Prompt

```
Context: I'm conducting a pre-distribution review of a [model type — e.g., "3-year revenue model", "LBO model", "unit economics model", "DCF valuation"] for [Company Name]. The model's primary output is: [e.g., "FY2027 EBITDA of $4.2M" / "Enterprise valuation of $42M" / "Breakeven date of Q3 2026"].

Key assumptions in the model (list each one I should review):
1. [Assumption 1 — e.g., "Revenue growth: 35% YoY for 3 years"]
2. [Assumption 2 — e.g., "Gross margin: 78% stable across all 3 years"]
3. [Assumption 3 — e.g., "CAC: $12,000 flat, with LTV of $48,000"]
4. [Add all major assumptions]

For each assumption, note:
- What data or rationale backs it (or note "not documented")
- Whether it has been sense-checked against industry benchmarks or historical actuals

Model audience: [CFO only / investor presentation / board approval / M&A due diligence]

Role: Act as a finance analyst doing a pre-distribution assumption quality review. You are the last quality gate before this model goes to an audience that will scrutinise every number — and you take that responsibility seriously.

Instruction: Produce an assumption quality review with:
1. Assumption Quality Table — for each assumption: rating (Well-Supported / Partially Supported / Weakly Supported), basis (what backs it), risk note (what could go wrong if this assumption is wrong)
2. Top 3 Sensitivity Analysis — for the three most impactful assumptions: show model output if assumption is -20%, -10%, base case, +10%, +20%
3. Assumptions Needing Strengthening — flagged list of assumptions rated Weakly Supported, with specific recommendations for how to improve the backing
4. Reviewer Sign-Off Note — a summary statement suitable for including in the model documentation

Spec:
- Assumption quality table with ratings
- Sensitivity table for top 3
- Flagged list with specific improvement actions
- 350–400 words for non-table sections
- Reviewer note: 50 words max

Performance bar: CFO can see which assumptions are solid and which need work in under 5 minutes. Sensitivity table shows which assumptions are model-threatening. Flagged items have specific improvement actions.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Check my financial model assumptions.

**Output produced:**
> The assumptions in your model should be reviewed carefully. Make sure they are realistic and supported by data. Consider doing a sensitivity analysis on your key assumptions. It's important that your model assumptions are defensible.

**Why it's weak:** Tells the analyst to do the work without doing it. No structure, no ratings, no sensitivity, no specific flags. "Make sure they are realistic" is advice, not a review.

---

## After Example (With CRISP)

**Assumptions provided:**
- Revenue growth: 35% YoY (backed by H1 actuals)
- Gross margin: 78% stable (partially backed — H1 actual 79%)
- CAC: $12,000 (industry benchmark, not company-specific data)
- LTV: $48,000 (based on 24-month average contract, no churn adjustment)
- Headcount cost: $120K avg fully-loaded (2023 data)

**Output produced:**

> **Financial Model Assumption Review — Helply 3-Year Revenue Model**  
> Reviewed by: James Reid | Date: June 27, 2025 | Model output: FY2027 EBITDA $4.2M
>
> **Assumption Quality Assessment**
>
> | Assumption | Value | Rating | Basis | Risk Note |
> |-----------|-------|--------|-------|-----------|
> | Revenue growth (YoY) | 35% | Well-Supported | H1 2025 run-rate implies 32%; Enterprise pipeline adds 3–4% | Weakens if Enterprise pilot conversion <50%; model shows 28% growth in bear case |
> | Gross margin | 78% | Partially Supported | H1 actual was 79%; assumes 1pt step-down for scale | No infrastructure cost model at projected revenue; may be optimistic at $15M+ ARR |
> | CAC | $12,000 | Weakly Supported | Industry benchmark (Bessemer SaaS report); no internal data | Actual CAC may vary significantly by segment; Enterprise CAC is 3–5x SMB — a blended assumption may mislead |
> | LTV | $48,000 | Weakly Supported | 24-month avg contract × ACV; no churn adjustment | LTV without a churn assumption is not LTV — this is ACV × contract length. Needs churn rate applied |
> | Headcount cost (fully-loaded) | $120K avg | Partially Supported | Based on 2023 actual; 2 years old | Compensation benchmarks have moved; validate against 2025 offers and Levels.fyi data |
>
> **Top 3 Sensitivity Analysis**
>
> | Assumption | -20% | -10% | Base | +10% | +20% |
> |-----------|------|------|------|------|------|
> | Revenue growth (35%) | 28% → EBITDA $2.1M | 31.5% → $3.1M | 35% → **$4.2M** | 38.5% → $5.4M | 42% → $6.7M |
> | Gross margin (78%) | 62.4% → EBITDA $1.8M | 70.2% → $3.0M | 78% → **$4.2M** | 85.8% → $5.4M | 93.6% → model overstated |
> | CAC ($12K) | $9.6K → EBITDA $4.8M | $10.8K → $4.5M | $12K → **$4.2M** | $13.2K → $3.9M | $14.4K → $3.6M |
>
> **Assumptions Needing Strengthening (before CFO/Investor distribution)**
>
> 1. **LTV ($48,000):** Add churn rate to calculation. Formula should be: LTV = ACV ÷ Annual Churn Rate. At 12% churn and $24K ACV, true LTV = $200K, not $48K. The current assumption understates LTV — which would actually improve the model, but needs to be correctly calculated.
> 2. **CAC ($12,000):** Replace industry benchmark with internal data. Use actual sales and marketing spend ÷ new logos from the last 4 quarters. Segment by SMB vs Enterprise — blended CAC hides a significant difference.
> 3. **Headcount cost ($120K):** Update to 2025 compensation data. Run against the last 6 months of payroll actuals, not 2023 data. Two years of salary inflation may have moved this by 10–15%.
>
> **Reviewer Sign-Off Note**  
> This model is conditionally appropriate for CFO review. LTV methodology and CAC sourcing require correction before external distribution. Revenue growth and gross margin assumptions are reasonable but carry scenario risk documented above. Three items flagged above must be addressed before investor presentation.
