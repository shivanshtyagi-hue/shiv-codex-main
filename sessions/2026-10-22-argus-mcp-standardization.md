# Argus MCP Standardization — 2026-10-22

## Objective

Standardize Argus access on the existing persistent `argus-browser` MCP connection at `http://127.0.0.1:8931/mcp`.

## Completed

- Audited the workspace for Argus REST/API clients, HTTP helpers, credential handling, auth probes, API chat helpers, and related instructions.
- Removed the isolated legacy Argus API helper scripts and Keychain-based access note.
- Updated workspace, master-agent, and session-log instructions to require MCP-only Argus access.
- Added `SOP/Argus/README.md` with the operating and verification rules.
- Verified the existing MCP connection using read-only tab listing and accessibility snapshot.

## Decisions and safety

- No Keychain credentials or secrets were inspected, deleted, or modified.
- No browser process, tab, LaunchAgent, MCP endpoint, SSO profile, or service configuration was changed.
- The existing Argus tab was left untouched after read-only verification.

## Remaining

- The unrelated Codex CLI integration note still contains an older workspace path; it was left unchanged because it is outside this Argus standardization.
- No Argus-specific API references remain apart from the new policy documentation.
