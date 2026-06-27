# Prompt 09 — Team OKR Draft

**Library:** People Manager Prompt Library  
**Role:** People Manager (team of 8)

---

## Purpose

Draft quarterly OKRs for a team with ambitious but achievable Objectives and Key Results that are genuinely measurable — not the "improve team performance" objectives that make OKR coaches cry.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Team: [name and function]. Quarter: [Q# Year]. Company-level OKRs or priorities this quarter: [list them — team OKRs must ladder up]. Team size: [N]. Biggest challenges or focus areas: [list]. |
| **Role** | You are a manager who has written OKRs that actually drive behaviour — because the Key Results have real numbers, clear ownership, and a 60–70% target attainment expectation (they should be stretchy). |
| **Instruction** | Write 3 Objectives with 3 Key Results each. Each KR must: have a baseline, a target, and a measurement method. Objectives should be qualitative and inspiring; KRs should be quantitative and specific. |
| **Spec** | OKR format: Objective as a statement, Key Results as numbered bullets. KR format: "[Metric] from [baseline] to [target] by [date], measured by [method]." 250–300 words. |
| **Performance** | At the end of the quarter, any team member can score each KR without asking the manager what it means. All three Objectives ladder to at least one company priority. None of the KRs are 100% achievable — they stretch. |

---

## Full Prompt

```
Context: I'm drafting Q[N] [Year] OKRs for the [Team Name] team ([function description]). Team size: [N people]. Quarter runs: [start date] to [end date].

Company-level priorities this quarter (our OKRs must ladder to at least one of these):
1. [Company priority 1]
2. [Company priority 2]
3. [Company priority 3]

Our team's biggest focus areas or challenges this quarter:
1. [Focus 1]
2. [Focus 2]
3. [Focus 3]

Last quarter: we hit [X of Y] OKRs. Our weakest area was [describe]. Our strongest was [describe].

Role: Act as a manager who writes OKRs that actually drive quarterly behaviour — with Key Results that have real numbers, clear measurement methods, and a 60–70% expected attainment (stretchy, not sandbagged).

Instruction: Write 3 Objectives with 3 Key Results each, following these rules:
- Objectives: qualitative, inspiring, 1 sentence
- Key Results: quantitative, format = "[Metric] from [baseline] to [target] by [end date], measured by [method]"
- Each Objective must ladder to at least one company priority (note which one)
- No KR should be 100% guaranteed — they should require stretch
- Baseline must be stated (not "increase X" without saying from what)

Spec:
- OKR format (Objective as header, KRs as numbered bullets)
- 250–300 words
- Each KR: baseline → target → measurement method
- Laddering note per Objective
- No KR uses the word "improve" without a number

Performance bar: Any team member can self-score each KR at quarter-end without asking what it means. OKRs clearly ladder to company priorities. Targets require genuine effort to hit.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Write OKRs for my engineering team.

**Output produced:**
> Objective 1: Improve code quality. KR1: Write better code. KR2: Reduce bugs. KR3: Improve review process. Objective 2: Ship faster. KR1: Deliver features on time. KR2: Improve sprint velocity.

**Why it's weak:** No baselines, no targets, no measurement methods. "Write better code" is not a KR. "Deliver features on time" — what percentage? From what baseline? These OKRs cannot be scored at quarter-end.

---

## After Example (With CRISP)

**Placeholders filled:**
- Team: Backend Engineering (5 developers)
- Q3 2025 | Jul 1 – Sep 30
- Company priorities: Reliability, faster feature delivery, customer retention
- Focus areas: Reduce incident rate, ship payment v2, improve onboarding experience

**Output produced:**

> **Q3 2025 OKRs — Backend Engineering Team**
>
> ---
>
> **Objective 1: Make our platform so reliable that customers stop thinking about it**  
> *(Ladders to: Company Priority — Reliability)*
>
> 1. Reduce P1/P2 incident rate from 3.2 incidents/month (Q2 avg) to 1.5 or fewer by Sep 30, measured by PagerDuty monthly report
> 2. Achieve mean time to recovery (MTTR) under 45 minutes for all P1 incidents by Sep 30, measured by incident log (baseline: 78 min in Q2)
> 3. Complete reliability review and remediation for 100% of "single point of failure" services identified in Q2 audit (6 services) by Aug 31
>
> ---
>
> **Objective 2: Ship Payment v2 and prove we can deliver complex features without drama**  
> *(Ladders to: Company Priority — Faster Feature Delivery)*
>
> 1. Payment v2 live in production by Aug 22, with zero P1 issues in the first 2 weeks post-launch
> 2. Reduce sprint story carryover rate from 18% (Q2 avg) to 8% or below by end of Q3, measured by Jira sprint reports
> 3. All Payment v2 features have automated regression test coverage of 90%+ before release, measured by coverage report in CI pipeline
>
> ---
>
> **Objective 3: Make the first 30 days better for every new customer**  
> *(Ladders to: Company Priority — Customer Retention)*
>
> 1. Reduce backend API errors on the onboarding flow from 4.2% error rate to under 1.5% by Aug 15, measured by error monitoring dashboard
> 2. Cut average onboarding setup time (time from signup to first active session) from 4.2 days to 2.5 days by Sep 30, measured by product analytics
> 3. Instrument 3 new onboarding funnel events in analytics by Jul 31 to give product team visibility into drop-off points
