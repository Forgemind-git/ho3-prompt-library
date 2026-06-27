# Content Marketer Prompt Library

**Role:** Content Marketing Manager  
**Sample:** 04 of 05 — HO3: Prompt Library

---

## Problem Statement

Content marketers face a brutal paradox: they need to produce more content across more channels than ever, while maintaining the quality and strategic coherence that actually drives results. The result is either volume without quality — generic posts that get ignored — or quality without volume — a bottleneck that kills momentum.

This prompt library gives content marketers a structured set of AI prompts that produce high-quality first drafts of every major content type: blog posts, LinkedIn thought leadership, email newsletters, case studies, social media, SEO content, and more. Every prompt is built on the CRISP framework to ensure the AI understands your brand, audience, goals, and quality bar before it writes anything.

---

## What Is the CRISP Framework?

| Letter | Stands For | What It Does |
|--------|-----------|--------------|
| **C** | Context | Your brand, audience, campaign, and content goals |
| **R** | Role | The content expertise the AI should adopt |
| **I** | Instruction | Exactly what content to produce |
| **S** | Spec | Format, word count, SEO requirements, tone rules |
| **P** | Performance | What "great content" looks like for this piece |

---

## How to Use This Library

1. **Browse `index.md`** to find the content type you need.
2. **Open the relevant prompt file** in `prompts/`.
3. **Copy the full prompt text** and fill in the `[BRACKET]` placeholders.
4. **Paste into Claude** and review the draft.
5. **Edit for voice and accuracy** — AI gives you the structure and first draft; you add brand voice and subject-matter accuracy.

### Content Marketing Tips
- Always fill in the audience and brand context — this is what separates generic AI content from on-brand content.
- For SEO content, include your target keyword in the Context section and specify where it should appear.
- Chain these prompts: use the Blog Post Outline prompt first, then pass the outline into a full-draft prompt.
- Save your best filled-in prompts as reusable templates for your content calendar.

---

## Prompt Index

| # | File | Use Case |
|---|------|----------|
| 01 | `blog-post-outline.md` | Create a SEO-structured blog post outline with H2/H3 hierarchy |
| 02 | `linkedin-thought-leadership.md` | Write a LinkedIn post that builds authority without being salesy |
| 03 | `email-newsletter-draft.md` | Draft a weekly/monthly newsletter with a clear editorial structure |
| 04 | `case-study-interview-questions.md` | Generate targeted case study interview questions for a customer story |
| 05 | `social-media-repurpose-pack.md` | Repurpose one piece of content into 5 social media formats |
| 06 | `seo-meta-description.md` | Write SEO meta descriptions and title tags that drive clicks |
| 07 | `competitor-content-gap-analysis.md` | Identify content gaps vs competitors and prioritise what to create |
| 08 | `content-calendar-brief.md` | Brief a month of content for a specific campaign or theme |
| 09 | `webinar-follow-up-email.md` | Write a post-webinar follow-up that drives the next step |
| 10 | `youtube-description.md` | Write a YouTube video description optimised for search and engagement |

---

## Folder Structure

```
sample-04/
├── README.md          <- You are here
├── index.md           <- One-line descriptions of all prompts
└── prompts/
    ├── blog-post-outline.md
    ├── linkedin-thought-leadership.md
    ├── email-newsletter-draft.md
    ├── case-study-interview-questions.md
    ├── social-media-repurpose-pack.md
    ├── seo-meta-description.md
    ├── competitor-content-gap-analysis.md
    ├── content-calendar-brief.md
    ├── webinar-follow-up-email.md
    └── youtube-description.md
```
