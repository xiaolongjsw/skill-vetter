---
name: skill-vetter
description: "Evaluates and validates OpenClaw skills. Use when: (1) User asks to check a skill, (2) Skill installation fails, (3) Skill behavior is unexpected, (4) User wants to validate skill compatibility."
---

# Skill Vetter

Evaluates and validates OpenClaw skills for functionality, security, and compatibility.

## Quick Reference

| Situation | Action |
|-----------|--------|
| Check skill status | List installed skills in ~/.openclaw/skills/ |
| Validate skill | Read SKILL.md and check required dependencies |
| Test skill | Run skill scripts if available |
| Report issues | Document errors and suggest fixes |

## Usage

```bash
# List all installed skills
ls ~/.openclaw/skills/

# Check specific skill
cat ~/.openclaw/skills/[skill-name]/SKILL.md

# Validate skill structure
python3 ~/.openclaw/skills/[skill-name]/scripts/validate.py
```

## Skill Requirements

- Must have SKILL.md with name and description
- Should have clear documentation
- Scripts should be executable
- Dependencies should be listed
