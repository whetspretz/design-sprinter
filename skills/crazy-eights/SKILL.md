---
name: crazy-eights
description: Use when generating rapid divergent solution concepts for a design challenge or opportunity area.
---

# Crazy Eights

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `crazy-eights.md` already exists in the working directory. If it does, ask: "I found existing concepts. Would you like to resume and refine them, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `crazy-eights.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Goal
Rapid concept divergence — generate 8 meaningfully different solution concepts.

## Input

Check the working directory and `context/` folder for prior exercise outputs (especially `hmw-opportunities.md`, `dot-vote-*.md`). If found, use the top-voted opportunity or HMW question as the design challenge.

If no prior outputs exist, ask the user to describe the design challenge or opportunity they want to ideate on.

## Rules

- Each concept must be **meaningfully different** from the others
- Mix safe and bold ideas
- Avoid minor variations of the same concept
- Each concept should use a **different product shape or mechanism** — don't repeat the same underlying approach with surface-level changes

### Diversity prompts

Push concepts across these different shapes:
- Automation (do it for the user)
- Marketplace (connect supply and demand)
- Community (leverage collective behavior)
- Tool (give the user power to do it themselves)
- Content (educate or inform)
- Gamification (motivate through progress and rewards)
- Integration (plug into existing workflows)
- Platform (enable others to build on top)

## Process

In Brainstorm mode, AI generates all 8 concepts for the user to react to, refine, and swap.

In Facilitate mode, AI prompts the user for each concept with provocative questions like:
- "What's the boldest version of this?"
- "What if you removed the main constraint?"
- "What would a competitor never try?"

## Output

### Crazy 8 Concepts

For each concept:

- **Concept name**
- **One-line idea**
- **Key differentiator**
- **Risk level** (Low / Medium / High)

Clearly label AI contributions.

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:dot-vote` — pick your top concepts
- `/design-sprinter:storyboarder` — bring the winning concept to life as a user journey
