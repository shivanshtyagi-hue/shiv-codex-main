# Argus Browser MCP SOP

## Current status

- Access method: existing persistent `argus-browser` MCP tools
- MCP endpoint: `http://127.0.0.1:8931/mcp`
- Browser target: the existing authenticated Argus session

## Operating rules

- Use the existing MCP connection and browser session only.
- Do not launch a second browser process or create a separate Argus session.
- Do not use direct Argus REST/API clients, shell HTTP helpers, API-key or Keychain credential handling, token-authentication probes, or natural-language API chat helpers.
- Do not inspect, export, print, or store credentials, cookies, bearer tokens, or other session secrets.
- Keep interactions read-only unless the user explicitly authorizes a change.
- Do not modify or restart the MCP endpoint, LaunchAgent, Chrome SSO profile, or other services.

## Verification

Read-only availability and authentication checks should use the existing `argus-browser` MCP tools, such as listing the current tab and reading its accessibility snapshot. If another Argus session is active and testing could interfere with it, report the conflict and skip the test.
