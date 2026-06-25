# US-10 — No Double-Lookup (Apartment ID vs Name)

- **Priority:** medium
- **Status:** backlog
- **Epic:** Pricing & Discount Guardrail

## Story

> As a leasing manager, I want the agent to use either the apartment ID or the apartment name — never both together, so that discount lookups are unambiguous and return accurate results.

## Acceptance criteria

- If an apartment ID is already known from a prior search, it is used directly
- Apartment name is only used when no ID is available
- Both are never sent together in the same request


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-10]`. Last updated: 2026-06-25T11:27:47.831529+00:00._
