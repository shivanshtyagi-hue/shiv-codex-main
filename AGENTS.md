# Codex Workspace Instructions

Before doing substantial work in this workspace:

1. Read `Shiv/master_agent.md`.
2. Read `context/user_profile.md` and `context/current_priorities.md`.
3. Read the relevant project, workflow, and integration notes.
4. Check the latest relevant file in `sessions/`.

Use this workspace as durable context for Shiv's coworking relationship with Codex. Keep instructions, decisions, and reusable workflows in Markdown files so they can be reused across sessions and the Codex CLI.

When a task changes the workspace, summarize the outcome in a dated session note. Do not store credentials or secrets in this repository.

For Argus work, use only the existing persistent `argus-browser` MCP tools through `http://127.0.0.1:8931/mcp`. Do not use direct Argus REST/API clients, shell HTTP helpers, API-key or Keychain credential handling, token-authentication probes, or natural-language API chat helpers. Do not launch another browser process or modify the MCP endpoint, browser SSO profile, LaunchAgent, or other service configuration. Keep Argus interactions read-only unless the user explicitly authorizes a change.

For session closeout, logging, or handoff requests, use the `$session-log` skill. If the user says “log this session” or “close out this session,” treat that as a request to invoke it.

For OpenAI, Codex, or API questions, consult the official OpenAI documentation when available.
