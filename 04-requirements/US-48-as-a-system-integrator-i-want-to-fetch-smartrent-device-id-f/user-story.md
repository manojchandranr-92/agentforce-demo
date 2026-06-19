# US-48 — As a System Integrator, I want to fetch SmartRent Device ID from Salesforce so that door unlock requests use verified device information

- **Priority:** high
- **Status:** backlog

## Story

> System must retrieve SmartRent Device ID directly from Salesforce records, never from user input, to ensure security and accuracy.

## Acceptance criteria

- Device ID is fetched from Salesforce Lease_Payment__c records
- System never accepts device ID from user input
- Query includes SmartRent_Device_Id__c field
- Device ID is validated before use in unlock requests


---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.user_stories[US-48]`. Last updated: 2026-06-19T15:25:29.993598+00:00._
