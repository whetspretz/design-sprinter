---
name: storyboarder
description: Use when creating a realistic 7-panel user journey storyboard for a product concept or feature.
---

# Storyboarder

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `storyboarder.md` already exists in the working directory. If it does, ask: "I found an existing storyboard. Would you like to resume and refine it, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `storyboarder.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Create a realistic user journey as a 7-panel storyboard.

## Input

Check the working directory and `context/` folder for prior exercise outputs. Useful inputs include:
- `context-builder.md` — persona and product context
- `design-principles.md` — strategic guardrails (ensure the storyboard reflects product principles)
- `jtbd-capture.md` — user needs
- `problem-framing.md` — problem statements
- `hmw-opportunities.md` — opportunity areas
- `crazy-eights.md` — solution concepts
- `battleship-brainstorm.md` — brainstorm concepts
- `dot-vote-*.md` — voting results indicating which concepts were selected

If no prior outputs exist, ask the user to describe:
- Who is the user?
- What product concept or feature are we storyboarding?
- What problem does it solve?

## Process

Create a **7-panel storyboard**. Each panel must include:

1. **Scene title**
2. **What the user is doing**
3. **What they are thinking/feeling**
4. **What the product does**
5. **Why this moment matters**

The story must feel grounded in everyday reality — not idealized or abstract.

### Arc & Pacing Guide

Follow this narrative structure across the 7 panels:

| Panels | Phase | Purpose |
|--------|-------|---------|
| 1–2 | **Status quo** | Show the user's world before the product — their current workflow, frustrations, workarounds |
| 3 | **Trigger** | The moment something changes — they discover the product, hit a breaking point, or get a recommendation |
| 4–5 | **Interaction** | The user engages with the product — show specific actions, not abstract "uses the app" |
| 6 | **Resolution** | The problem is solved or meaningfully improved — show the concrete outcome |
| 7 | **New normal** | The user's world has changed — they return, recommend, or build a new habit |

In Brainstorm mode, AI drafts the full storyboard for the user to refine.

In Facilitate mode, AI walks the user through panel by panel with guiding questions:
- "Where does the user first encounter this problem?"
- "What's the emotional turning point?"
- "What makes them come back?"

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:sprint-compiler` — assemble all exercise outputs into a single sprint document
