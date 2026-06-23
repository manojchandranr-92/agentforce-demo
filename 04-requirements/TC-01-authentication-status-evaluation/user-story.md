# TC-01 — Authentication Status Evaluation

- **Priority:** high
- **Status:** backlog
- **Epic:** Tenant Concierge

## Story

> As a resident platform administrator, I want the chat session to accurately evaluate authentication status, so that guest accounts are blocked from accessing operational internal tenant workflows.

## Acceptance criteria

- System reads global profile variables ($User.Id).
- If session is guest/unauthenticated, agent stops execution and politely prompts user to log into their tenant portal.
- If authenticated, agent confirms active tenancy before executing subsequent service tasks.


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[TC-01]`. Last updated: 2026-06-23T08:00:00.912250+00:00._
