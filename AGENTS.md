Caveman ultra.

- Do not run broad `rg` across whole roots or multiple roots at once.
- Do not use `view_image` or large CI/binary outputs unless exactly needed.
- Use `apply_patch` for edits.
- Install by cloning `https://github.com/kevin91nl/codex-ops.git` into a user-chosen directory.
- Update an existing clone with `git pull --ff-only`.
- To install an automation, copy `automations/<name>/prompt.md` into a Codex automation prompt; `automation.toml` is metadata, not runtime config.
- Keep local changes visible: check `git status --short` before pull or push.
