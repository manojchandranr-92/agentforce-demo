# US-41 — As a Guest User, I want to be prompted to login when requesting maintenance so that the system can verify my identity

- **Priority:** high
- **Status:** backlog

## Story

> When a guest user attempts to report maintenance issues, the agent should detect they are not logged in and politely request authentication.

## Acceptance criteria

- Agent detects when user is not authenticated
- System prevents maintenance actions for unauthenticated users
- User receives polite prompt to login before continuing
- No maintenance actions are executed without proper authentication


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-41]`. Last updated: 2026-06-19T15:25:29.992554+00:00._
