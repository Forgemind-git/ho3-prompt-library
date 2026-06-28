# Project Manager Prompt Library

**Role:** Project Manager (Agile/Scrum)  
**Sample:** 02 of 05 — HO3: Prompt Library

---

## Problem Statement

Project managers spend hours writing the same documents over and over — sprint agendas, stakeholder updates, retrospective summaries, risk register entries. Each one is important but time-consuming to produce from scratch, and inconsistent quality across PMs makes it hard to standardise how the team communicates with stakeholders.

This prompt library gives PMs a structured set of AI prompts that produce first-draft PM artefacts in minutes. Every prompt follows the CRISP framework to ensure the AI understands your project context, constraints, and quality bar before it writes a single word.

---

## Use it with your Claude.ai subscription
No API key needed. Just your normal Claude.ai login.

1. Open the file **`index.html`** from this folder in your web browser (double-click it). You'll see every PM prompt as a card.
2. Find the prompt you need (for example, *Stakeholder Status Update*) and click its **Copy** button.
3. Open **Claude.ai** in another tab and paste the prompt into the chat box.
4. Replace the `[BRACKET]` placeholders with your real project details, then press Enter.
5. Read Claude's draft, adjust it with your PM judgement, and use it. If it's too long, tell Claude "make it tighter".

Prefer reading the prompts as text? Open any file in the **`prompts/`** folder and copy the prompt from its **Full Prompt** section. No API key needed.

## What Is the CRISP Framework?

Every prompt in this library is built on **CRISP** — a five-part structure that eliminates ambiguity:

| Letter | Stands For | What It Does |
|--------|-----------|--------------|
| **C** | Context | Sets the scene — your project, team, sprint stage |
| **R** | Role | Tells the AI what PM expertise to adopt |
| **I** | Instruction | The core task — what the AI must produce |
| **S** | Spec | Output specifications — format, length, sections |
| **P** | Performance | The quality bar — what "done well" means for this artefact |

---

## How to Use This Library

1. **Browse `index.md`** to find the PM artefact you need.
2. **Open the relevant `.md` file** in the `prompts/` folder.
3. **Copy the full prompt text** from the "Full Prompt" section.
4. **Replace all `[BRACKET]` placeholders** with your actual project details.
5. **Paste into Claude** and review the draft.
6. **Adjust and refine** — the AI gives you 80% done; you bring the PM judgement.

### PM-Specific Tips
- The more project context you put in the `[BRACKET]` fields, the better the output — don't shortcut the Context section.
- For recurring prompts (sprint planning, retrospectives), save your filled-in version as a template for next sprint.
- Chain these prompts: use the Risk Register Entry prompt to populate the risk, then use the Stakeholder Status Update to reference it.

---

## Prompt Index

| # | File | Use Case |
|---|------|----------|
| 01 | `sprint-planning-agenda.md` | Structure a sprint planning session for a 2-week sprint |
| 02 | `stakeholder-status-update.md` | Write a concise stakeholder update that manages expectations |
| 03 | `risk-register-entry.md` | Document a new project risk with impact, likelihood, and mitigation |
| 04 | `retrospective-summary.md` | Summarise a sprint retrospective with clear actions |
| 05 | `meeting-action-items.md` | Extract and format action items from meeting notes |
| 06 | `scope-change-impact-note.md` | Document a scope change request with timeline and cost impact |
| 07 | `project-kickoff-brief.md` | Write a project kickoff brief that aligns all stakeholders |
| 08 | `vendor-evaluation-scorecard.md` | Create a scored vendor evaluation from a requirements list |
| 09 | `budget-variance-explanation.md` | Explain a budget variance clearly to non-financial stakeholders |
| 10 | `project-closure-report.md` | Write a project closure report that captures lessons learned |

---

## Folder Structure

```
sample-02/
├── README.md          <- You are here
├── index.md           <- One-line descriptions of all prompts
└── prompts/
    ├── sprint-planning-agenda.md
    ├── stakeholder-status-update.md
    ├── risk-register-entry.md
    ├── retrospective-summary.md
    ├── meeting-action-items.md
    ├── scope-change-impact-note.md
    ├── project-kickoff-brief.md
    ├── vendor-evaluation-scorecard.md
    ├── budget-variance-explanation.md
    └── project-closure-report.md
```
