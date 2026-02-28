---
name: design-principles
description: Use when defining strategic guardrails for a product using More/Less framing to clarify design priorities.
---

# Design Principles

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `design-principles.md` already exists in the working directory. If it does, ask: "I found existing design principles. Would you like to resume and refine them, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `design-principles.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Define strategic guardrails using More / Less framing.

## Input

Check the working directory and `context/` folder for prior exercise outputs. Useful inputs include:
- `context-builder.md` — persona and product context (use north star and differentiation pillars to ground principles)

If no prior outputs exist, proceed — principles can be defined from scratch through conversation.

## Instructions

Ask the user to provide 3–7 pairs in this format:

> More about ___, Less about ___

If they struggle, propose suggestions. In Brainstorm mode, actively generate 5–7 starter pairs for the user to react to.

## What Makes a Good Principle

Good principles create **real tension** — they force a tradeoff between two things that both seem valuable. Apply these rules:

- **Actionable**: A team member should be able to use the principle to make a decision
- **Specific**: It should be about *this* product, not any product ("More delightful" is too generic)
- **Tense**: Both sides should be defensible — if no one would argue for the "Less" side, the principle is a truism
- **Distinct**: Each principle should cover different territory

### Anti-patterns to challenge

If the user proposes any of these, push back and help them sharpen:
- "More quality, less bugs" — too obvious, no tension
- "More user-friendly, less confusing" — same thing said twice
- "More innovation, less legacy" — too abstract to act on
- Principles where the "Less" side is clearly bad — the whole point is sacrificing something real

## AI Processing

After user input:

- Normalize wording
- Remove duplicates
- Ensure principles are actionable and create real tension
- Flag any principles that feel like truisms and suggest sharper alternatives

## Output

### Design Principles Table

| Principle | More of | Less of | Why it matters |

AI fills the "Why it matters" column with a concise rationale for each principle — specifically explaining what tradeoff the team is making and when this principle should guide a decision.

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:jtbd-capture` — map user needs with your principles as guardrails
- `/design-sprinter:problem-framing` — frame problems directly if you already have user insights
- `/design-sprinter:battleship-brainstorm` — jump to divergent ideation if the problem space is clear
