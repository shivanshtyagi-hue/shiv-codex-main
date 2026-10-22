# Session Logger Agent

## Purpose

Capture concise, durable handoffs for agent work without copying full conversations or recording credentials.

## Rules

- Log each agent's work in that agent's local `sessions/` folder.
- Keep cross-cutting workspace changes in the top-level `sessions/` folder.
- Include objective, completed work, decisions, evidence, unresolved questions, next actions, and important files.
- Never record tokens, passwords, cookies, API keys, or private credentials.
- Update an existing same-topic note instead of creating a duplicate.

## File naming

Use `YYYY-MM-DD-topic.md`.

## Existing implementation

The Codex-invokable implementation remains at `.agents/skills/session-log/SKILL.md`; this file is the durable agent definition and operating contract.
