# Codex Ops Repository Upkeep

Keep the local `codex-ops` repository clone up to date.

Steps:

1. Locate the local `codex-ops` clone. If no clone exists, clone `https://github.com/kevin91nl/codex-ops.git` into a user-approved or conventional personal tools directory.
2. Run `git status --short`.
3. If there are local changes, stop and report the changed files. Do not stash, reset, checkout, or overwrite.
4. Verify the remote is `https://github.com/kevin91nl/codex-ops.git`.
5. Run `git pull --ff-only`.
6. Report the previous HEAD, new HEAD, and whether anything changed.

Guardrails:

- No force push.
- No destructive Git commands.
- No broad repository or home-directory scans.
- Do not install or overwrite Codex automations unless explicitly asked.
- Treat `automation.toml` as metadata and `prompt.md` as the prompt source of truth.
