# CRP Maintenance Plan

> **Status:** Active — Last updated 2026-07-18

## Why This Document Exists

CRP has grown from a single skill into two skills — `crp:decision` and `crp:content`. This increases the complexity. Future updates should follow this reference to avoid deleting or breaking critical files.

## File Map

### Canonical Skill Definitions (the source of truth)

| File | Purpose |
|------|---------|
| `skills/crp-decision/SKILL.md` | Core decision skill — roles, steps, output format, behavior rules |
| `skills/crp-content/SKILL.md` | Core content skill — roles, workflow, output format, behavior rules |

**Rule:** Do NOT delete or rename these files. Every other file in the repo derives from them.

### Platform Adaptations (derived from skills)

| File | Platform |
|------|----------|
| `adaptations/claude-code.md` | Claude Code skill setup, slash commands, auto-trigger guidance |
| `adaptations/chatgpt-gpts.md` | ChatGPT GPTs instructions for both skills |
| `adaptations/codex.md` | Codex system prompt addition for both skills |
| `adaptations/universal.md` | Minimal system prompt for any LLM |

**Rule:** When the core skill files change, check each adaptation to keep them in sync.

### Repo-Level Docs

| File | Purpose |
|------|---------|
| `README.md` | Public-facing overview, quick start, repo structure |
| `CONTRIBUTING.md` | Contribution guide, PR process |
| `LICENSE` | MIT license |
| `MAINTENANCE.md` | This file — internal maintenance reference |

## Update Checklist

When making a change to CRP, follow this order:

1. **Design the change** — decide what changes and why
2. **Update skill file(s)** — `skills/crp-decision/SKILL.md` and/or `skills/crp-content/SKILL.md`
3. **Sync adaptations** — check all four files in `adaptations/`
4. **Sync README** — if the change affects user-facing behavior or quick-start examples
5. **Sync CONTRIBUTING** — if the contribution process changed
6. **Commit** — single commit with a descriptive message

## Critical Rules

- **Never delete `skills/` directory or either sub-skill**
- **Never rename skill files** — skill names in frontmatter must match the directory names
- **Keep everything in English** — no mixed-language content
- **Backward compatible** — changes should not break existing installations
- **Frontmatter format:** `name` field uses `crp:` namespace (e.g., `crp:decision`)

## Repository Structure (Snapshot)

```
CRP-CEO-Review-Protocol/
├── skills/
│   ├── crp-decision/
│   │   └── SKILL.md
│   └── crp-content/
│       └── SKILL.md
├── adaptations/
│   ├── claude-code.md
│   ├── chatgpt-gpts.md
│   ├── codex.md
│   └── universal.md
├── README.md
├── CONTRIBUTING.md
├── MAINTENANCE.md
└── LICENSE
```