---
name: dot-vote
description: Use when you need to prioritize a list of items using a 5-vote allocation exercise with optional AI panel voting.
---

# Dot Vote

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if any `dot-vote-*.md` files already exist in the working directory. If found, list them and ask: "I found previous voting results. Would you like to start a new vote, or revisit an existing one?"

3. **AI participation**: Ask: "Would you like the AI panel to vote alongside you, or do you want to vote solo?"
   - **Panel mode**: AI votes as multiple roles — each role gets 5 votes with a brief rationale. User also gets 5 votes. Results are combined and compared.
   - **Solo mode**: User votes alone. AI tallies results and highlights patterns but doesn't vote.

4. **AI roles** (Panel mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, name the output file based on what was voted on — e.g., `dot-vote-jtbd.md`, `dot-vote-concepts.md`, `dot-vote-hmw.md`. Ask the user for a short label if the source isn't obvious. If a file with that name already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Prioritize a list of items using a vote allocation.

This is a reusable utility — it works with any list: JTBD clusters, HMW questions, solution concepts, features, or anything else.

## Input

Check the working directory and `context/` folder for prior exercise outputs that contain lists. Useful sources include:
- `jtbd-capture.md` — JTBD clusters
- `hmw-opportunities.md` — HMW questions
- `crazy-eights.md` — solution concepts
- `battleship-brainstorm.md` — brainstorm concepts

If items are found, present them numbered. If not, ask the user to provide the list.

## Rules

- User gets **5 votes** total
- They may distribute votes however they want (all 5 on one item, or spread across several)
- User responds with their vote allocations

### Panel Mode Rules (if selected)

After the user votes, each AI role votes independently with 5 votes each.

**Default roles** (used when no `context/sprint-roles.md` exists):
- **PM** (5 votes): Prioritizes user impact and business value
- **Design** (5 votes): Prioritizes user experience and desirability
- **Engineering** (5 votes): Prioritizes feasibility and technical leverage
- **Business** (5 votes): Prioritizes market fit and revenue potential

If custom roles are defined (e.g., Doctor, Teacher, Regulator), each custom role gets 5 votes and evaluates from its own stated perspective.

Each role provides a 1-sentence rationale for their top pick.

## AI Processing

- Tally votes (user + AI panel if in Panel mode)
- Rank items by total vote count
- Highlight top selections
- Call out any close ties
- In Panel mode, flag items where roles disagree significantly — these reveal tension worth discussing

## Output

### Dot Vote Results

**Panel mode table:**

| Item | User | Role 1 | Role 2 | Role 3 | Role 4 | Total | Rank |
|------|------|--------|--------|--------|--------|-------|------|

(Column headers adapt to the active roles — default or custom.)

**Solo mode table:**

| Item | Votes | Rank |
|------|-------|------|

Then clearly mark: **Top priorities moving forward**

In Panel mode, add a brief "Alignment & Tensions" section noting where roles agreed and where they diverged.

---

## What's Next

Suggest the next exercise based on what was voted on:
- If voting on JTBD clusters → `/design-sprinter:problem-framing`
- If voting on HMW questions → `/design-sprinter:crazy-eights`
- If voting on solution concepts → `/design-sprinter:storyboarder`
- Otherwise → suggest the most logical next step based on context
