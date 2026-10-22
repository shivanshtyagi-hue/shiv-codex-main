# Personal Commands

Codex does not require a custom shell command for every workflow. Use these layers:

## Always-on behavior

Put rules that should apply to every task in the workspace `AGENTS.md`.

## Reusable command-like workflows

Put repeatable workflows in `.agents/skills/<skill-name>/SKILL.md`. Invoke one directly with its `$skill-name` form, or use `/skills` to inspect available skills in the interactive CLI.

Current workflow:

- `$session-log` — create or update a concise dated session handoff

## Shell shortcuts

Use a shell alias or function only for convenience, such as launching Codex in this workspace. Keep the actual behavior in `AGENTS.md` or a Skill so it remains visible, reviewable, and versionable.
