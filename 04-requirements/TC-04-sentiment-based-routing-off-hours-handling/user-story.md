# TC-04 — Sentiment-Based Routing & Off-Hours Handling

- **Priority:** medium
- **Status:** backlog
- **Epic:** Tenant Concierge

## Story

> As an authenticated tenant displaying high frustration, I want the agent to recognize my negative sentiment and smoothly adjust routing behaviors depending on current staffing hours.

## Acceptance criteria

- Agent parses angry text strings (e.g., "leaking for the third time, fix this now or else").
- Agent returns a supportive, empathetic validation response.
- During standard shift hours, it schedules an instant live agent handoff.
- At off-hours (e.g., 2 AM), it logs the case securely with an elevated visibility tag and explicitly informs the user that a supervisor will review it first thing in the morning.


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[TC-04]`. Last updated: 2026-06-24T05:38:04.182878+00:00._
