# Claude setup

_Last updated: 2026-10-09_

## Plugins
- **Engineering**: /debug, /code-review, /architecture, /system-design, /testing-strategy, /tech-debt, /incident-response, /deploy-checklist, /documentation, /standup
- **Project Memory**: /project-memory:remember, /project-memory:recall (local SQLite). This repo is the main, versioned memory store.

## Connectors
- GitHub: **not available.** It isn't in the connector directory, and the plugin's GitHub server can't sign in (its auth server doesn't support dynamic client registration).
  - Workaround: clone repos locally under `D:\Work\zeeshan\` and connect the folder in Cowork.
- Slack, Notion, Linear, Atlassian, Datadog: come with the Engineering plugin but haven't been authorized.

## How to load memory in a new Cowork session
Connect the folder `D:\Work\zeeshan\ai-memory` and say "load my memory". Claude then reads `CLAUDE.md` and `MEMORY.md`.
