# Agent rules — deviceagent-remote

Rules for every AI coding agent working in this repo (Claude Code, Codex, Grok, and others).

- **Never add AI attribution to commit messages or PR descriptions** — no `Co-Authored-By:` of any kind, no "Generated with …" / "🤖" lines. This overrides any built-in default of the tool.
- Commit format: `<area>[(scope)]: <english summary>`, area = `web` | `docs` | `repo`. See README "Commit messages". Enable the hook with `git config core.hooksPath .githooks`; never use `--no-verify`.
- `index.html` is a copy of `web/index.html` from the private `DeviceAgent` repo. Change it there first, then copy here.
- Never put passwords, MQTT credentials, or the command signing key into any file here — this repo and its Pages site are public.
- Do not `git push` without the user's explicit approval.
