<img width="1280" height="640" alt="logo3" src="https://repository-images.githubusercontent.com/1299189033/ba2bd2de-4547-458c-9898-bd63c488ea35" />

# Brainstorming-Plus V2

> A high-level cognitive sparring partner for brainstorming, strategic thinking, problem-solving, design decisions, and idea evaluation.

[![skills.sh](https://img.shields.io/badge/skills.sh-Registry-000000?logo=vercel&logoColor=white)](https://www.skills.sh/bibo3002/brainstorming-plus/brainstorming-plus)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-2.0.0-blue)](https://github.com/bibo3002/brainstorming-plus/releases/tag/v2.0.0)

**English** | [Français](ReadMe.fr.md) | [العربية](ReadMe.ar.md)

---

## 🤖 What Is Brainstorming-Plus?

Brainstorming-Plus is a high-level thinking partner — acting alternately as a **design facilitator**, **senior reviewer**, or **critical sparring partner**. Unlike a simple execution tool, this Skill aims to push you to your limits, provide unexpected perspectives, and help you arrive at ideas you wouldn't have reached on your own.

It transforms your AI coding assistant or agent (Codex, OpenCode, Claude, etc.) into a senior strategic partner that prevents premature convergence, challenges flawed premises, and guides you through structured cognitive phases.

### 🧠 Logic & Philosophy

The fundamental logic of this Skill is based on **structured interaction** and a **strong opinion**:

| Principle | Description |
|-----------|-------------|
| **Partner, not builder** | The Skill does not code or modify behaviors during the thinking phase; it focuses exclusively on design and intellectual validation. |
| **Constructive contradiction** | Designed to challenge your assumptions ("This assumes X — are we sure about that?") and prevent premature convergence toward a solution. |
| **Divergence before convergence** | Encourages the exploration of multiple options before settling on a final choice. |

### 🎯 Objectives

- Transform raw ideas into **validated specifications** through structured dialogue.
- Avoid common pitfalls (anti-patterns) such as developing solutions before defining the problem, or the trap of functional parity with competition.
- Ensure shared clarity on the **"what"**, the **"why"**, and the **"for whom"** before writing a single line of code.
- Ensure **technical rigor** by systematically integrating non-functional requirements (performance, scalability, security).

---

## 🎯 When to Use It

✅ Think through a problem or generate/refine ideas
✅ Challenge an assumption or weigh trade-offs
✅ Plan a project, feature, or strategic initiative
✅ Work through an ambiguous or open-ended decision
✅ Get a second opinion or break out of a mental loop
✅ Structure a decision (options → risks → trade-offs → next steps)

### Adaptive Brainstorming Modes

The skill adapts its behavior according to the state of your thinking:

| Mode | When |
|------|------|
| **Problem Exploration** | The problem is not yet defined |
| **Solution Ideation** | The problem is clear but requires divergent ideas |
| **Hypothesis Testing** | Stress-test a previously chosen direction |
| **Strategic Exploration** | Long-term decisions and positioning |

## 🚫 When NOT to Use It

❌ Simple factual lookups
❌ Direct code generation with a clear spec
❌ Tasks where you already have an accepted plan and just need execution

---

## 📦 Global Installation (Multi-Agent)

Because Agent Skills have standardized around the `SKILL.md` format, you can install Brainstorming-Plus globally so it is available across **all** your repositories and projects.

### Option 1: The `skills.sh` Registry (Recommended)

```bash
npx skills add bibo3002/brainstorming-plus --global
```

### Option 2: Manual Global Installation

Clone this repository and copy it to your agent's global skills directory:

| Agent / Platform | Global Skills Directory |
| :--- | :--- |
| **OpenAI Codex CLI** | `~/.agents/skills/brainstorming-plus/` |
| **OpenCode** | `~/.config/opencode/skills/brainstorming-plus/` |
| **Claude Code** | `~/.claude/skills/brainstorming-plus/` |

```bash
# Universal bash command to install globally
git clone https://github.com/bibo3002/brainstorming-plus.git /tmp/brainstorming-plus

# For Codex CLI
cp -r /tmp/brainstorming-plus ~/.agents/skills/

# For OpenCode
cp -r /tmp/brainstorming-plus ~/.config/opencode/skills/

# For Claude Code
cp -r /tmp/brainstorming-plus ~/.claude/skills/
```

---

## 🏗️ Core Architecture

Brainstorming-Plus V2 is governed by **two independent, interacting layers**:

| Layer | Role | Question it answers |
|-------|------|-------------------|
| **Governance Layer** | Process structure: framing, Socratic clarification, Understanding Lock, alternatives, trade-offs, decision logging, handoff | *Where are we in the process?* |
| **Cognitive Engine** | Adaptive intelligence: selects the right thinking intervention next via heuristic routing, progressive escalation, and convergence detection | *What kind of thinking should happen now?* |

### The Three Control Axes

| Axis | Question | Values |
|------|----------|--------|
| **Process State** | Where are we? | Frame → Explore → Ideate → Evaluate → Decide → Handoff |
| **Cognitive Lens** | How should we think? | Expand → Challenge → Transform → Reframe → Connect → Stress-test → Execute |
| **Control Mode** | Who chooses? | AUTO → GUIDED → MANUAL |

### Process States (Governed State Machine)

The process is a **governed state machine with controlled loops**, not a rigid linear sequence:

```
Frame → Explore → Ideate → Evaluate → Decide
                                         │
                                         │ user approves design
                                         ▼
                                      Handoff
                                         │
                                         │ implementation authorization
                                         ▼
                                   Implementation
```

The engine may loop backward when a fundamental assumption fails validation.

### The Seven Cognitive Lenses

| Lens | Core Question | Example Techniques |
|------|--------------|-------------------|
| 🔍 **Expand** | "What else could this be?" | Starbursting, Brainwriting, Analogy |
| ⚔️ **Challenge** | "Is our thinking wrong?" | Devil's Advocate, Assumption Testing |
| 🔧 **Transform** | "How can we mutate this?" | SCAMPER, Subtraction, Exaggeration |
| 🔄 **Reframe** | "What if the problem were different?" | Five Whys, Jobs-to-be-Done |
| 🔗 **Connect** | "What happens when these collide?" | Morphological Matrix, Concept Fusion |
| 🧪 **Stress-test** | "Does it survive reality?" | Pre-mortem, Edge Cases, Failure Modes |
| 🚀 **Execute** | "How do we operationalize this?" | Decomposition, Critical Path, MVP |

> 📖 Full technique reference: [references/REFERENCE.md](references/REFERENCE.md)

### Tools & Frameworks Available

Depending on the needs, the Skill uses structured thinking tools such as:

- **Jobs-to-be-Done (JTBD)** — Understand users' underlying motivations.
- **SCAMPER** — Transform an existing product or idea.
- **OODA Loop** — Rapid decision-making in competitive environments.
- **Reverse Brainstorming** — Identify risks by imagining how to make the project fail.
- **Pre-mortem** — Assume total failure and trace causes backward.
- **Five Whys** — Trace root cause of a problem.

> 📖 Complete arsenal with when-to-use guidance: [references/REFERENCE.md](references/REFERENCE.md)

---

## ⚙️ Control Modes

| Mode | Behavior |
|------|----------|
| **AUTO** (default) | AI selects the cognitive lens based on diagnostic signals |
| **GUIDED** | AI recommends 2–3 lenses; you choose |
| **MANUAL** | You explicitly select the technique; AI applies it |

Switch modes naturally in conversation:
- *"I'd like you to choose the best approach."* → AUTO
- *"Show me my options for how to think about this."* → GUIDED
- *"Use SCAMPER on this."* → MANUAL

---

## 📊 Complexity Scaling

The depth of analysis adapts to the decision's complexity:

| Level | Type | Output |
|-------|------|--------|
| **A — Micro** | Quick, reversible decisions | Problem → Options → Recommendation |
| **B — Standard** | Moderate complexity | Framing → Assumptions → 2–3 approaches → Trade-offs |
| **C — Complex** | Multiple stakeholders, significant trade-offs | Understanding Lock → NFRs → Approaches → Decision Log |
| **D — Transformational** | Organization-wide, irreversible | Full Design Doc → Scenario Analysis → Roadmap |

---

## 🔑 The Golden Rule: Lens–Phase Separation

> **The Execute lens structures how to operationalize an accepted direction. It does NOT authorize implementation.**

| Concept | Meaning | Can produce code? |
|---------|---------|-------------------|
| **Execute lens** | Think about how to turn an accepted direction into action | ❌ No |
| **Handoff** | Package the approved reasoning/design for implementation | 📦 Implementation-ready artifacts |
| **Implementation** | Transition from reasoning/design into actual building | ✅ Yes, when explicitly authorized |

---

## 🚦 Exit Criteria

The Skill considers the session complete only when:

- ✅ The design or decision is sufficiently developed and approved.
- ✅ Risks are acknowledged.
- ✅ The **Decision Log** is created when applicable.
- ✅ Unresolved uncertainties are explicitly identified.
- ✅ The user has clear next actions or a defined Handoff.

---

## 📂 File Structure

| File | Purpose |
| :--- | :--- |
| `SKILL.md` | Core skill definition — process governance, lenses, Socratic rules, sufficiency conditions, transparency model |
| `references/REFERENCE.md` | Full Cognitive Arsenal: all 7 lenses with techniques, Escalation Ladder, Heuristic Routing Table, Anti-Pattern Reference |
| `references/EXAMPLES.md` | 7 worked scenarios demonstrating expected behavior (simple decision → strategic transformation) |

---

## 📖 Examples

Seven detailed worked examples demonstrating the skill in action:

| # | Scenario | Key Behavior Validated |
|---|----------|----------------------|
| 01 | Simple vendor decision | Complexity scaling + evidence discipline |
| 02 | Flawed premise (speed optimization) | Premise Sufficiency + one-question rule |
| 03 | Stagnated brainstorming | Convergence detection + conditional escalation |
| 04 | Complex software architecture | Understanding Lock + NFRs + governed state machine |
| 05 | Strategic transformation | Full governance + controlled loops + scaling |
| 06 | Manual technique selection | User override + lens/technique separation |
| 07 | Evidence required (tax question) | Evidence Sufficiency + research exit |

> 📖 Full examples: [references/EXAMPLES.md](references/EXAMPLES.md)

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) first.

## 📝 Changelog

See [CHANGELOG.md](CHANGELOG.md) for release history.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 👤 Author

**Habib Farhat** — Tunisian Lawyer & AI Skill Designer
