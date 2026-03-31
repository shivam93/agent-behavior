# First-Principles Thinking Partner

**An AI skill that refuses to give you answers — so you build better ones yourself.**

Most AI tools race to provide solutions. This one deliberately withholds them. The core mechanism — what I call the **Resolution Refusal** — protects your capacity to think by forcing you to construct your own reasoning before conclusions land. The friction is the feature.

The skill separates real constraints from inherited assumptions using a three-bucket classification:

- **First Principle** — governed by physics, math, or biology. Irreducible.
- **Institutional Constraint** — governed by law, regulation, or contract. Real friction, but human-constructed.
- **Conventional Assumption** — governed by habit, precedent, or organizational norm. This is where the opportunity lives.

The difference between calling something "institutional" and "conventional" isn't academic — it determines whether you need to negotiate the system or just stop obeying a habit.

---

## What This Skill Does

- Asks questions that surface constraints you've been treating as fixed
- Classifies each constraint so you know what's actually immovable vs. what you've inherited
- Pushes your reasoning to bedrock before letting you rebuild
- Checks your new direction against the system it lives in (so you don't optimize one thing and break three others)

## What This Skill Doesn't Do

- Generate ideas (this is for evaluating and diagnosing, not brainstorming)
- Give you answers quickly (the delay is intentional)
- Replace domain expertise (it sharpens thinking, it doesn't supply knowledge)

---

## Installation

This skill uses the [Agent Skills open standard](https://github.com/anthropics/agent-skills) and works across multiple AI coding tools.

### Claude Code

```bash
# Project-level
cp -r first-principles/ your-project/.claude/skills/

# Or global (applies to all projects)
cp -r first-principles/ ~/.claude/skills/
```

### Cursor

```bash
cp -r first-principles/ your-project/.cursor/skills/
```

### Gemini CLI

```bash
cp -r first-principles/ your-project/.gemini/skills/
```

### Other Tools

Any tool supporting the Agent Skills standard (Codex CLI, Windsurf, Aider, etc.) can load this skill. Place the `first-principles/` directory in the tool's skills folder.

---

## How to Use

Start a conversation with any of these phrases:

- "Help me rethink how we're approaching X"
- "Challenge my assumptions about X"
- "I want to go deep on whether X is actually true"
- "What's actually a constraint here vs. what we've inherited?"
- "Why does X work this way — is there a better reason than 'it's always been this way'?"

The skill works across domains. It ships with domain-specific constraint libraries for **behavior design**, **product ideation**, **strategy/organizational change**, and **engineering architecture** — but the method applies to any problem where the existing frame may be the problem.

### What a Good Session Looks Like

You'll know it worked when:
- You rephrased the original problem mid-session
- A constraint you treated as fixed turned out to be conventional
- You left with a different question than you arrived with

You'll know it didn't when:
- You felt validated in your original framing
- The final synthesis used the same vocabulary as the initial problem

---

## Domains Covered

The `references/fp-protocol.md` file contains domain-specific first principles, common assumptions to challenge, and probing questions for:

1. **Behavior Design** — motivation, friction, effort-to-reward ratios
2. **Product Ideation** — value creation, jobs-to-be-done, minimum viable proof
3. **Strategy & Organizational Change** — incentive structures, culture-as-behavior, change friction
4. **Engineering Architecture** — scaling constraints, abstraction costs, rewrite decisions

You can add your own domain sections to `fp-protocol.md` following the same structure. Over time, you'll build a personal library of high-leverage questions for the domains you work in.

---

## Test Prompts

These prompts verify the skill triggers correctly. They also show what it's designed for — and what it isn't.

### Should Trigger

1. *"I want to rethink our entire onboarding flow — I think our assumptions about what users need are wrong"*
2. *"We keep saying we need to rewrite the backend but I'm not sure that's actually true"*
3. *"Help me challenge my thinking about why we're building this as a platform instead of a tool"*
4. *"What's actually true about user retention? I feel like we're just copying what Duolingo does"*
5. *"I need to go deep on whether our org structure is actually preventing us from shipping faster"*

### Should Not Trigger

1. *"Help me brainstorm 10 ideas for our hackathon project"* — generative mode, not evaluation
2. *"Write a technical spec for the authentication service"* — execution, not diagnosis
3. *"What are the best practices for designing onboarding flows?"* — knowledge retrieval, not assumption challenging

---

## Files

```
first-principles/
├── SKILL.md                      # Behavioral instructions — how Claude operates
├── references/
│   └── fp-protocol.md            # Domain constraint library — ammunition for decomposition
└── README.md                     # This file
```

---

## Built By

**Shivam Bhatnagar** — 12 years designing enterprise AI. Now building the vocabulary for agent behavior design: the discipline that didn't exist when I needed it.

[LinkedIn](https://www.linkedin.com/in/shivam-bhatnagar-design/) · [X](https://x.com/MrShivamB) · [GitHub](https://github.com/shivam93/agent-behavior)

---

## License

MIT — use it, fork it, adapt it, make it yours.
