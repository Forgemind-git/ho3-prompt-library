# People Manager Prompt Library

**Role:** People Manager (team of 8)  
**Sample:** 03 of 05 — HO3: Prompt Library

---

## Problem Statement

Managing people is the highest-leverage thing a manager does — and also the thing most managers say they don't have time to do well. Writing a thorough performance review, preparing for a difficult conversation, or drafting a meaningful recognition note takes time that gets deprioritised when the week gets busy.

This prompt library gives people managers a structured set of AI prompts for every people management artefact — from 1:1 prep notes to PIP outlines to hiring rubrics. Every prompt follows the CRISP framework to produce first drafts that are human, specific, and ready to refine.

---

## What Is the CRISP Framework?

| Letter | Stands For | What It Does |
|--------|-----------|--------------|
| **C** | Context | Sets the scene — who the team member is, what's going on |
| **R** | Role | Tells the AI what management expertise to adopt |
| **I** | Instruction | The core task — what the AI must produce |
| **S** | Spec | Output format, length, tone constraints |
| **P** | Performance | The quality bar — what "good" looks like for this situation |

---

## How to Use This Library

1. **Browse `index.md`** to find the artefact you need.
2. **Open the prompt file** in `prompts/`.
3. **Copy the full prompt text** and fill in all `[BRACKET]` placeholders.
4. **Paste into Claude** and review the output.
5. **Edit with your own knowledge** of the person — the AI provides the structure and language; you provide the human context.

### Important Note on People Prompts
Always add your own specific examples and observations to the AI output. The AI provides structure and professional language — you bring the actual knowledge of the person. Never use an AI-generated performance review without personalising it with your own evidence.

---

## Prompt Index

| # | File | Use Case |
|---|------|----------|
| 01 | `one-on-one-prep-notes.md` | Prepare structured 1:1 notes with talking points and goals |
| 02 | `performance-review-draft.md` | Draft a balanced, evidence-based performance review |
| 03 | `constructive-feedback-script.md` | Write a feedback script for a specific behaviour |
| 04 | `team-recognition-note.md` | Write a meaningful recognition note for an individual or team |
| 05 | `pip-outline.md` | Draft a Performance Improvement Plan outline |
| 06 | `job-levelling-rationale.md` | Write a promotion or levelling rationale with evidence |
| 07 | `offboarding-checklist.md` | Create a structured offboarding plan for a departing team member |
| 08 | `hiring-rubric.md` | Design an interview evaluation rubric for a specific role |
| 09 | `team-okr-draft.md` | Draft quarterly OKRs for a team with measurable key results |
| 10 | `difficult-conversation-script.md` | Write a script for a difficult conversation with a team member |

---

## Folder Structure

```
sample-03/
├── README.md          <- You are here
├── index.md           <- One-line descriptions of all prompts
└── prompts/
    ├── one-on-one-prep-notes.md
    ├── performance-review-draft.md
    ├── constructive-feedback-script.md
    ├── team-recognition-note.md
    ├── pip-outline.md
    ├── job-levelling-rationale.md
    ├── offboarding-checklist.md
    ├── hiring-rubric.md
    ├── team-okr-draft.md
    └── difficult-conversation-script.md
```
