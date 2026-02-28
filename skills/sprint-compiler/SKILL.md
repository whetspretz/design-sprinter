---
name: sprint-compiler
description: Use when assembling individual exercise outputs into a single structured Notion-ready sprint document.
---

# Sprint Compiler

# Session Setup

Before starting:

1. **Context check**: Look for a `context/` folder in the working directory. If it exists, read all files inside for additional materials. If it doesn't exist, ask if the user has reference materials. If yes, create the `context/` folder and tell them to drop files in. If no, create an empty `context/` folder and proceed.

2. **Resume check**: Check if `sprint-artifact.md` already exists. If it does, ask: "I found an existing sprint artifact. Would you like to rebuild it from scratch, or update it with any new exercise outputs?"

3. **AI participation**: Ask: "Should I add editorial commentary, or assemble as-is?"
   - **Editorial mode**: AI adds brief commentary between sections — highlighting themes that connect across exercises, calling out gaps, and noting tensions worth revisiting.
   - **Assemble mode**: AI compiles content as-is with minimal formatting cleanup and no added commentary.

4. **Output**: The compiled document will be saved as `sprint-artifact.md` in the working directory. If the file already exists, ask before overwriting. Add `<!-- STATUS: complete -->` at the top of the file when finished. If saving a partial result mid-exercise, use `<!-- STATUS: in-progress -->` instead.

## Facilitation Quality Bar
- Preserve the substance of each exercise — don't water down or editorialize the content
- Clean up formatting inconsistencies across exercises
- In Editorial mode, keep commentary brief and clearly separated from exercise content
- Flag exercises that weren't completed as potential gaps

---

# Exercise

## Goal
Assemble individual exercise outputs into a single structured sprint document.

## Process

Scan the working directory for these exercise output files:

- `context-builder.md`
- `design-principles.md`
- `jtbd-capture.md`
- `dot-vote-*.md` (all files matching this pattern — there may be multiple voting rounds)
- `problem-framing.md`
- `hmw-opportunities.md`
- `crazy-eights.md`
- `storyboarder.md`
- `battleship-brainstorm.md`

Report which files were found and which are missing.

## Output Format

Assemble all found outputs into this structure:

```
# Design Sprint — Final Artifact

## 1. Context
(from context-builder.md: persona snapshot, five insights, north star, differentiation)

## 2. Design Principles
(from design-principles.md)

## 3. Jobs to Be Done
(from jtbd-capture.md: raw JTBD, clusters)
(include dot-vote-jtbd.md results here if found)

## 4. Problem Framing
(from problem-framing.md)

## 5. HMW Opportunities
(from hmw-opportunities.md)
(include dot-vote-hmw.md results here if found)

## 6. Solution Concepts
(from crazy-eights.md and/or battleship-brainstorm.md)
(include dot-vote-concepts.md results here if found)

## 7. Storyboard
(from storyboarder.md)

## 8. Recommended Next Steps
(AI-generated practical 1-2 week execution plan based on the sprint outputs)
```

**Rules:**
- Only include sections for which output files exist
- Preserve the content from each file — clean up formatting but don't alter substance
- Place dot-vote results inline with the section they relate to (match by filename label)
- If a dot-vote file doesn't clearly map to a section, include it in a "Voting Results" appendix
- Add a "Recommended Next Steps" section with a practical 1-2 week execution plan based on the sprint outputs
- Note which exercises were not completed, in case the user wants to revisit them
- Add `<!-- STATUS: complete -->` at the top of the output file (or `<!-- STATUS: in-progress -->` if the compilation is partial)

---

## What's Next

Suggest these follow-up actions:
- Share the sprint artifact with your team for feedback
- Run `/design-sprinter:status` to see if any exercises were skipped
- Start a new sprint cycle by revisiting `/design-sprinter:context-builder` with refined context
