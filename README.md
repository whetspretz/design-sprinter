```
     _           _                            _       _
  __| | ___  ___(_) __ _ _ __    ___ _ __  _ __(_)_ __ | |_ ___ _ __
 / _` |/ _ \/ __| |/ _` | '_ \  / __| '_ \| '__| | '_ \| __/ _ \ '__|
| (_| |  __/\__ \ | (_| | | | | \__ \ |_) | |  | | | | | ||  __/ |
 \__,_|\___||___/_|\__, |_| |_| |___/ .__/|_|  |_|_| |_|\__\___|_|
 ─ ── ───────────  |___/ ────────── |_| ─────────────────── ─── ── ─ ─
```

A modular design sprint toolkit for [Claude Code](https://docs.anthropic.com/en/docs/claude-code). Run exercises in any order to brainstorm, prioritize, and storyboard product ideas.

## Install

```bash
claude plugin add /path/to/design-sprinter
```

Or clone this repo and add it as a local plugin.

## Quick Start

Pick any exercise and run it:

```
/design-sprinter:crazy-eights
```

That's it. Each exercise is standalone — no required sequence.

## Exercises

| Command | What it does |
|---------|-------------|
| `/design-sprinter:context-builder` | Build persona and product context (north star, differentiation) |
| `/design-sprinter:design-principles` | Define strategic guardrails with More/Less framing |
| `/design-sprinter:jtbd-capture` | Generate and cluster Jobs-to-Be-Done statements |
| `/design-sprinter:dot-vote` | Prioritize any list with AI panel voting or solo voting |
| `/design-sprinter:problem-framing` | Turn user needs into sharp problem statements |
| `/design-sprinter:hmw-opportunities` | Generate How Might We questions to expand solutions |
| `/design-sprinter:crazy-eights` | 8 rapid divergent solution concepts |
| `/design-sprinter:storyboarder` | 7-panel user journey storyboard |
| `/design-sprinter:battleship-brainstorm` | 7x7 forced-collision matrix for novel ideas |
| `/design-sprinter:sprint-compiler` | Assemble exercise outputs into one Notion-ready doc |
| `/design-sprinter:status` | Check sprint progress and get suggested next steps |

## How It Works

### Context Folder

Drop reference docs, screenshots, or other materials into a `context/` folder in your working directory. Every exercise checks this folder for background understanding. If the folder doesn't exist, the exercise will offer to create it for you.

```
your-project/
├── context/
│   ├── user-research.pdf        ← your reference materials
│   ├── competitor-screenshot.png
│   └── sprint-roles.md          ← optional custom AI roles
├── context-builder.md            ← exercise output (auto-discovered)
├── crazy-eights.md               ← exercise output (auto-discovered)
└── ...
```

Exercise outputs are saved to the working directory root and are automatically discovered by subsequent exercises — no need to copy them into `context/`.

### AI Participation

Each exercise asks how you want the AI to participate:

- **Brainstorm mode** — AI contributes ideas from multiple role perspectives (clearly labeled)
- **Facilitate mode** — AI asks questions and structures your responses, but doesn't generate ideas

The dot-vote exercise has its own modes:
- **Panel mode** — AI votes as multiple roles alongside you
- **Solo mode** — You vote alone, AI just tallies results

### Custom AI Roles

By default, the AI brainstorms as four roles: **PM, Design, Engineering, Business**. You can customize these for your domain by creating a `context/sprint-roles.md` file:

```markdown
# Sprint Roles

- **Doctor**: Prioritizes patient safety, clinical evidence, and health outcomes
- **Teacher**: Prioritizes learning effectiveness, accessibility, and engagement
- **Regulator**: Prioritizes compliance, risk mitigation, and public trust
```

If no roles file exists, the exercise will ask if you want to customize — and offer to save your choices for future exercises. Maximum 6 roles.

### Resume Support

Every exercise checks for existing output files. If you've already started an exercise, you can pick up where you left off instead of starting over.

### Output

Each exercise saves its output as a markdown file in your working directory (e.g., `crazy-eights.md`, `jtbd-capture.md`). The sprint compiler can assemble them all into a single document.

## Suggested Sequences

Exercises work in any order, but here are some effective flows:

**Full Sprint**
1. `context-builder` → `design-principles` → `jtbd-capture` → `dot-vote` → `problem-framing` → `hmw-opportunities` → `crazy-eights` → `dot-vote` → `storyboarder` → `sprint-compiler`

**Quick Ideation**
1. `battleship-brainstorm` → `dot-vote` → `storyboarder`

**Problem Discovery**
1. `context-builder` → `jtbd-capture` → `problem-framing` → `hmw-opportunities`

## License

MIT
