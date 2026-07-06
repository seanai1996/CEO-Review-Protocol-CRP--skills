<p align="center">
  <img src="https://img.shields.io/badge/status-stable-brightgreen" alt="Status: Stable">
  <img src="https://img.shields.io/badge/license-MIT-blue" alt="License: MIT">
  <img src="https://img.shields.io/badge/platforms-Claude%20Code%20%7C%20ChatGPT%20%7C%20Codex%20%7C%20Universal-8A2BE2" alt="Platforms">
</p>

<h1 align="center">🧠 CEO Review Protocol (CRP)</h1>
<p align="center"><em>A decision is only as good as the strongest challenge it survives.</em></p>

---

## What is CRP?

**CRP** (CEO Review Protocol) is a **structured multi-role decision framework** that transforms any strategic question from "what's the right answer?" into "what do four distinct perspectives reveal about the tradeoffs?"

Instead of giving a single recommendation, CRP forces a decision through four adversarial roles — ensuring blind spots are exposed, assumptions are stress-tested, and the final decision accounts for what could go wrong.

## Why CRP?

Most AI assistants give you **one answer** — a single perspective optimized for coherence and confidence. CRP is different:

| Traditional AI | CRP |
|:---|:---|
| One voice, one answer | Four roles with conflicting perspectives |
| Optimizes for sounding right | Tests for being wrong |
| Confirmation bias amplified | Confirmation bias neutralized |
| Answers "what should we do?" | Answers "what should we do, <em>and how could we be wrong?</em>" |

**Use CRP when:** the decision involves significant money, strategy, resources, or risk. Not for trivial choices.

## The Four Roles

| Role | Perspective | Role |
|:---|:---|:---|
| 🧠 **Advisor** | Builder / Optimist | "What's the best way forward?" |
| 🧨 **Devil** | Skeptic / Challenger | "Why is this wrong or risky?" |
| 📚 **Historian** | Pattern-matcher | "What does history tell us?" |
| 🧱 **Founder** | Integrator / Decider | "What do we actually do?" |

## The Seven Steps

Every CRP analysis follows this exact sequence:

```
1️⃣ Build (Advisor)      → Propose a concrete approach
2️⃣ Challenge (Devil)    → Attack it with 3+ distinct risks
3️⃣ Memory (Historian)   → Cite analogous patterns
4️⃣ Second-order Thinking → Model ripple effects
5️⃣ Decision             → Make a concrete call
6️⃣ Founder Filter       → Test vs strategy/resources
7️⃣ How Could We Be Wrong? → Find the failure modes
```

## Quick Start

### Claude Code

```bash
# Add to your skills directory
cp skills/crp/SKILL.md .claude/skills/crp/SKILL.md

# Then use:
/crp Should we pivot to enterprise or keep doing PLG?
```

### ChatGPT (GPTs)

1. Create a new GPT
2. In "Instructions", paste the content from `adaptations/chatgpt-gpts.md`
3. Done

### Any LLM

Paste the content from `adaptations/universal.md` into the system prompt.

### Codex

Add the instructions from `adaptations/codex.md` to your Codex system setup.

## Output Format

Every CRP response follows this exact structure:

```
──────── CEO REVIEW ────────

🧠 Build (Advisor)
[proposal]

🧨 Challenge (Devil)
[3+ risks]

📚 Memory (Historian)
[historical patterns]

🔍 Second-order Thinking
[ripple effects]

⚖️ Decision
[concrete recommendation]

🧱 Founder Filter
[strategy check]

⚠️ How Could We Be Wrong?
[failure conditions]

────────────────────────────
```

## Behavior Rules

| Rule | Why |
|:---|:---|
| ⚠️ No skipping roles | Each role catches different blind spots |
| ⚠️ Devil is mandatory | Without challenge, it's just confirmation |
| ⚠️ "How Could We Be Wrong?" required | The most important step |
| ⚠️ No averaging | Decision is a judgment, not a compromise |
| ⚠️ Distinct voices | If all roles agree, challenge harder |

## Repository Structure

```
CEO-Review-Protocol-CRP--skills/
├── skills/
│   └── crp/
│       └── SKILL.md              # Core skill definition (canonical)
├── adaptations/
│   ├── claude-code.md             # Claude Code /crp command
│   ├── chatgpt-gpts.md            # ChatGPT GPTs instructions
│   ├── codex.md                   # Codex adaptation
│   └── universal.md               # Pure system prompt (any LLM)
├── README.md                      # This file
├── CONTRIBUTING.md                # How to contribute
└── LICENSE                        # MIT
```

## Status

**Stable** — The core framework has been refined through hundreds of strategic reviews. Multi-platform adaptations are available and maintained.

## License

MIT — free for personal and commercial use. Improve the protocol and share back.

---

<p align="center">
  <em>Built for founders who want decisions, not opinions.</em>
</p>