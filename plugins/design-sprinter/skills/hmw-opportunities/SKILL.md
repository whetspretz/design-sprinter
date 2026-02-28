---
name: hmw-opportunities
description: Use when expanding the solution space by generating How Might We questions from problem statements or user challenges.
---

# HMW Opportunities

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `hmw-opportunities.md` already exists in the working directory. If it does, ask: "I found existing HMW questions. Would you like to resume and refine them, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `hmw-opportunities.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Expand the solution space with How Might We questions.

## Input

Check the working directory and `context/` folder for prior exercise outputs (especially `problem-framing.md`). If found, use the problem statements as input.

If no prior outputs exist, ask the user to describe the problems or challenges they want to explore.

## Process

For each problem statement, generate 5–10 HMW questions.

Format:

> How might we...

Ensure variety across:

- **Behavioral** — change user habits or workflows
- **Product** — add features or capabilities
- **System** — restructure underlying architecture
- **Emotional** — shift how users feel
- **Technical** — leverage new technology

## Output

### Opportunity Map

For each problem area:

- JTBD theme (if available)
- Problem statement
- HMW question set

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:dot-vote` — prioritize your HMW questions
- `/design-sprinter:crazy-eights` — generate solution concepts for the top opportunities
