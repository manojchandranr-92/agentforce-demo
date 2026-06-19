# US-42 — As a Property Agent, I want to verify tenant status before processing maintenance requests so that only active tenants can create issues

- **Priority:** high
- **Status:** backlog

## Story

> System must validate that the logged-in user is an active tenant before allowing them to initiate maintenance actions.

## Acceptance criteria

- Agent verifies user has active tenant status
- System blocks maintenance actions for inactive tenants
- Verification occurs before any maintenance workflow begins
- Clear error message displayed for inactive tenants


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-42]`. Last updated: 2026-06-19T15:25:29.992706+00:00._
