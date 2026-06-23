# LA-04 — Building Policy Validation (RAG)

- **Priority:** medium
- **Status:** backlog
- **Epic:** Leasing Assistant

## Story

> As a prospective tenant, I want to ask unstructured questions about complex building policies (e.g., guest limits, pet sizes, bicycle storage), so that I can determine if the community suits my constraints.

## Acceptance criteria

- Agent invokes a RAG action pointing to the Tenant Handbook index.
- Answers match accurate policies (e.g., 50 lb Labrador restrictions in SF, bicycle storage in Portland).
- Responses omit hallucinated clauses and ground answers completely within the source document context.


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[LA-04]`. Last updated: 2026-06-23T08:00:00.911849+00:00._
