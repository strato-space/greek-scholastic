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
