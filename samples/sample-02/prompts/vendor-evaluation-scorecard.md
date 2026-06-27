# Prompt 08 — Vendor Evaluation Scorecard

**Library:** Project Manager Prompt Library  
**Role:** Project Manager (Agile/Scrum)

---

## Purpose

Create a weighted vendor evaluation scorecard from a requirements list and vendor information — so vendor selection is defensible, objective, and documented rather than based on who gave the best demo.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Evaluating vendors for [product/service]. Budget: [$X/year]. Vendors being evaluated: [list 2–4]. Key requirements: [list]. Evaluation team: [roles who will score]. |
| **Role** | You are a PM who runs vendor evaluations that procurement teams trust because they are structured, weighted by business priority, and produce a clear recommendation with a documented rationale. |
| **Instruction** | Create a weighted scorecard with criteria derived from the requirements, score each vendor on 1–5 scale, calculate weighted scores, produce a ranked result table, and write a one-paragraph recommendation. |
| **Spec** | Scorecard table format. Criteria must have weights that total 100%. Scores 1–5 with definitions (1=does not meet, 3=meets, 5=exceeds). Weighted score = score x weight. Recommendation in one paragraph. |
| **Performance** | A procurement team can use this scorecard in a vendor selection meeting. The recommendation is supported by the scores and explains any trade-offs. |

---

## Full Prompt

```
Context: I'm evaluating vendors for [product/service] at [Company]. Budget: $[X] per year. Contract duration: [N years]. Decision needed by: [date].

Vendors being evaluated:
1. [Vendor A name] — brief description
2. [Vendor B name] — brief description
3. [Vendor C name] — brief description

Key requirements (I'll provide these — you assign weights based on business priority):
- [Requirement 1]
- [Requirement 2]
- [Requirement 3]
- [Requirement 4]
- [Requirement 5]

Information about each vendor:
[Paste vendor information here — from demos, RFP responses, or your notes]

Role: Act as a PM who runs objective vendor evaluations that produce defensible, documented recommendations. You assign criteria weights that reflect actual business priorities, not equal weighting.

Instruction: Using the requirements and vendor information above:
1. Create weighted evaluation criteria (must total 100%) based on the requirements provided; explain the weight rationale briefly
2. Score each vendor on each criterion (1–5 scale) with a one-line justification
3. Calculate weighted scores for each vendor
4. Produce a ranked results table
5. Write a recommendation paragraph that: states the recommended vendor, explains why, and acknowledges the top trade-off

Spec:
- Scorecard as a table (criteria | weight | Vendor A | Vendor B | Vendor C)
- Score definitions: 1=fails to meet, 2=partially meets, 3=meets, 4=exceeds in one area, 5=clearly exceeds
- Weights must total 100%
- Separate justification per score per vendor
- Recommendation: one clear paragraph, 100 words max

Performance bar: A procurement panel can defend this selection to a CFO. The recommendation explains trade-offs honestly. Scoring rationale prevents "we just liked their demo" decisions.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Compare three CRM vendors.

**Output produced:**
> Vendor A, B, and C all offer CRM features. Vendor A is expensive but has good features. Vendor B is cheaper. Vendor C has mixed reviews. You should consider your budget and needs when making a decision.

**Why it's weak:** No scores, no weights, no criteria, "consider your budget" is useless. A procurement committee cannot use this to make a defensible decision.

---

## After Example (With CRISP)

**Placeholders filled:**
- Product: CRM platform | Budget: $24,000/year
- Vendors: HubSpot Enterprise, Salesforce Professional, Pipedrive Advanced
- Requirements: Contact migration tool, marketing integration, mobile app, reporting, support SLA

**Output produced:**

> **Vendor Evaluation Scorecard — CRM Platform**  
> Evaluated by: James Reid (PM) | Date: June 27, 2025 | Budget: $24,000/year
>
> **Criteria and Weights**
>
> | Criterion | Weight | Rationale |
> |-----------|--------|-----------|
> | Data migration tooling | 30% | Highest priority — poor migration = project failure |
> | Marketing integration | 25% | Core use case for CMO sponsorship |
> | Reporting and dashboards | 20% | Sales leadership requirement |
> | Mobile app quality | 15% | Field sales team; requested explicitly |
> | Support SLA | 10% | Important but manageable with any tier-1 vendor |
>
> **Scores (1–5)**
>
> | Criterion | Weight | HubSpot | Salesforce | Pipedrive |
> |-----------|--------|---------|------------|-----------|
> | Data migration tooling | 30% | 5 | 4 | 2 |
> | Marketing integration | 25% | 5 | 3 | 3 |
> | Reporting and dashboards | 20% | 4 | 5 | 3 |
> | Mobile app quality | 15% | 4 | 4 | 4 |
> | Support SLA | 10% | 3 | 5 | 3 |
> | **Weighted Total** | **100%** | **4.45** | **3.95** | **2.90** |
>
> **Result Ranking:** 1st HubSpot (4.45) | 2nd Salesforce (3.95) | 3rd Pipedrive (2.90)
>
> **Recommendation**  
> HubSpot Enterprise is the recommended vendor. It scores highest on the two most heavily weighted criteria — migration tooling and marketing integration — which are the primary success factors for this project. The trade-off is Support SLA (scored 3 vs Salesforce's 5), but HubSpot's Enterprise tier includes a dedicated CSM which mitigates this in practice. Salesforce would be the choice if reporting depth were the top priority, but it is not for this project scope.
