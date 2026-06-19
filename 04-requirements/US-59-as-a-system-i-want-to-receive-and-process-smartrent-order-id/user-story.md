# US-59 — As a System, I want to receive and process SmartRent Order ID from successful submissions so that I can track order status

- **Priority:** high
- **Status:** backlog

## Story

> When SmartRent accepts an order, the system must capture and store the returned Order ID for tracking purposes.

## Acceptance criteria

- System receives 201 Created status from SmartRent API
- SmartRent Order ID is extracted from response
- Order ID is stored in system for future reference
- Success status is logged and communicated


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-59]`. Last updated: 2026-06-19T15:25:29.995225+00:00._
