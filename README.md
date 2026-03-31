# agent-behavior

No organizing model yet exists for how AI agents should behave.

Not the interface. Not the prompts. The behavior itself: when an agent answers, when it withholds, how it communicates failure, what it does when the user's frame is the problem.

UI design has a vocabulary. Agent behavior design is genuinely unclaimed territory.

This repo is where that vocabulary starts. One named behavior pattern per week. 12 weeks. Each entry: the design spec, the cognitive science behind it, and a forkable skill.

---

## Skills

Installable AI skills implementing named behavior patterns. Each one is a behavioral specification — grounded in research, tested across domains, ready to drop into your setup.

### [First-Principles Thinking Partner](first-principles/)

An AI skill that refuses to give you answers — so you build better ones yourself.

The Oracle Default: every AI system, by training, resolves uncertainty as fast as possible. For thinking-intensive work — strategy, diagnosis, assumption auditing — that's the problem. This skill implements the counter-behavior.

```bash
# Claude Code (global — works in all your projects)
cp -r first-principles/ ~/.claude/skills/

# Claude Code (project-level)
cp -r first-principles/ your-project/.claude/skills/

# Cursor
cp -r first-principles/ your-project/.cursor/skills/

# Gemini CLI
cp -r first-principles/ your-project/.gemini/skills/
```

→ [Full install instructions, usage, and test prompts](first-principles/README.md)

---

## Entries

Behavioral design specs. The pattern, the mechanism, the edge cases, and what breaks when you get it wrong.

**[01 — The Resolution Refusal](entries/01-the-resolution-refusal/)** — The most valuable behavior a thinking-partner agent can have: deliberately withholding resolution. Why the Oracle Default is trained in, what the cognitive science says, and how to design against it.

*Entry 02 publishing April 13.*

---

## Work With Me

If your team is building an AI product and the behavior isn't specified — when it answers, when it withholds, how it handles failure — [reach out on LinkedIn](https://www.linkedin.com/in/shivambhatnagar/).

---

**Shivam Bhatnagar** — 12 years designing enterprise AI. Now building the vocabulary for agent behavior design: the discipline that didn't exist when I needed it.

[LinkedIn](https://www.linkedin.com/in/shivambhatnagar/) · [GitHub](https://github.com/shivam93)

---

MIT License
