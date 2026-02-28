---
name: problem-framing
description: Use when turning user needs or JTBD clusters into sharp, human-centered problem statements.
---

# Problem Framing

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `problem-framing.md` already exists in the working directory. If it does, ask: "I found existing problem statements. Would you like to resume and refine them, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `problem-framing.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Turn user needs into sharp, human-centered problem statements.

## Input

Check the working directory and `context/` folder for prior exercise outputs. Useful inputs include:
- `jtbd-capture.md` — JTBD clusters to frame as problems
- `dot-vote-*.md` — voting results indicating top-priority clusters
- `design-principles.md` — strategic guardrails to ensure problem framing aligns with product direction
- `context-builder.md` — persona context for grounding statements in real user situations

If found, use the top-priority JTBD clusters as input.

If no prior outputs exist, ask the user to describe the problem areas they want to frame.

## Process

For each problem area, generate a structured Problem Statement:

- **User**: Who experiences this problem
- **Situation**: When and where it occurs
- **Core struggle**: What they're trying to do but can't
- **Why current solutions fail**: What's broken about the status quo
- **Impact if unsolved**: What happens if nothing changes

Be concrete and human-centered. Avoid abstract or generic framing.

In Brainstorm mode, AI drafts initial problem statements for the user to refine and sharpen.

In Facilitate mode, AI walks the user through each field with guiding questions.

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:hmw-opportunities` — expand the solution space with How Might We questions
