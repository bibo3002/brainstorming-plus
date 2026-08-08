# Brainstorming-Plus V2 — Cognitive Arsenal & Reference

## Table of Contents

1. [Lens vs Technique](#1-lens-vs-technique)
2. [The Seven Cognitive Lenses](#2-the-seven-cognitive-lenses) — Expand, Challenge, Transform, Reframe, Connect, Stress-test, Execute
3. [Escalation Ladder](#3-escalation-ladder) — Levels 0–6, from Clarify to Converge
4. [Heuristic Routing Table](#4-heuristic-routing-table) — condition → lens → technique lookup
5. [Cognitive State Signals (Internal)](#5-cognitive-state-signals-internal) — diagnostic signals and routing logic
6. [Convergence Detection](#6-convergence-detection) — recognizing when to stop generating
7. [Control Mode Behaviors](#7-control-mode-behaviors) — AUTO / GUIDED / MANUAL
8. [Anti-Pattern Reference](#8-anti-pattern-reference) — detection and correction table

## 1. Lens vs Technique

**A lens defines the cognitive objective; a technique is the mechanism used to achieve it.**

```
Lens: CHALLENGE
    ↓
Techniques:
    Assumption Testing
    Devil's Advocate
    Reverse Brainstorming
    Question Storming
```

The router selects a lens based on the diagnosed bottleneck, then selects the most appropriate technique within that lens.

---

## 2. The Seven Cognitive Lenses

### EXPAND

**Objective:** Broaden the solution space, perspectives, questions, or possibilities.

**Core question:** "What else could this be?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Starbursting | Generate questions around Who/What/Where/When/Why/How | Problem is defined but unexplored | Problem is still vague |
| Brainwriting | Independent parallel idea generation | Group settings; avoid anchoring | Solo quick decisions |
| Random Stimulus | Force new associations via unrelated input | Stagnation; ideas too similar | Problem needs precision, not novelty |
| Forced Connections | Combine unrelated concepts | Need unconventional angles | Constraints are very tight |
| Analogy | Transfer solutions from other domains | Problem is well-understood but stuck | Domain-specific precision required |

### CHALLENGE

**Objective:** Attack the idea, premise, or reasoning to expose weaknesses.

**Core question:** "Is our thinking or premise wrong?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Question Storming | Generate questions instead of answers | Premise is vague or untested | Problem is well-defined and clear |
| Devil's Advocate | Argue against the position | Overconfidence detected | User needs validation, not attack |
| Reverse Brainstorming | Imagine how to guarantee failure | Stagnation; need risk exposure | Early exploration phase |
| Assumption Testing | Identify and attack hidden assumptions | High assumption risk detected | Assumptions already validated |
| Reversal | Invert the problem statement | Stuck in one direction | Problem is genuinely one-directional |

### TRANSFORM

**Objective:** Change the structure of the idea deliberately.

**Core question:** "How can we mutate this into something different?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| SCAMPER | Substitute/Combine/Adapt/Modify/Put to other use/Eliminate/Reverse | Ideas are incremental variations | Need fundamental rethinking |
| Combination | Merge two or more concepts | Separate good ideas exist | Ideas are already integrated |
| Subtraction | Remove components to find essence | Overcomplexity detected | Simplicity already achieved |
| Exaggeration | Amplify or minimize attributes | Need to find breaking points | Precision is critical |
| Constraint Manipulation | Add/remove/modify constraints artificially | Stuck within current constraints | Constraints are genuinely fixed |

### REFRAME

**Objective:** See the problem from a fundamentally different perspective.

**Core question:** "What if the problem were something else entirely?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Five Whys | Trace root cause | Symptom-level problem definition | Root cause already known |
| Stakeholder Inversion | View from another actor's perspective | Single-perspective bias | All perspectives already considered |
| Jobs-to-be-Done | Identify underlying user motivation | Solution-focused without user need | User need already clear |
| Problem Inversion | Define the opposite problem | Stuck in original framing | Original framing is correct |
| Constraint Reframing | Redefine what the constraints mean | Constraints feel limiting | Constraints are genuinely absolute |
| Perspective Shifting | View from different time/scale/role | Need fresh angle | Angle already explored |

### CONNECT

**Objective:** Combine apparently unrelated concepts into new solutions.

**Core question:** "What happens when these collide?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Forced Connections | Merge unrelated elements | Need novelty; stagnation | Problem needs depth, not breadth |
| Morphological Matrix | Systematic combination of parameters | Multiple independent variables | Single-variable problem |
| Cross-industry Analogy | Import solutions from other fields | Domain thinking is exhausted | Domain-specificity is essential |
| Concept Fusion | Blend two ideas into a hybrid | Two partial solutions exist | Solutions are incompatible |
| Random Stimulus | Introduce chaos to break patterns | Deep stagnation | Problem needs focus |

### STRESS-TEST

**Objective:** Determine whether the idea survives contact with reality.

**Core question:** "Assuming the concept is valid, does it survive reality?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Pre-mortem | Imagine total failure; trace causes | Before commitment; high stakes | Early ideation phase |
| Edge Cases | Test boundary conditions | Design is mostly complete | Concept still forming |
| Failure Modes | Systematic failure analysis | Technical/engineering context | Pure strategy/creative work |
| Second-order Effects | Trace consequences of consequences | Systemic decisions | Simple isolated choices |
| Constraint Analysis | Test against real limitations | Feasibility uncertain | Feasibility already proven |

**CHALLENGE vs STRESS-TEST distinction:**
- CHALLENGE asks: "Is our thinking or premise wrong?"
- STRESS-TEST asks: "Given the concept is valid, does it survive reality?"

### EXECUTE

**Objective:** Translate an accepted direction into actionable structure.

**Core question:** "How do we operationalize this?"

| Technique | Purpose | When to Use | When NOT to Use |
|-----------|---------|-------------|-----------------|
| Decomposition | Break into smaller components | Direction accepted; need structure | Direction still uncertain |
| Critical Path | Identify dependencies and sequence | Multi-step implementation | Single-step action |
| MVP Thinking | Define minimum viable version | Need speed-to-learning | Perfection is required |
| Experiment Design | Create testable hypotheses | High uncertainty; need validation | Decision already validated |
| Resource Analysis | Identify what's needed | Planning phase | Pure ideation phase |
| Milestone Definition | Create checkpoints | Long timeline | Immediate action |

**Important:** The Execute lens produces plans, experiments, milestones, decomposition, sequencing, and acceptance criteria. It remains cognitive/design work. It does NOT produce implementation artifacts unless the process has explicitly transitioned to Handoff/Implementation.

---

## 3. Escalation Ladder

Escalation is conditional, not mandatory. Do not immediately deploy heavy frameworks. Start with low cognitive friction and escalate only when progress stalls.

**Levels 0–5 are exploration/escalation levels. Level 6 is the convergence phase, not a higher-intensity thinking level.**

| Level | Name | Purpose | Techniques |
|-------|------|---------|------------|
| 0 | Clarify | Determine what the user is actually trying to solve | Frame, Socratic questions, 5W1H, HMW |
| 1 | Diverge | Generate straightforward alternatives | Brainstorming, Starbursting, Question Storming |
| 2 | Reframe | Define the problem differently | Reversal, Analogy, Perspective shifting, Five Whys |
| 3 | Transform | Deliberately mutate the concepts | SCAMPER, Morphological Analysis, Combination, Subtraction |
| 4 | Attack | Assume failure; expose weaknesses | Reverse Brainstorming, Devil's Advocate, Pre-mortem |
| 5 | Radical | Remove major constraints; extreme scenarios | First Principles, Constraint inversion, Cross-domain synthesis |
| 6 | Converge | Stop generating. Synthesize. | Clustering, Pattern extraction, Prioritization, Decision matrix |

### Escalation Rule

> **Escalate only when the current level is unlikely to produce sufficient progress, or when the current intervention has failed to produce meaningful progress. Do not escalate merely because a more powerful technique exists.**

This means the engine may skip levels when diagnostic signals clearly indicate that a lower level is inadequate. For example:

```
Extremely entrenched assumption detected
        ↓
Diagnostic signal: assumption_risk = critical
        ↓
Level 1 (Diverge) clearly insufficient
        ↓
Route directly to Level 3 or 4
```

The AI should not deliberately waste a turn applying a weak technique when the diagnosis already shows it will fail.

---

## 4. Heuristic Routing Table

**The routing table provides candidate interventions, not mandatory mappings.** Select the least disruptive technique likely to address the detected bottleneck. Escalate only when the current intervention fails to produce meaningful progress.

| Detected Condition | Recommended Lens | Candidate Techniques |
|--------------------|-----------------|---------------------|
| Problem is vague / undefined | Reframe / Challenge | Question Storming / 5W1H |
| Premise appears questionable | Challenge | Assumption Testing / Reversal |
| One strong untested idea | Challenge | Assumption Testing / Pre-mortem |
| Few solution directions | Expand | Starbursting / Brainwriting |
| Ideas are repetitive / incremental | Transform / Connect | SCAMPER / Forced Connections |
| No new ideas emerging (stagnation) | Reframe / Transform | Reversal / SCAMPER / Random Stimulus |
| Several competing concepts | Connect or Stress-test | Morphological Analysis; then Evaluate → Trade-off Analysis |
| Need feasibility validation | Stress-test | Pre-mortem / Edge Cases |
| Need strategic alternatives | Expand / Reframe | Scenario Thinking / Cross-industry Analogy |
| Need implementation structure | Execute | Decomposition / Critical Path / MVP |
| User is stuck | Connect / Transform | Forced Connections / Random Stimulus |
| Too much complexity | Execute / Reframe | Decomposition / Simplification |
| Evidence is missing | — | Research / Evidence Gathering (exit brainstorming) |

### The "Don't Know" Route

If the diagnostic signal is ambiguous, choose the **least disruptive intervention that can reduce uncertainty**. Do not escalate merely because the optimal technique is unclear.

```
Uncertain diagnosis
      ↓
Clarifying question
      ↓
New information
      ↓
Reroute
```

NOT:

```
Uncertain diagnosis
      ↓
SCAMPER!
```

---

## 5. Cognitive State Signals (Internal)

The engine continuously estimates these signals. They are **heuristic estimates, not user-facing metrics**.

| Signal | Description |
|--------|-------------|
| clarity | How well-defined is the problem? |
| context_sufficiency | Do we have enough information to proceed? |
| novelty | Are ideas genuinely different? |
| diversity | Are ideas from different solution spaces? |
| depth | Are we beyond surface-level? |
| assumption_risk | Are hidden assumptions exposed? |
| stagnation | Are we repeating ourselves? |
| convergence_readiness | Can we move toward decision? |
| complexity | How complex is the problem? |
| uncertainty | What remains unknown? |

### Routing Logic Examples

```
high assumption_risk → Challenge → Assumption Testing
low novelty + high clarity → Transform → SCAMPER
high stagnation → Reframe or Attack → Reverse Brainstorming
high complexity → Execute → Decomposition
evidence missing → Exit → Research
```

---

## 6. Convergence Detection

The system must recognize when useful work has stopped:

> "We are no longer generating materially different ideas. Continuing the same technique will have diminishing returns."

### Convergence triggers:
- New ideas become structurally similar to existing ones
- User begins refining rather than generating
- Solution space has adequate coverage
- Trade-offs between top options are clear
- Remaining uncertainty requires evidence, not ideation

### Convergence actions:
- Cluster ideas into patterns
- Extract promising concepts
- Identify combinations
- Form winning hypotheses
- Design experiments or next steps

---

## 7. Control Mode Behaviors

### AUTO

AI selects the cognitive lens based on diagnostic signals.

> "Your idea is interesting, but the main weakness is an untested assumption. Let's start by questioning that assumption before generating more variations."

### GUIDED

AI recommends several lenses and lets the user choose.

> "I see three productive directions:
> 1. Challenge — attack the assumptions
> 2. Expand — generate alternative models
> 3. Transform — radically modify the concept
>
> My recommendation: Challenge. Which would you prefer?"

### MANUAL

User explicitly chooses the technique. AI uses the requested technique regardless of its heuristic recommendation, while still identifying material limitations, contradictions, or research requirements when relevant.

> User: "Use SCAMPER."
> AI: Applies SCAMPER immediately, while preserving relevant diagnostic or evidence requirements.

---

## 8. Anti-Pattern Reference

| Anti-Pattern | Detection | Correction |
|--------------|-----------|------------|
| Endless Interrogator | Questions exceed context sufficiency | Stop questioning; advance |
| Premature Convergence | Solution before problem validated | Route to Challenge/Reframe |
| Framework as Template | Tool applied without diagnosis | Return to diagnostic; choose minimum intervention |
| Metric Obsession | Treating signals as precise measurements | Use qualitative language; hide numbers |
| Technique Theater | Complex framework for simple problem | Simplify; use Level 0-1 intervention |
| Escalation Addiction | Escalating when clarification suffices | Check if Level 0-1 would resolve |
| False Precision | "Stagnation = 0.73" in natural dialogue | Rephrase as natural observation |
| Premature Meta-Discussion | Discussing methodology instead of problem | Return to user's actual problem |
