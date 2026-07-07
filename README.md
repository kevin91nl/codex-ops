# Codex Ops

Home for reusable Codex automations, skills, helper scripts, checklists, and shared operating rules.

## Layout

- `automations/`: reusable automation prompts and metadata.
- `skills/`: future Codex skills. Add one folder per skill, each with its own `SKILL.md`.
- `AGENTS.md`: repo-local rules for agents working in this repository.

## Install

Clone or move this repo wherever you keep personal Codex assets:

```bash
git clone https://github.com/kevin91nl/codex-ops.git
cd codex-ops
```

To update later:

```bash
git pull --ff-only
```

To reuse an automation:

1. Open the automation folder.
2. Copy `prompt.md` into a Codex automation.
3. Pick a schedule in Codex.
4. Keep the prompt in Git as the source of truth.

## Automations

`automations/self-optimization/` contains the Codex self-optimization review automation. Its purpose is to inspect recent Codex session history, workspace guidance, reusable artifacts, and current research-backed practices, then make at most one high-leverage improvement that reduces repeated work, token burn, avoidable retries, or user intervention.

`automations/repository-upkeep/` contains a small upkeep automation. Its purpose is to let Codex keep a local clone of this repository up to date with `git pull --ff-only`, while stopping if local changes need human review.

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
