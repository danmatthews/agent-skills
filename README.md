# agent-skills

A collection of agent skills, installable with [`skills`](https://github.com/vercel-labs/skills).

## Install

```bash
# Install all skills
npx skills add danmatthews/agent-skills

# List the available skills
npx skills add danmatthews/agent-skills --list

# Install a specific skill
npx skills add danmatthews/agent-skills --skill <skill-name>
```

## Structure

Each skill lives in its own folder under `skills/`, with a `SKILL.md` at its root:

```
skills/
  <skill-name>/
    SKILL.md        # required: frontmatter + instructions
    scripts/        # optional: helper scripts
    references/     # optional: extra docs loaded on demand
    assets/         # optional: templates, files used in output
```

`SKILL.md` starts with YAML frontmatter:

```markdown
---
name: skill-name
description: What the skill does and when the agent should use it.
---

# Skill Name

Instructions for the agent...
```

The `name` must match the folder name (lowercase, hyphen-separated).
