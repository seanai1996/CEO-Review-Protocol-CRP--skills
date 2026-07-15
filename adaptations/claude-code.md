---
name: crp-claude-code
description: CRP (CEO Review Protocol) adaptation for Claude Code — /crp command and auto-trigger
---

# Claude Code — CRP Adaptation

Place `skills/crp/SKILL.md` in your `.claude/skills/crp/` directory for skill-based access.

## /crp Command

Add to `.claude/commands/crp.md`:

```markdown
---
name: crp
description: Run the CEO Review Protocol — structured multi-role decision analysis
---

# /crp

Run a CEO Review Protocol (CRP) analysis on a strategic question.

## How to use

```
/crp [your strategic question]
```

Example:
```
/crp We have $50k runway, 200 free users, 0 paying. Pivot to enterprise or double down on PLG?
```

## What happens

The agent activates the CRP framework with five roles (Advisor, Devil, Historian, Budget Steward, Founder) and executes eight steps:

1. **Build** — Advisor proposes solution
2. **Challenge** — Devil attacks (3+ risks)
3. **Memory** — Historian cites patterns
4. **Budget Review** — Budget Steward evaluates cost feasibility
5. **Second-order Thinking** — Ripple effects
6. **Decision** — Concrete recommendation
7. **Founder Filter** — Strategic consistency check
8. **How Could We Be Wrong?** — Anti-fragility check

## Auto-trigger

The agent also auto-triggers CRP when detecting strategic decision signals: resource allocation, product tradeoffs, risk assessment, pricing decisions, hiring decisions, or "should we do X" with significant impact.
```