---
name: session-log
description: Create or update a concise dated session handoff for the current Codex session. Use when the user asks to log, summarize, close out, hand off, or record a session.
---

# Session Log

Create or update a Markdown note in the relevant agent or knowledge-base `sessions/` folder using the filename `YYYY-MM-DD-topic.md`. Use `/Users/shivansh.tyagi/Desktop/Shiv-Codex-main/sessions/` for cross-cutting workspace work.

Include only useful durable context:

- objective
- completed work
- decisions and assumptions
- important numbers or evidence
- unresolved questions or blockers
- next actions
- files and tools involved

Do not copy the full conversation, raw command output, credentials, tokens, or private secrets.

The durable agent definition is `Agents/session_logger.md`.

When recording Argus work, refer only to the existing persistent `argus-browser` MCP connection at `http://127.0.0.1:8931/mcp`. Do not record or recommend REST/API clients, HTTP helpers, API keys, Keychain credentials, token probes, or API chat helpers.

If a note for the same date and topic already exists, update it rather than creating a duplicate. Preserve useful existing content and add a short `Updated` line.

After saving, report the exact file path and a three-line summary.
