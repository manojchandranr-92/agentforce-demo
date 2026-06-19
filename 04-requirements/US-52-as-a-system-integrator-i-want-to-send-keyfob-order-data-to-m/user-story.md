# US-52 — As a System Integrator, I want to send keyfob order data to MuleSoft API so that approved orders are processed

- **Priority:** medium
- **Status:** backlog

## Story

> When tenant approves keyfob order, system sends POST request to MuleSoft experience/process API with order payload.

## Acceptance criteria

- POST request sent to MuleSoft experience/process API
- Payload includes status: approved, fobType: Standard, quantity: 1
- Request is triggered only after tenant approval
- API call includes proper authentication and headers


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-52]`. Last updated: 2026-06-19T15:25:29.994192+00:00._
