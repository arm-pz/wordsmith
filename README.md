# Agent Skill Template

A starter repo for creating reusable AI agent skills in the `SKILL.md` format.

## Create a skill from this template

1. Create a new repository from this GitHub template.
2. Replace `my-skill` with your skill's name.
3. Edit `skills/my-skill/SKILL.md`.
4. Add optional examples or reference files inside `skills/my-skill/`.
5. Test the skill using prompts in `tests/test-prompts.md`.
6. Install the skill folder in the location your AI agent uses.

The skill folder contains the skill itself. The `tests/` folder is for people testing the skill; it is not needed when installing the skill.

## Install a skill

Copy the complete skill folder—not just `SKILL.md`—to the project-level location for your agent:

| Agent | Project-level location |
|---|---|
| Claude Code | `.claude/skills/<skill-name>/` |
| Codex | `.agents/skills/<skill-name>/` |
| Cursor | `.agents/skills/<skill-name>/` or `.cursor/skills/<skill-name>/` |
| Qoder | `.qoder/skills/<skill-name>/` |

For example, install Wordsmith by copying its folder to
`.claude/skills/wordsmith/` for Claude Code, or
`.agents/skills/wordsmith/` for Codex.

The same skill files can be copied to more than one agent's skill directory.

## Skill file requirements

Each skill folder needs a `SKILL.md` file. It begins with YAML metadata containing:

- `name`: a short identifier using lowercase letters and hyphens
- `description`: what the skill does and the kinds of requests that should activate it

The Markdown body contains the skill instructions.

## Test checklist

- Does the skill activate for the requests it is meant to handle?
- Does it follow its own instructions?
- Does it handle vague requests sensibly?
- Does it avoid inventing facts?
- Are the results useful and distinct across different test prompts?
