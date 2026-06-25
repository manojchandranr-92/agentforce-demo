# US-09 — Move-in Special Lookup

- **Priority:** high
- **Status:** backlog
- **Epic:** Pricing & Discount Guardrail

## Story

> As a prospective tenant, I want to ask if there are any discounts or move-in specials for an apartment, so that I can make an informed decision about which unit to rent.

## Acceptance criteria

- Agent is triggered by any of: discount request, negotiation attempt, price comparison, request for offers/specials/deals
- Agent collects: Apartment name or ID, city (if no ID), bedrooms (optional), move-in month (optional, defaults to current month)
- Response format always includes: Base Rent, Applicable Move-in Special (if any), Final Effective Rent, Offer Validity


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-09]`. Last updated: 2026-06-25T11:27:47.831237+00:00._
