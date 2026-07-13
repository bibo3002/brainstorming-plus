# Brainstorming Plus — Reference

Supporting material for the brainstorming-plus skill. Loaded on demand when the main process calls for it.

## Brainstorming Modes

Identify which mode fits the conversation and adapt. Shift between modes as it evolves.

### Problem Exploration

Use when the user has a problem area but has not yet defined what to solve.

- Ask "who has this problem?" and "what are they doing about it today?" first
- Map the problem ecosystem: who is involved, triggers, consequences of inaction
- Distinguish symptoms from root causes — keep asking "why" until you hit something structural
- Surface adjacent problems not yet considered
- Ask how the problem varies across user segments — it rarely affects everyone the same way

**Key questions:**
- "What happens if we do nothing? Who suffers and how?"
- "Who has solved a version of this in a different context?"
- "Is this a problem of awareness, ability, or motivation?"
- "What would need to be true for this problem to not exist?"

### Solution Ideation

Use when the problem is well-defined and divergent thinking is needed.

- Generate **5-7 distinct approaches** before evaluating any
- Vary along: scope (small tweak vs big bet), approach (product vs process vs policy), timing (quick win vs long-term)
- Include at least one "what if we did the opposite?" option
- Include at least one option that removes something rather than adding
- Resist converging too early — if the user latches onto the first decent idea, push them past the obvious first 3-5

**Ideation techniques:**
- **Constraint removal**: "What if no technical/budget/political constraints?" Then work backward.
- **Analogies**: "How does [another industry] solve this? What can we steal?"
- **Inversion**: "How would we make this problem worse? Now reverse each."
- **Decomposition**: Break into subproblems, solve independently, combine.
- **User hat-switching**: "How would a power user solve this? A new user? An admin? Someone who hates our product?"

### Assumption Testing

Use when the user has a direction and needs to stress-test it.

- List every assumption — stated and unstated
- For each: "How confident are we? What evidence? What would disprove this?"
- Identify the riskiest assumption — the one that kills the idea if wrong
- Suggest the cheapest way to test it before building
- Play devil's advocate: argue the strongest possible case against the idea

**Categories to probe:**
- **User assumptions**: "Users want this" — how do we know, from what evidence, how many users?
- **Problem assumptions**: "This is a real problem" — how often, how much do users care?
- **Solution assumptions**: "This solution will work" — why this approach, what alternatives were dismissed?
- **Business assumptions**: "This will move the metric" — which metric, by how much, over what timeline?
- **Feasibility assumptions**: "We can build this" — in what timeframe, with what trade-offs?
- **Adoption assumptions**: "Users will find and use this" — how, what behavior change does it require?

### Strategy Exploration

Use when thinking about direction, positioning, or big bets — not a specific feature.

- Map possible strategic moves, not just the obvious one
- Think in bets: what are we betting on, odds, payoff
- Second-order effects: "If we do X, what does that enable or foreclose?"
- Competitive dynamics: "If we do this, how do competitors respond?"
- Timeframes: right move for 3 months vs 12 months vs 3 years

## Frameworks (Use as Thinking Tools, Not Templates)

Pull in a framework when it moves the conversation forward. Do not force every conversation through every framework.

### How Might We (HMW)

"How might we [desired outcome] for [user] without [constraint]?"

- Too broad: "How might we improve onboarding?" — could mean anything
- Too narrow: "How might we add a tooltip to step 3?" — that is a solution, not a question
- Right level: "How might we help new users reach their first success within 10 minutes?"

Generate 5-10 HMW questions from a single problem statement. Each reframing opens a different solution space.

### Jobs-to-be-Done (JTBD)

"When [situation], I want to [motivation] so I can [expected outcome]."

- The job is stable even when solutions change — people have been "hiring" solutions to share updates with colleagues for decades: memos, email, Slack, shared docs.
- Functional jobs (get something done) are easier to identify. Emotional jobs (feel confident, look competent) and social jobs (be seen as a leader) are often more powerful.
- Ask "What did they fire to hire your product?" to reveal the real competitive set.

### Opportunity Solution Trees

```text
Desired Outcome
├── Opportunity A (user need / pain point)
│   ├── Solution A1 → Experiment
│   └── Solution A2 → Experiment
├── Opportunity B
│   ├── Solution B1
│   └── Solution B2
└── Opportunity C
    └── Solution C1
```

- Opportunities come from research, not imagination — every opportunity should trace back to evidence
- Multiple solutions per opportunity; if you only have one, you have not explored enough
- Multiple experiments per solution — find the cheapest way to test before building
- The tree is a living artifact; update it as you learn

### First Principles Decomposition

1. State the assumption to examine
2. Break down to fundamental components
3. Question each: law of physics or convention?
4. Rebuild from ground up

**When to use**: when the team is stuck in incremental thinking, when everyone says "that is just how it works," when the category has not been reimagined in years.

### SCAMPER

Seven lenses on an existing product or process:

- **Substitute**: What component could be replaced? What if a different user did this step?
- **Combine**: What if we merged two features? Two workflows? Two user roles?
- **Adapt**: What idea from another product or industry could we borrow?
- **Modify**: What if we made this 10x bigger? 10x smaller? 10x faster?
- **Put to other use**: Could this feature serve a different user or use case?
- **Eliminate**: What if we removed this entirely? Would anyone notice?
- **Reverse**: What if we did the opposite? Flipped the sequence? Inverted the default?

### Reverse Brainstorming

1. Invert: "How could we make this as bad as possible?"
2. Generate ideas that worsen the problem
3. Reverse each — each "make it worse" idea contains the seed of a solution
4. Evaluate the most promising reversals

**Why it works**: people are better at identifying what is wrong than imagining what is right. Inversion unlocks creative thinking when the team is stuck.

### OODA Loop (Observe-Orient-Decide-Act)

A decision-tempo framework for fast-moving, competitive environments. The power is in cycling through the steps faster than the competition, not in the steps themselves.

1. **Observe**: Gather raw signals — usage data, feedback, competitive moves, market shifts. Do not filter yet.
2. **Orient**: Make sense of what you observed through mental models, prior experience, cultural context. Challenge your own orientation — are you seeing what is actually there, or what you expect to see?
3. **Decide**: Choose a direction — a hypothesis to test, not a final commitment. Small bets when uncertain, bigger moves when the signal is clear.
4. **Act**: Ship something. Run the experiment. Then immediately return to Observe with new data.

**When to use in brainstorming**: when the team is over-deliberating and needs to move; when competitive dynamics matter (a competitor shipped, a window is closing, a customer is about to churn); when the brainstorm keeps circling without converging — OODA forces a decision and reframes it as reversible.

**The advantage**: most teams get stuck in Orient — endlessly analyzing, waiting for more data. OODA says: orient with what you have, decide, act, let the next cycle correct your course. The team that cycles fastest learns fastest.

## Being a Good Thinking Partner

A brainstorm is a conversation, not a deliverable. Show up as the kind of experienced PM or design lead who challenges assumptions, asks the hard questions, and pushes ideas further before anyone converges too early.

**Show up this way:**

- **Be opinionated.** "I think approach B is stronger because..." is more useful than listing pros and cons.
- **Challenge constructively.** "That assumes X — are we confident?" rather than "That will not work."
- **Bring unexpected angles.** Cross-industry analogies, counterexamples, edge cases the user has not considered.
- **Match energy.** If the user is excited about an idea, explore it with them before poking holes.
- **Ask the next question.** When the user finishes a thought, do not just agree. Push further: "And then what happens?"
- **Name the pattern.** When you spot a common trap (solutioning too early, scope creep, feature parity thinking, anchoring on the first idea), name it directly.

**Use frameworks as thinking tools when they help** — not as a checklist to work through. A thinking partner who only validates is not a thinking partner; push back.

**The brainstorm generates options. The decision comes later with more data.** If the user leads with a single solution, acknowledge it, then ask "What else could solve this?" Push for three or more alternatives before evaluating any.

**In divergent mode, defer feasibility judgment** — it kills creative thinking. Explore freely first; figure out what is feasible when you converge.

## Anti-Patterns

- **"Too simple to need a design"** — every project gets a design. Simple ones get a short design (a few sentences), but you MUST present it and get approval. "Simple" is where unexamined assumptions cause the most wasted work.
- **Solutioning before framing** — the user jumps to "build X" before defining the problem. Slow them down. Ask what user problem X serves and how we know.
- **Feature parity trap** — "competitor has X, so we need X." Ask what user need X serves and whether there is a better way to serve it.
- **Anchoring on constraints** — "we cannot do that because of technical limitation Y." In divergent mode, set constraints aside. Explore freely first, then figure out feasibility.
- **The one-idea brainstorm** — the user arrives with a solution and calls it brainstorming. Acknowledge the idea, then push for 3+ alternatives. "That is one approach. What are three others?"
- **Analysis paralysis** — too much exploration, no convergence. Prompt: "If you had to pick one direction right now, which would it be and why?"
- **Brainstorming when you should be researching** — some questions cannot be brainstormed; they need data. If the session keeps circling because no one knows the answer, stop and identify what research is needed.
