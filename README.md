# agent-behavior

No organizing model yet exists for how AI agents should behave.

Not the interface. Not the prompts. The behavior itself: when an agent answers, when it withholds, how it communicates failure, what it does when the user's frame is the problem.

UI design has a vocabulary. Agent behavior design is genuinely unclaimed territory.

This repo is where that vocabulary starts.

---

**How this works:** Each entry names and specifies a behavior pattern — the design thinking, the cognitive science, the edge cases. Each entry has a companion skill you can install and use directly.

---

## Entries

Behavioral design specs. One per week, 12 weeks.

| # | Pattern | Companion Skill |
|---|---|---|
| [01](entries/01-the-resolution-refusal/) | The Resolution Refusal | [first-principles](skills/first-principles/) |
| 02 | Coming soon | — |

### [01 — The Resolution Refusal](entries/01-the-resolution-refusal/)

The most valuable behavior a thinking-partner agent can have: deliberately withholding resolution.

The Oracle Default — every AI system resolves uncertainty as fast as possible — is trained in via RLHF. For thinking-intensive work, it's the wrong behavior. This entry specifies the counter-pattern: when to withhold, how to design the withholding, and what breaks when you get it wrong.

→ [Read the full entry](entries/01-the-resolution-refusal/) · [Install the skill](skills/first-principles/)

---

## Skills

Installable AI skills — one per entry, each implementing the named behavior pattern.

### [First-Principles Thinking Partner](skills/first-principles/)

The companion skill for Entry 01. Implements the Resolution Refusal: refuses to answer until you've done the cognitive work that makes the answer meaningful.

```bash
# Clone the repo
git clone https://github.com/shivam93/agent-behavior

# Claude Code (global — works across all projects)
cp -r skills/first-principles ~/.claude/skills/

# Claude Code (project-level)
cp -r skills/first-principles your-project/.claude/skills/

# Cursor
cp -r skills/first-principles your-project/.cursor/skills/

# Gemini CLI
cp -r skills/first-principles your-project/.gemini/skills/
```

→ [Full install instructions and test prompts](skills/first-principles/README.md)

---

## Framework (in progress)

Each entry follows the same structure: **Behavior Name → Context → Design Specification → Edge Cases → Usable Artifact.**

The patterns across 12 entries are converging toward an organizing model for agent behavior design — a vocabulary for the decisions that currently have no names. That model will be documented here as it emerges from the work.

The entries are the evidence. The framework is the conclusion.

---

## About

**Shivam Bhatnagar** — 12 years designing enterprise AI. Designed AI Studio at Automation Anywhere, which drove 65% of new enterprise sales. Now building the vocabulary for agent behavior design: the discipline that didn't exist when I needed it.

[LinkedIn](https://www.linkedin.com/in/shivam-bhatnagar-design/) · [X](https://x.com/MrShivamB) · [GitHub](https://github.com/shivam93)

---

## Work With Me

If your team is building an AI product and the behavior isn't specified — when it answers, when it withholds, how it handles failure — [reach out on LinkedIn](https://www.linkedin.com/in/shivam-bhatnagar-design/).

---

MIT License
