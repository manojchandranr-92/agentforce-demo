# TC-06 — Keyfob Replacement & Provisioning Integration

- **Priority:** medium
- **Status:** backlog
- **Epic:** Tenant Concierge

## Story

> As an authenticated tenant, I want to inquire about keyfob replacements, review pricing, and place an order seamlessly in the interface, so that an order is created automatically in the provisioning system.

## Acceptance criteria

- Agent queries the Tenant Handbook vector index to pull and present the accurate keyfob replacement cost.
- If the user clicks "OK/Approve" or indicates intent to purchase, the application fires a structured JSON payload to the MuleSoft experience layer.
- MuleSoft processes transformations and verifies a successful mock return code (201 Created) containing a SmartRent Order ID back to the user chat UI.


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[TC-06]`. Last updated: 2026-06-24T05:42:48.518898+00:00._
