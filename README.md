# ReproNim Skills

A collection of skills for AI coding agents tailored to [ReproNim](https://www.repronim.org/) tools and neuroimaging workflows. Skills are packaged instructions that extend AI agent capabilities when working with ReproNim's ecosystem of tools.

Skills follow the [Agent Skills](https://agentskills.io/) format and are compatible with **Claude Code**, **GitHub Copilot**, **Cursor**, and other AI coding agents.

## Available Skills

Skills are located in the [`skills/`](./skills/) directory. Each skill is a single Markdown file (e.g., `skills/my-skill.md`) containing structured instructions for the agent.

> No skills have been added yet. See [Contributing](#contributing) to add one.

## Installation

```bash
npx skills add ReproNim/skills
```

### Install a specific skill

```bash
npx skills add ReproNim/skills --skill <skill-name>
```

### Install to a specific agent

```bash
npx skills add ReproNim/skills -a claude-code
npx skills add ReproNim/skills -a cursor
```

## Purpose

This repository provides reusable, shareable AI agent skills for the ReproNim community. Skills encode domain knowledge about:

- ReproNim tools and best practices (e.g., DataLad, Neurodocker, ReproSchema)
- Neuroimaging data management and FAIR data principles
- Reproducible research workflows
- BIDS (Brain Imaging Data Structure) conventions

By packaging this knowledge as agent skills, researchers and developers get consistent, expert guidance directly inside their AI coding assistant.

## Skill Structure

Each skill is a single Markdown file placed directly in the `skills/` directory:

```
skills/
└── my-skill.md    # SKILL.md-format file describing the skill
```

### Skill file format

```markdown
---
name: repronim-my-skill
description: >
  Brief description of when and how to use this skill.
license: MIT
metadata:
  author: ReproNim
  version: 1.0.0
---

# My Skill

## When to Apply

...

## Guidelines

...
```

## Contributing

1. Create a new Markdown file in the `skills/` directory (e.g., `skills/datalad-best-practices.md`).
2. Follow the skill file format above.
3. Update this README to list the new skill under [Available Skills](#available-skills).
4. Open a pull request.

## License

MIT
