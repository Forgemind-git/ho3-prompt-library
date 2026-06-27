# Prompt 08 — Excel Formula Explainer

**Library:** Financial Analyst Prompt Library  
**Role:** Financial Analyst (corporate finance)

---

## Purpose

Explain a complex Excel or Google Sheets formula in plain language — breaking down what each part does, why the formula is structured that way, and what to watch out for — so a non-technical colleague can use and maintain the formula confidently.

---

## CRISP Breakdown

| Element | Content |
|---------|---------|
| **Context** | Formula: [paste the exact formula]. Spreadsheet context: [what the sheet is tracking, what the formula is supposed to calculate]. Audience: [someone who uses Excel but has never written this kind of formula]. |
| **Role** | You are a finance analyst who teaches Excel by breaking formulas into understandable parts — you don't just say "it works," you explain the logic so the person can modify it if needed. |
| **Instruction** | Explain the formula with: plain language description of what it does, a component-by-component breakdown, the logic of how the components work together, common errors to watch for, and when you would use a different approach. |
| **Spec** | Explainer format. Component breakdown uses the exact formula syntax. No Excel jargon without explanation. One modification example to show the person how to adapt it. 300 words max. |
| **Performance** | The person can read this explanation and modify the formula for a slightly different use case without asking for help. They understand why the formula is structured the way it is, not just what it produces. |

---

## Full Prompt

```
Context: I need to explain the following Excel/Google Sheets formula to [audience — e.g., "a marketing manager who uses Excel but hasn't written complex formulas", "a new finance analyst joining the team", "a business analyst who needs to maintain this model"]. 

The formula is:
[PASTE THE EXACT FORMULA HERE]

What the formula is trying to calculate:
[Describe in plain English what this formula should produce — e.g., "It should return the monthly recurring revenue for any customer that is currently active and on an annual plan"]

Spreadsheet context:
- The formula is in column: [e.g., "Column F — Monthly Revenue"]
- Key columns referenced: [e.g., "Column A = Customer Name, Column B = Plan Type, Column C = Contract Value, Column D = Status"]

Role: Act as a finance analyst who explains Excel formulas as a teacher, not a manual. You explain the logic behind the structure, not just what each function is named.

Instruction: Write an Excel formula explanation with:
1. Plain English Summary — what does this formula do, in one sentence
2. Component Breakdown — break the formula into parts, explain each one in plain language (what function, what it's looking for, what it returns)
3. How the Parts Work Together — explain the logic of how the components combine to produce the result
4. Common Errors — 2–3 things that could break this formula or produce incorrect results, and how to spot them
5. Modification Example — show how you'd change one thing about the formula to handle a slightly different scenario

Spec:
- Explainer format with bold headers
- Component breakdown uses exact formula syntax in backticks
- No Excel jargon without immediate plain-language explanation
- 300 words maximum
- One modification example

Performance bar: Reader can modify the formula for a similar use case without further help. They understand WHY it's structured this way, not just WHAT it does.
```

---

## Before Example (Weak Prompt)

**Prompt used:**
> Explain this Excel formula: =SUMIFS(C:C,B:B,"Annual",D:D,"Active")

**Output produced:**
> This formula uses SUMIFS to sum values. SUMIFS sums a range based on multiple criteria. It will sum column C where column B equals "Annual" and column D equals "Active."

**Why it's weak:** Just restates the formula in slightly different words. "Will sum column C" doesn't explain what the person is looking at. No error guidance. No modification example. Someone who doesn't understand SUMIFS still doesn't understand it.

---

## After Example (With CRISP)

**Formula provided:**
```
=IFERROR(SUMIFS(C:C,B:B,"Annual",D:D,"Active")/12,"—")
```

**Context:** Column C = Annual Contract Value, Column B = Plan Type, Column D = Customer Status. This calculates monthly revenue contribution from all active annual plan customers.

**Output produced:**

> **Excel Formula Explanation**  
> Formula: `=IFERROR(SUMIFS(C:C,B:B,"Annual",D:D,"Active")/12,"—")`
>
> **Plain English Summary**  
> This formula adds up all contract values for customers who are on an "Annual" plan AND have "Active" status, then divides by 12 to convert annual value to a monthly figure. If anything goes wrong, it shows a dash instead of an error.
>
> **Component Breakdown**
>
> - `SUMIFS(C:C, B:B,"Annual", D:D,"Active")` — this is the engine. It looks at every row and only adds the value in Column C if Column B says "Annual" AND Column D says "Active". Both conditions must be true. If either is missing, that row is excluded.
>
> - `/12` — divides the result by 12 to convert annual contract value into a monthly revenue figure.
>
> - `IFERROR(...,"—")` — wraps the whole formula. If SUMIFS hits an error (e.g., empty columns, a reference problem), it shows "—" instead of showing a confusing error code.
>
> **How the Parts Work Together**  
> SUMIFS filters and totals → divide by 12 converts to monthly → IFERROR catches any failures silently. The result is: monthly revenue from active annual customers only.
>
> **Common Errors**
> 1. **Typo in criteria:** "Annual" is case-sensitive in some systems. If someone typed "annual" or "ANNUAL" in Column B, those rows are excluded. Check with `=COUNTIF(B:B,"Annual")` to see how many rows match.
> 2. **Column range mismatch:** All three column references (`C:C`, `B:B`, `D:D`) must cover the same number of rows. If Column C only goes to row 100 but Column B goes to row 200, SUMIFS may give wrong results.
> 3. **"Active" status variation:** If Column D contains "active" (lowercase), "ACTIVE" (uppercase), or trailing spaces, the formula misses those rows.
>
> **Modification Example**  
> To calculate the same thing for Monthly plan customers instead of Annual:  
> `=IFERROR(SUMIFS(C:C,B:B,"Monthly",D:D,"Active"),0)`  
> Two changes: "Annual" → "Monthly" in the criteria, and divide-by-12 is removed (monthly values are already monthly). Also changed "—" to 0 for easier use in further calculations.
