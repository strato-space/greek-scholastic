# Greek Scholastic

Public repository for the `greek-scholastic` Codex skill.

## Contents

- [`greek-scholastic/SKILL.md`](./greek-scholastic/SKILL.md) — the skill definition
- [`greek-scholastic/agents/openai.yaml`](./greek-scholastic/agents/openai.yaml) — UI metadata for skill installers and clients
- [`.claude/commands/greek-scholastic.md`](./.claude/commands/greek-scholastic.md) — ready-to-copy Claude Code slash command template
- [`.cursor/rules/greek-scholastic.mdc`](./.cursor/rules/greek-scholastic.mdc) — ready-to-copy Cursor rule template

## Install

### Codex

Recommended install style is URL-first through the built-in `$skill-installer`, using the GitHub skill path directly:

```text
Use $skill-installer to install https://github.com/strato-space/greek-scholastic/tree/main/greek-scholastic
```

This keeps the instruction at the product level instead of exposing an implementation-specific helper script path.

Direct equivalent GitHub URL:

```text
https://github.com/strato-space/greek-scholastic/tree/main/greek-scholastic
```

After installing, restart Codex to pick up the new skill.

## Claude Code

Claude Code does not use the Codex skill format directly. The closest official equivalent is a custom slash command stored as Markdown.

Recommended setup:

1. Copy [`.claude/commands/greek-scholastic.md`](./.claude/commands/greek-scholastic.md) into:
   - project scope: `.claude/commands/greek-scholastic.md`
   - user scope: `~/.claude/commands/greek-scholastic.md`
2. Invoke it in Claude Code as:

```text
/greek-scholastic
```

Official references:
- Anthropic docs: custom slash commands in `.claude/commands/` / `~/.claude/commands/`
- https://docs.anthropic.com/en/docs/claude-code/slash-commands

Comparison note:

- A widely used Claude Code command repository, `wshobson/commands`, documents installation at the GitHub-repo level (`git clone` into `~/.claude`) and also points to a higher-level marketplace path, rather than exposing low-level internal helper scripts.
- This README now follows the same repo-level / URL-first installation style for Codex.

## Cursor

Cursor also does not use the Codex skill format directly. The closest official equivalents are:

- a Project Rule in `.cursor/rules`
- a User Rule in `Cursor Settings -> Rules`
- or an `AGENTS.md` file as a simple markdown-based alternative

Recommended setup:

1. Copy [`.cursor/rules/greek-scholastic.mdc`](./.cursor/rules/greek-scholastic.mdc) into your project’s `.cursor/rules/`.
2. Or adapt the same text into a User Rule / `AGENTS.md` setup if you prefer.
3. Use it as a reusable reasoning rule for critique, ontology checks, and modality analysis.

Official references:
- Cursor Rules docs: project rules in `.cursor/rules`, user rules in settings, `AGENTS.md` as an alternative
- https://docs.cursor.com/en/context/rules
