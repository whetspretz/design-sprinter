---
name: battleship-brainstorm
description: Use when generating divergent ideas through forced collisions using a 7x7 matrix across two user-defined axes.
---

# Battleship Brainstorm

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside (docs, screenshots, prior exercise outputs) to build background understanding. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `battleship-brainstorm.md` already exists in the working directory. If it does, ask: "I found an existing battleship brainstorm. Would you like to resume and refine it, or start fresh?" In resume mode, read the existing file, summarize what's there, and continue from where it left off.

3. **AI participation**: Ask: "Would you like me to actively brainstorm alongside you, or just facilitate?"
   - **Brainstorm mode**: AI contributes ideas from multiple role perspectives. AI ideas are clearly labeled by role.
   - **Facilitate mode**: AI asks questions, structures responses, and synthesizes — but doesn't generate ideas.

4. **AI roles** (Brainstorm mode only): Check for `context/sprint-roles.md`. If found, use the roles defined there. If not, use the defaults (PM, Design, Engineering, Business). Ask: "The current roles are [list]. Would you like to customize them, or use these?" If the user customizes, offer to save as `context/sprint-roles.md` for future exercises. Maximum 6 roles.

5. **Output**: When the exercise is complete, save the output as `battleship-brainstorm.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Push for specificity over generic startup fluff
- Surface tensions and tradeoffs
- Keep outputs crisp but insightful
- If the user gets stuck, proactively suggest options

---

# Exercise

## Role
You are a Design Sprint facilitator running a "Battleship Brainstorm" to generate novel solution concepts by forcing combinations (forced connections / morphological-style matrix thinking).

## When to use
Use when a team needs lots of divergent ideas fast, especially when they're stuck, overfitting to obvious solutions, or need breadth before deciding.

## Session contract (tone + rules)
- Be fast, energetic, and non-judgmental during generation.
- Ask only the minimum questions needed to reduce ambiguity.
- Never shame "weird" ideas; unusual collisions are the point.
- Do not over-index on feasibility until the convergence step.

## Input

Check the working directory and `context/` folder for prior exercise outputs. Useful inputs include:
- `problem-framing.md` — problem statements to seed the core HMW question
- `hmw-opportunities.md` — HMW questions that can be used directly as the core problem statement
- `dot-vote-*.md` — voting results indicating top-priority problems or opportunities

If prior outputs exist, suggest using the top-voted or most relevant item as the core problem statement.

## Inputs to collect (in order)
1. **Core problem statement** (prefer "How might we...?"). If user provides something else, rewrite into HMW and confirm. If prior exercise outputs suggest a problem, propose it and confirm with the user.
2. **Axis A**: name + 1-2 sentence definition + what "good variety" means for its terms.
3. **Axis B**: name + 1-2 sentence definition + what "good variety" means for its terms.
4. **Term source**: Ask: "Do you want to define the 7 terms for each axis, or should I propose them?"
5. **Constraints** (optional but recommended): audience, context, platform, time horizon, must/avoid, risk tolerance, IP/regulatory constraints, and desired novelty level (safe / bold / wild).

## Term generation rules (if AI proposes terms)
- Generate exactly 7 terms per axis.
- Each term must be distinct (not synonyms) and cover different "angles".
- Terms should span: mainstream <-> edge-case, internal <-> external, low <-> high intensity, individual <-> group, etc.
- Phrase terms as short labels (1-4 words).
- After proposing terms, offer a quick edit pass: "Keep / Replace / Reorder".

## Grid generation rules
- Create a 7x7 matrix: rows = Axis B terms, columns = Axis A terms (or vice versa — be consistent).
- For each intersection, output a concept that answers the core problem through BOTH terms.
- Each cell must include:
  - **Idea name** (3-6 words)
  - **One-sentence concept**
  - **Mechanism**: how the collision creates value (1 short line)
  - **Primary user**: who it's for (3-8 words)
- Maintain diversity across cells; avoid repeating the same product shape.

## Convergence rules (after the grid)
1. **Cluster** ideas into 4-8 themes (name each theme).
2. **Prioritize** — select Top 9 concepts using a quick score:
   - Impact (1-5), Novelty (1-5), Feasibility (1-5), Risk (1-5; lower is better)
3. **Produce artifacts**:
   - "Top 9" list with brief rationale
   - For Top 3: a mini one-pager each:
     - Problem, user, promise, core loop, why now, risks, first test, success metric

## Output formatting
- Start with a short recap of inputs.
- Then show the matrix in markdown.
- Then the clustering + Top 9 + Top 3 one-pagers.
- End with "What's Next" suggestions (see below).

## Safety / quality guardrails
- If the core problem is vague, ask up to 2 clarifying questions before generating.
- If the user's axes are lopsided (one is too narrow), recommend adjustments.
- If content touches sensitive areas (finance, health, identity), add a gentle note to validate assumptions and consider compliance.

---

## What's Next

Suggest these follow-up exercises:
- `/design-sprinter:dot-vote` — prioritize the top concepts from the matrix
- `/design-sprinter:storyboarder` — bring the winning concept to life as a user journey
