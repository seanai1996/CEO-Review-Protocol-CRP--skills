# Contributing to CEO Review Protocol (CRP)

Thanks for your interest in improving CRP!

## Ways to Contribute

- **Platform adaptations** — Add support for more AI platforms (Cursor, Windsurf, Continue.dev, etc.)
- **Use case examples** — Share real CRP outputs with context so others can learn from them
- **Bug fixes** — Clarify rules, improve wording, fix broken links
- **Behavior improvements** — Strengthen role definitions, close loopholes in auto-trigger logic

## Adding a Platform Adaptation

1. Create a new file in `adaptations/` with the platform name (e.g., `adaptations/cursor.md`)
2. Follow the same structure as existing adaptations:
   - Clarify trigger mechanism for the platform
   - Translate the four roles and seven steps into platform-native format
   - Include the output format template
   - Document behavior rules in platform-native terms
3. Submit a PR with a brief description of the platform's differences

## Skill Changes

If you improve the core `skills/crp/SKILL.md`:
- Keep the YAML frontmatter valid
- Maintain backward compatibility with existing adaptations (or update them too)
- Test your changes with at least one strategic decision scenario

## PR Process

1. Fork the repo
2. Create a branch with a descriptive name
3. Make your changes
4. Submit a PR — short description of what and why