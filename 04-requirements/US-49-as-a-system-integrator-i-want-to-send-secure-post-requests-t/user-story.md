# US-49 — As a System Integrator, I want to send secure POST requests to SmartRent API so that door unlock commands are transmitted safely

- **Priority:** high
- **Status:** backlog

## Story

> System compiles verified tenant and device information into secure POST request to SmartRent API endpoint for door unlock.

## Acceptance criteria

- POST request sent to /devices/{deviceId}/unlock endpoint
- Payload includes verified tenant Contact ID and apartment record
- Request uses secure authentication with SmartRent
- System handles API response codes appropriately


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-49]`. Last updated: 2026-06-19T15:25:29.993751+00:00._
