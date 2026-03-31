# First-Principles Protocol — Domain Constraint Library

This reference provides domain-specific ammunition for first-principles decomposition. Each domain lists irreducible first principles, common assumptions worth challenging, and high-leverage probing questions. Read the relevant domain section when the user's problem falls within it.

These are starting points, not exhaustive lists. The best questions come from the specific context the user brings.

---

## Behavior Design

**First principles:**
- Human motivation is governed by biology — reward circuits, threat responses, social belonging
- Behavior follows perceived effort-to-reward ratio, not stated preferences
- Context shapes behavior more than intention
- Friction is the primary mechanism, not willpower

**Assumptions to challenge:**
- "Users need to be educated to change behavior" → usually false; context redesign works better than information campaigns
- "People make rational decisions" → System 1 drives ~95% of daily behavior; conscious deliberation is the exception
- "If they know the benefit, they'll act" → knowing ≠ doing; the intention-action gap is real and large
- "We need to motivate users" → what if the motivation exists but the friction is too high?
- "Engagement equals value" → high engagement can signal addiction or confusion, not satisfaction

**Probing questions:**
- "What is the user doing *instead* of the behavior you want? That's your real competitor."
- "If you removed every barrier, would this behavior happen naturally — or does it require ongoing effort?"
- "Is the reward visible *before* the effort, or only after?"

---

## Product Ideation

**First principles:**
- Value is created when someone achieves an outcome they couldn't before, or at significantly lower cost/effort
- Markets are conversations about what's true and valuable — not what's clever
- Distribution is a constraint as real as engineering
- The unit of progress is the customer's struggling moment, not the feature

**Assumptions to challenge:**
- "This feature is needed" → what outcome does it serve? Could something simpler serve it?
- "The user wants X" → what job are they actually hiring the product to do?
- "We need to build all of this" → what's the minimum that proves the core assumption?
- "Our competitors do X, so we need X" → are they successful *because* of X, or *despite* it?
- "Users asked for this" → what problem were they trying to describe? The request is often a solution, not a problem statement.

**Probing questions:**
- "If this product disappeared tomorrow, what would users do instead? How painful would the switch be?"
- "What's the smallest version that proves the riskiest assumption?"
- "Are you building because you validated demand, or because the idea is interesting?"

---

## Strategy and Organizational Change

**First principles:**
- Organizations change when the pain of not changing exceeds the friction of changing
- Culture is behavior patterns reinforced by incentives, not stated values
- Decision quality is governed by information quality, not intelligence
- Power structures determine which information flows where — and what gets ignored

**Assumptions to challenge:**
- "We need buy-in from X before we can start" → is that institutional (X has veto power by policy) or conventional (we've always asked X first)?
- "This needs to be phased" → what's the actual constraint that requires phasing? Sometimes phasing is a risk-reduction mechanism; sometimes it's a delay mechanism.
- "People resist change" → which people, and what specifically are they resisting? Often they're resisting the loss of competence, not the change itself.
- "We need alignment first" → alignment on what? Direction? Priorities? Vocabulary? These are different problems with different fixes.
- "Our culture won't support this" → culture is a result, not a cause. What incentive structure produces the current behavior?

**Probing questions:**
- "What would have to be true for this change to be obviously correct? Who would need to believe that, and what evidence would convince them?"
- "What's the smallest change that would generate visible evidence that the direction is right?"
- "If you could change one incentive in the system, which one would shift the most behavior?"

---

## Engineering Architecture

**First principles:**
- Latency is governed by physics (speed of light), not software design — but most latency is software overhead, not physical distance
- Consistency, availability, and partition tolerance cannot all be maximized simultaneously (CAP theorem)
- Complexity compounds — every abstraction layer has a maintenance cost that accrues interest
- The cost of a wrong abstraction is higher than the cost of duplication

**Assumptions to challenge:**
- "We need a microservices architecture" → what problem does the current architecture actually create? Microservices solve organizational scaling problems; if you don't have those, you're importing complexity.
- "We need to rewrite this" → what would it take to fix the current system incrementally? Rewrites are often a conventional response to accumulated friction, not a first-principles conclusion.
- "This won't scale" → at what specific load does it break, and what's the realistic timeline to reach that load? "Won't scale" is frequently an assumption about a future that's further away than it feels.
- "We need real-time" → how real is real-time? 100ms? 1 second? 10 seconds? The answer often changes the architecture dramatically.
- "We should use [trending technology]" → what specific problem does it solve that the current stack doesn't? New tools solve new problems; they also introduce new failure modes.

**Probing questions:**
- "What breaks first at 10x current load? That's your actual scaling constraint — everything else is premature."
- "If you had to ship this in two weeks with the current stack, what would you build differently?"
- "What's the cost of being wrong about this architecture choice? Is it reversible?"
