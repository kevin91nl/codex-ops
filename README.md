# Codex Ops

Home for reusable Codex automations, skills, helper scripts, checklists, and shared operating rules.

## Layout

- `automations/`: reusable automation prompts and metadata.
- `skills/`: future Codex skills. Add one folder per skill, each with its own `SKILL.md`.
- `AGENTS.md`: repo-local rules for agents working in this repository.

## Install

Clone or move this repo wherever you keep personal Codex assets:

```bash
git clone <repo-url> codex-ops
```

For local use:

```bash
cd codex-ops
```

To reuse an automation, open the automation folder, copy the prompt into a Codex automation, and set the schedule in Codex. Keep the prompt in Git as the source of truth.

## Current Automation

`automations/self-optimization/` contains the Codex self-optimization review automation. Its purpose is to inspect recent Codex session history, workspace guidance, reusable artifacts, and current research-backed practices, then make at most one high-leverage improvement that reduces repeated work, token burn, avoidable retries, or user intervention.

Files:

- `automation.toml`: human-readable metadata.
- `prompt.md`: the full automation prompt.

## Adding Skills

Create a new folder under `skills/`:

```bash
mkdir -p skills/my-skill
touch skills/my-skill/SKILL.md
```

Keep skills narrow, executable, and backed by concrete trigger rules. Prefer helpers or checklists when a full skill would add ceremony without reducing repeated work.
