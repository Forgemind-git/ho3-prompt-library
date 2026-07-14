# HO3 — Prompt Library

> Hands-on portfolio project · **Week 2** · **Peer-reviewed** · module M6. Part of the **ForgeMind AI — AI Productivity Essentials** course.

## Goal

**Done when:** you have 8–12 **CRISP** prompts for the work you actually repeat — and for each one, the
lazy prompt it replaces, both outputs side by side, and the proof that the structure is what made the
difference.

## The idea in one minute

A prompt library is not a folder of prompts. It is a folder of prompts **you can prove are better**.

Next to each one sits the lazy version you used to type, and the mediocre thing it gave you back.
**Keep the bad output.** Without it you have a pile of text. With it, you have evidence — and you can
show anyone, in ten seconds, exactly what the structure bought you.

Every prompt is written with **CRISP**, and each letter is doing a job:

| | |
|---|---|
| **Context** | The situation. What is going on, and who for. |
| **Role** | Who Claude is being. An expert, not a generalist. |
| **Instruction** | The task, in steps. What to actually do. |
| **Spec** | Format, length, tone, the bans. What the output must look like. |
| **Performance** | The bar. How you'll know it's good enough to send. |

**Performance** is the one people drop, and it's the one that decides whether the output is *sendable*
rather than merely correct.

## Pick a problem statement

Choose the one closest to **your** job — the prompts only pay you back if they are for work you
genuinely repeat. Each maps to a finished sample of **10 prompts** in `samples/`, where every prompt
shows the lazy version beside the CRISP one.

1. **Customer support** — your team answers the same issues in wildly different tones. One reply is
   warm and specific, the next reads like a form letter, and the customer can tell which one they got.
2. **Project management** — every status update, risk entry and retro summary comes out in a different
   shape, so nobody reads them and nothing gets actioned.
3. **People management** — you stare at a blank page before every 1:1, review and difficult
   conversation, and what you finally write is inconsistent enough to be unfair.
4. **Content marketing** — you reinvent the wheel for every post, and the voice drifts from one piece
   to the next because nothing about the voice was ever written down.
5. **Financial analysis** — variance commentary, board narratives and forecast assumptions get
   rewritten from scratch every cycle, and the numbers arrive without the story that makes them mean
   anything.

Or build a library for any other role — as long as it is work you genuinely repeat.

## What to ship

```
ho3-prompt-library/
├─ README.md              ← the index: what each prompt is for, and when to reach for it
├─ prompts/
│  ├─ 01-reply-to-angry-customer.md
│  ├─ 02-escalation-note.md       ← each file: purpose · CRISP breakdown · the prompt
│  └─ …                              · the lazy prompt + its weak output + why
└─ .gitignore                        · the CRISP output + the bar it had to clear
```

A reviewer should be able to open **any single prompt file** and see the whole story without opening
anything else.

## How it works

1. **List 8–12 things you write again and again.** Not clever things — *repetitive* things. If you
   only write it twice a year, it does not belong in the library.
2. **Write the lazy prompt first**, exactly as you'd normally type it. One line, no thought. **Run it,
   and keep the output.** That mediocre answer is the most valuable thing in the file.
3. **Rewrite it with CRISP.** Leave the placeholders in `[SQUARE BRACKETS]` so it is reusable, not a
   one-off.
4. **Run the CRISP version on the same task.** Same model, same day. The only thing that changed is
   what you told it.
5. **Save both outputs together**, with one line on why the first was weak.
6. **Push it.**

## The mistake everyone makes

- **Skipping the lazy prompt** because you already know the CRISP one is better. Then the library is
  just assertions — you have shown nobody anything, least of all yourself.
- **Running the before/after in the same chat.** If you ask for the lazy answer in the chat where you
  just designed the CRISP prompt, Claude already knows what you want — it will quietly write a *good*
  answer to a *bad* prompt, and your before/after proves nothing. **Use a fresh chat.**
- **Writing prompts you'll never use.** Twelve beautiful prompts for work you don't do is twelve
  pieces of homework. Eight for work you do weekly is a tool you'll still be using next year.

## About this repo

`samples/sample-01 … sample-05` are five finished libraries — ten prompts each. Open one: pick a
prompt from the rail, then flip between **"Lazy prompt"** and **"CRISP prompt"** and watch the output
change. Same task, same model; the only thing that differs is what you told it.

No API key. Everything runs on your normal Claude.ai subscription.

---

*HO3 · Peer-reviewed · ForgeMind AI Course · module M6 (Week 2)*
