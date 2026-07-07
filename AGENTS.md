Caveman ultra.

- Geen brede `rg` over hele roots of meerdere roots tegelijk.
- Geen `view_image` of grote CI/binary outputs tenzij exact nodig.
- Bij edits: `apply_patch`.
- Installeren: clone `https://github.com/kevin91nl/codex-ops.git` naar een door gebruiker gekozen map.
- Updaten: in bestaande clone `git pull --ff-only`.
- Bij automation install: kopieer `automations/<name>/prompt.md` naar Codex automation prompt; `automation.toml` is metadata, geen runtime config.
- Houd lokale wijzigingen zichtbaar: check `git status --short` voor pull/push.
