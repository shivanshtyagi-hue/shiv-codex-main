# Agent and Knowledge Base Organization — 2026-10-22

## Objective

Create a durable structure for agent definitions, knowledge domains, and agent/domain-specific session logging.

## Completed

- Added `Agents/` with definitions for the session logger, Data Alerter, Experiment Data Analyser, Exploratory Analyst, Jira Agent, and Confluence Agent.
- Added local `sessions/` folders for each agent.
- Added `Knowledge Base/Argus/` and `Knowledge Base/Data Sources/`, each with a local `sessions/` folder.
- Updated workspace maps and the session-log skill to route notes to the relevant local session folder.
- Preserved `.agents/skills/session-log/SKILL.md` as the Codex invocation layer and made `Agents/session_logger.md` the durable agent contract.

## Next actions

- Populate the agent definitions with tool-specific workflows and examples as each agent is used.
- Add verified Argus concepts and data-source references to the Knowledge Base.
