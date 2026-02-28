---
name: jtbd-capture
description: Use when generating and clustering Jobs-to-Be-Done statements to map user needs and identify opportunity themes.
---

# JTBD Capture

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `jtbd-capture.md` already exists in the working directory. If it does, ask: "I found existing JTBD work. Would you like to resume and refine it, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `jtbd-capture.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Generate job statements and cluster them into themes.

## Input

Check the working directory and `context/` folder for prior exercise outputs. Useful inputs include:
- `context-builder.md` — persona and product context (use persona pains and motivations to seed JTBD statements)
- `design-principles.md` — strategic guardrails (ensure JTBDs align with product direction)

If no prior outputs exist, proceed — JTBDs can be generated from scratch through conversation.

## Part 1 — JTBD Generation

Ask the user to write JTBD statements in this format:

> As a user when ___, I want to ___, so I can ___.

Encourage 5–15 statements.

In Brainstorm mode, propose additional JTBDs from each active role's perspective (default: PM, Design, Engineering, Business — or custom roles if configured).

Label AI-generated ones clearly.

## Part 2 — Clustering

After JTBD collection:

- Group into 4–8 natural themes
- Name each cluster clearly
- Provide 1-line summary per cluster

### Output: JTBD Clusters

For each cluster:

- Cluster name
- Theme summary
- Included JTBD statements

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:dot-vote` — prioritize your JTBD clusters
- `/design-sprinter:problem-framing` — turn the top clusters into sharp problem statements
