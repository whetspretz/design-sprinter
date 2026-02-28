---
name: context-builder
description: Use when starting a design sprint or product exploration to build persona and product context from scratch.
---

# Context Builder

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `context-builder.md` already exists in the working directory. If it does, ask: "I found an existing context builder output. Would you like to resume and refine it, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `context-builder.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Build deep shared context about the target user and the product.

## Input

Check the working directory and `context/` folder for any existing materials. Useful inputs include:
- Reference docs, user research, competitor analysis
- Screenshots or mockups
- Any prior exercise outputs that provide background

If nothing is found, proceed — this exercise builds context from scratch through conversation.

## Part 1 — Persona Discovery

Ask structured questions to understand the target user:

- Who is the primary user?
- What situation are they in when this problem appears?
- What are their biggest frustrations today?
- What motivates them most?
- What alternatives are they currently using?

If answers are thin, ask up to 2 follow-ups.

### Output: Persona Snapshot
- Name (invent if needed)
- Role/context
- Environment
- Key pains
- Key motivations

### Output: Five Key Insights
Generate exactly five sharp behavioral insights about this persona.

Label which are:
- User-provided
- AI-inferred

---

## Part 2 — Product Context

Ask:

- What is the product or business north star?
- What makes this product meaningfully different?
- Any constraints or must-haves?

If missing, help propose options (in Brainstorm mode, actively suggest north star candidates and differentiators).

### Output: North Star
(one clear sentence)

### Output: Differentiation Pillars
(3–5 bullets)

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:design-principles` — define strategic guardrails based on the context you just built
- `/design-sprinter:jtbd-capture` — map user needs using the persona insights
