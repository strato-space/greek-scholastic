# Greek Scholastic

Public repository for the `greek-scholastic` Codex skill.

## Contents

- `greek-scholastic/SKILL.md` — the skill definition
- `greek-scholastic/agents/openai.yaml` — UI metadata for skill installers and clients

## Install

Example installation from GitHub:

```bash
python /root/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo strato-space/greek-scholastic \
  --path greek-scholastic
```

After installing, restart Codex to pick up the new skill.

## Claude Code

Claude Code does not use the Codex skill format directly. The closest official equivalent is a custom slash command stored as Markdown.

Recommended setup:

1. Create a project command or a personal command:
   - project scope: `.claude/commands/greek-scholastic.md`
   - user scope: `~/.claude/commands/greek-scholastic.md`
2. Copy the body of [`greek-scholastic/SKILL.md`](./greek-scholastic/SKILL.md) into that file.
3. Invoke it in Claude Code as:

```text
/greek-scholastic
```

Official references:
- Anthropic docs: custom slash commands in `.claude/commands/` / `~/.claude/commands/`
- https://docs.anthropic.com/en/docs/claude-code/slash-commands

## Cursor

Cursor also does not use the Codex skill format directly. The closest official equivalents are:

- a Project Rule in `.cursor/rules`
- a User Rule in `Cursor Settings -> Rules`
- or an `AGENTS.md` file as a simple markdown-based alternative

Recommended setup:

1. Create a project-scoped Cursor rule or project `AGENTS.md`.
2. Paste the body of [`greek-scholastic/SKILL.md`](./greek-scholastic/SKILL.md).
3. Use it as a reusable reasoning rule for critique, ontology checks, and modality analysis.

Suggested project-scoped path:

```text
.cursor/rules/greek-scholastic.mdc
```

Official references:
- Cursor Rules docs: project rules in `.cursor/rules`, user rules in settings, `AGENTS.md` as an alternative
- https://docs.cursor.com/en/context/rules
