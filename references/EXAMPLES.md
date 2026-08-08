# Brainstorming-Plus V2 — Validation Suite

This file contains seven test cases demonstrating how the Brainstorming-Plus V2 system should behave in different scenarios. These serve as a behavioral regression suite to ensure future updates do not violate the core architecture defined in `SKILL.md` and `REFERENCE.md`.

---

## Example 01: Simple Decision (Complexity Scaling + Evidence Discipline)

### Scenario

User needs to choose between two vendors for office supplies. Quick decision, low consequence, fully reversible.

### Expected Behavior

```text
AI detects: Low complexity, low consequence, high reversibility.
Complexity Level: A (Micro)
No escalation needed. No heavy frameworks.

AI asks ONE clarifying question:
"What matters most here — cost, reliability, or delivery speed?"

User answers: "Reliability is the absolute priority."

AI immediately recognizes an Evidence Sufficiency gap:

"Reliability is your priority, but we don't yet have comparable 
reliability data for the two vendors. Before making a confident 
recommendation, we should verify delivery performance and service 
history.

Evidence required:
- On-time delivery rate
- Service reliability / disruption history
- References from similar law firms

Once we have those facts, the decision will be straightforward."
```

### Validates:
- ✅ Adaptive exit criteria (Level A output)
- ✅ No unnecessary framework deployment
- ✅ Single question before convergence
- ✅ **Evidence Sufficiency** (prevents fabricated certainty)

---

## Example 02: Flawed Premise (Premise Sufficiency + Socratic Rule)

### Scenario

User says: "How do we make our client onboarding process 30% faster?"

### Expected Behavior

```text
AI detects: Premise may be questionable.
Process State: Frame → Explore
Cognitive Lens: Reframe
Escalation Level: 0 → 2

AI does NOT immediately generate speed optimization ideas.
AI strictly follows the one-question rule.

AI asks:
"Before optimizing speed, who actually experiences the onboarding 
process as slow: the client, the internal team, or both?"

User answers: "The internal team. Clients don't complain, but our 
paralegals are overwhelmed by redundant data entry."

AI asks the next progressive question:
"What would happen if we eliminated the redundant steps entirely 
rather than trying to type the data in faster?"

User realizes the process itself is the bottleneck, not the speed.

AI reframes:
"The problem isn't 'how to make onboarding faster.' 
It's 'how to eliminate redundant data entry so the team can focus 
on high-value client interaction.' Let's explore that direction."
```

### Validates:
- ✅ Premise Sufficiency check
- ✅ Reframe lens deployment
- ✅ **Strict adherence to the one-primary-question rule**
- ✅ Controlled loop (back to Frame/Explore)

---

## Example 03: Stagnated Brainstorming (Conditional Escalation)

### Scenario

User has been generating ideas for a new service offering. The last 5 ideas are variations of the same concept.

### Expected Behavior

```text
AI detects: High stagnation, low novelty, low diversity.
Process State: Ideate
Cognitive Lens: Transform → Challenge/Stress-test
Escalation Level: 1 → 3/4 (selected dynamically based on bottleneck)

AI (natural language, no metrics):
"We're generating variations of the same concept. More divergence 
in this direction is unlikely to help. Let's change the way we're 
approaching the problem.

Assume this service fails completely within 6 months. What caused 
the failure?"

User identifies: Distribution, not product quality.

AI:
"That's a significant insight. The limitation isn't the service — 
it's how clients discover it. Let's shift our lens to Connect 
and explore distribution partnerships."
```

### Validates:
- ✅ Stagnation detection
- ✅ **Conditional, non-deterministic escalation**
- ✅ Natural language transparency (no "stagnation = 0.78")
- ✅ Lens switch based on insight

---

## Example 04: Complex Software Architecture (Governed State Machine)

### Scenario

User is designing a document management system for a law firm. Multiple stakeholders, compliance requirements, integration needs.

### Expected Behavior

```text
AI detects: High complexity, multiple stakeholders, compliance constraints.
Complexity Level: C (Complex)
Process State: Frame → Explore → Understanding Lock → Ideate → Evaluate → Decide 
(with controlled loops if assumptions fail validation).

Phase 1 — Frame:
AI inspects context. Identifies: compliance requirements (Tunisian data 
protection law), existing systems, user roles, integration points.

Phase 2 — Explore (Socratic, one question at a time):
"What is the primary compliance constraint that would make or break 
this system?"
User: "Client confidentiality. Documents must be access-controlled 
per matter, per attorney."

Phase 3 — NFR Analysis:
AI identifies: Security, access control granularity, audit trail, 
performance under load, scalability.

Understanding Lock checkpoint: 
Before committing to the design direction, the AI summarizes its 
current understanding and requests confirmation.
"Let me confirm my understanding... Do you confirm this is accurate?"
User confirms.

Phase 4 — Ideate (2-3 approaches):
AI presents approaches with trade-offs.

Phase 5 — Decision Log:
Records decision, alternatives, cognitive triggers, unresolved uncertainty.

Phase 6 — Handoff:
Produces implementation-ready specification. Does NOT write code 
(Lens-Phase separation maintained).
```

### Validates:
- ✅ Level C output structure
- ✅ **Accurate representation of the governed state machine**
- ✅ Understanding Lock as a checkpoint, not a rigid permanent phase
- ✅ NFR analysis
- ✅ Lens-Phase separation (no code during design)

---

## Example 05: Strategic Transformation (Full Governance + Scaling)

### Scenario

A law firm is considering transforming from a traditional partnership model to a technology-enabled legal services platform. Timeline: جانفي through ديسمبر of the following year. Irreversible once committed.

### Expected Behavior

```text
AI detects: Transformational complexity, high consequence, high uncertainty, 
low reversibility.
Complexity Level: D (Transformational)
Process State: Full B+ governance with multiple controlled loops across 
Frame, Explore, Ideate, Evaluate, Decide, and Handoff.

Phase 1 — Frame & Explore:
AI maps the strategic landscape. Reaches Context Sufficiency, 
then Premise Sufficiency.

Phase 2 — Cognitive Engine activates:
Detects high assumption_risk → Routes to Challenge lens.

Possible illustrative escalation trajectory: Level 0 → 2 → 4.
(The actual escalation level is selected dynamically according to 
the diagnosed bottleneck and whether the current intervention is 
likely to produce sufficient progress).

AI applies Pre-mortem: "Assume it's ديسمبر next year and the 
transformation failed. What went wrong?"

Phase 3 — Convergence & Decision:
When Convergence Sufficiency is reached, AI synthesizes.
Presents 2-3 strategic approaches with full trade-off matrix.
Records comprehensive Decision Log (including cognitive triggers).

Phase 4 — Handoff:
Packages everything for implementation. Does NOT execute.
Requires explicit user authorization for any implementation step.
```

### Validates:
- ✅ Level D output structure
- ✅ **Correct terminology ("Full B+ governance across the six states")**
- ✅ **Illustrative, non-deterministic escalation trajectory**
- ✅ Tunisian month names used naturally
- ✅ Explicit authorization required for Implementation phase

---

## Example 06: User Manually Selects Technique (MANUAL Mode)

### Scenario

User says: "Use SCAMPER on our current client communication workflow."

### Expected Behavior

```text
AI detects: MANUAL control mode. User has explicitly chosen technique.

AI:
"Understood. I'll use SCAMPER rather than switching to another technique."

AI applies SCAMPER immediately without substituting its preferred 
technique. It may still identify material limitations or evidence 
requirements if relevant.

"Let's apply SCAMPER to your client communication workflow:

Substitute: What if we replaced email with a client portal?
Combine: What if we merged intake and status updates into one flow?
...
Reverse: What if the client initiated every interaction instead of us?

Which of these directions interests you most?"
```

### Validates:
- ✅ MANUAL mode respected (User choice overrides heuristic routing)
- ✅ AI does not override user choice
- ✅ **No unnecessary diagnostic discussion before applying the technique**
- ✅ AI retains ability to flag limitations if they arise during the exercise

---

## Example 07: Evidence Required (Research Exit)

### Scenario

User asks: "Which Tunisian tax structure would be most advantageous for this new business?"

### Expected Behavior

```text
AI detects: The question depends on current legal/fiscal facts rather 
than brainstorming alone.

AI does not launch SCAMPER, generate arbitrary alternatives, or 
pretend certainty.

AI identifies the required evidence:
- Applicable legal form (e.g., SUARL, SARL, Personne Physique)
- Current tax regime
- Relevant turnover/activity
- Applicable VAT/IR/IS rules
- Current legislative status

AI states:
"This cannot be resolved reliably through brainstorming alone. 
We first need to establish the applicable legal and fiscal rules. 
Once those facts are verified, we can brainstorm the available 
strategic options."
```

### Validates:
- ✅ **Evidence Sufficiency**
- ✅ **Research exit** (stops brainstorming when facts are needed)
- ✅ No fabricated certainty
- ✅ No unnecessary cognitive framework deployment
- ✅ Clear separation between reasoning and factual verification

---

## Regression Testing Protocol

When updating Brainstorming-Plus V2, validate against all seven examples:

| # | Test Case | Primary Behavior Validated |
|---|-----------|----------------------------|
| 01 | Simple Decision | Complexity scaling + evidence discipline |
| 02 | Flawed Premise | Premise Sufficiency + one-question rule |
| 03 | Stagnation | Convergence detection + conditional escalation |
| 04 | Complex Architecture | Understanding Lock + NFRs + governed state machine |
| 05 | Strategic Transformation | Full B+ governance + controlled loops + scaling |
| 06 | Manual Technique | User override + lens/technique separation |
| 07 | Evidence Required | Evidence Sufficiency + research exit |

### Pass Criteria

All seven examples must produce behavior consistent with:
- Adaptive complexity scaling
- Sufficiency-based transitions (Context, Premise, Divergence, Convergence, Evidence)
- Invisible machinery / visible intelligence
- Lens-Phase separation (Execute lens ≠ Implementation authorization)
- Progressive, conditional escalation
- User agency preserved