---
name: status
description: Use to check which design sprint exercises have been completed and get suggested next steps.
---

# Sprint Status

## Process

Scan the working directory for these exercise output files:

- `context-builder.md`
- `design-principles.md`
- `jtbd-capture.md`
- `dot-vote-*.md` (any files matching this pattern)
- `problem-framing.md`
- `hmw-opportunities.md`
- `crazy-eights.md`
- `storyboarder.md`
- `battleship-brainstorm.md`
- `sprint-artifact.md`

Also check for a `context/` folder and note whether it exists and what's in it.

## Output

### Sprint Progress

Show a checklist of all exercises with their completion status:

```
## Sprint Progress

- [x] Context Builder (context-builder.md)
- [ ] Design Principles
- [x] JTBD Capture (jtbd-capture.md)
- [x] Dot Vote — JTBD (dot-vote-jtbd.md)
- [ ] Problem Framing
- [ ] HMW Opportunities
- [x] Crazy Eights (crazy-eights.md)
- [ ] Storyboarder
- [ ] Battleship Brainstorm
- [ ] Sprint Artifact
```

For each completed exercise, check for a `<!-- STATUS: complete -->` or `<!-- STATUS: in-progress -->` comment at the top of the file. If `in-progress`, mark it as `[~]` (partial) in the checklist.

### Context Folder

Report whether `context/` exists and list its contents if it does.

### Suggested Next Steps

Based on what's been completed, recommend 1-3 exercises to run next. Use these suggested sequences as a guide:

**Full Sprint:**
context-builder → design-principles → jtbd-capture → dot-vote → problem-framing → hmw-opportunities → crazy-eights → dot-vote → storyboarder → sprint-compiler

**Quick Ideation:**
battleship-brainstorm → dot-vote → storyboarder

**Problem Discovery:**
context-builder → jtbd-capture → problem-framing → hmw-opportunities

Identify which sequence the user appears to be following (or if they're doing a custom flow), and suggest the next logical step. If enough exercises are done, suggest running `/design-sprinter:sprint-compiler` to assemble the final document.
