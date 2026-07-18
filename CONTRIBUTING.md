# Contributing to CRP

Thanks for your interest in improving CRP!

## Ways to Contribute

- **Platform adaptations** — Add support for more AI platforms (Cursor, Windsurf, Continue.dev, etc.)
- **Use case examples** — Share real CRP outputs with context so others can learn from them
- **Bug fixes** — Clarify rules, improve wording, fix broken links
- **Behavior improvements** — Strengthen role definitions, close loopholes in auto-trigger logic

## Adding a Platform Adaptation

1. Create a new file in `adaptations/` with the platform name (e.g., `adaptations/cursor.md`)
2. Follow the same structure as existing adaptations:
   - Clarify the trigger mechanism for both `crp:decision` and `crp:content`
   - Translate the role sets and output formats into platform-native format
   - Include guidance for when to use each skill
   - Document behavior rules in platform-native terms
3. Submit a PR with a brief description of the platform's differences

## Skill Changes

If you improve the core skills:
- Keep the YAML frontmatter valid
- Maintain backward compatibility with existing adaptations, or update them too
- Update both `skills/crp-decision/SKILL.md` and `skills/crp-content/SKILL.md` when the shared CRP behavior changes
- Test your changes with at least one strategic decision scenario and one content review scenario
- New roles or steps must be added after existing ones (don't reorder)

## PR Process

1. Fork the repo
2. Create a branch with a descriptive name
3. Make your changes
4. Submit a PR — short description of what and why
