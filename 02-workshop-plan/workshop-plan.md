# Workshop plan

## Facilitator state

```json
{
  "single_plan": null,
  "series_plan": {
    "series_title": "Agentforce Demo \u2014 Discovery Workshop Series",
    "series_goal": "Understand the use case requirement, understand the technical dependencies",
    "total_sessions": 4,
    "cadence": "Back-to-back days",
    "cadence_rationale": "No discovery duration found in the source documents \u2014 defaulted to 2 sessions/week.",
    "replanning_notes": "",
    "sessions": [
      {
        "session_number": 1,
        "day_label": "Week 1 \u2014 Day 1",
        "title": "Current-state walk-through & pain-point mapping",
        "focus": "Baseline the as-is for the in-scope processes pulled from the SOW.",
        "duration_minutes": 90,
        "format": "hybrid",
        "status": "planned",
        "depends_on": [],
        "attendees": [
          {
            "role": "Solution Architect (you)",
            "why_invite": "Facilitate, capture decisions, drive to closure."
          },
          {
            "role": "Product Owner / Business Lead",
            "why_invite": "Owns prioritization and approval hierarchy."
          },
          {
            "role": "IT / Integration Lead",
            "why_invite": "Commits to integration scope and dates."
          },
          {
            "role": "End-user representatives (2-3)",
            "why_invite": "Validate pain points and to-be flows."
          },
          {
            "role": "Project Sponsor (key sessions only)",
            "why_invite": "Required for scope/exit decisions."
          }
        ],
        "pre_reads": [
          {
            "item": "Latest scope & timeline",
            "source_filename": "Agentforce Pacific Haven Properties .docx",
            "what_to_review": "Confirm in-scope vs out-of-scope before the session."
          }
        ],
        "logical_breakup": [
          {
            "slot_minutes": 5,
            "segment": "Opening, goal, consent",
            "purpose": "Lock the room on the session goal.",
            "facilitator_script": "Our one outcome today: Documented current-state journey for top in-scope processes.",
            "probing_questions": [
              "Any constraints we should know in the next 90 minutes?"
            ],
            "decisions_to_land": [
              "Recording consent obtained."
            ],
            "fallback_if_blocked": "Switch to scribe-only mode."
          },
          {
            "slot_minutes": 25,
            "segment": "Anchor in source documents",
            "purpose": "Use the relevant section of Agentforce Pacific Haven Properties .docx as the spine.",
            "facilitator_script": "I've pulled the section from Agentforce Pacific Haven Properties .docx that drives today's discussion \u2014 play it back to me.",
            "probing_questions": [
              "Where is this still ambiguous?",
              "Who is the named owner for this area?"
            ],
            "decisions_to_land": [
              "Shared understanding of the anchor section confirmed."
            ],
            "fallback_if_blocked": "Capture disagreement as an open question with an owner."
          },
          {
            "slot_minutes": 40,
            "segment": "Working session on focus theme",
            "purpose": "Baseline the as-is for the in-scope processes pulled from the SOW.",
            "facilitator_script": "Time-boxing per item to 5 minutes \u2014 let's drive to a decision or park.",
            "probing_questions": [
              "Who is the business owner of this?",
              "What breaks if we defer to Phase 2?",
              "What's the acceptance test for 'done'?"
            ],
            "decisions_to_land": [
              "Documented current-state journey for top in-scope processes",
              "Top 5 pain points ranked by business impact"
            ],
            "fallback_if_blocked": "Default to 'should' + follow-up with owner."
          },
          {
            "slot_minutes": 15,
            "segment": "Decisions, action items, parking lot",
            "purpose": "Read the decision log back; assign owners + due dates.",
            "facilitator_script": "Before we close, I'm going to read every decision and action \u2014 stop me on anything wrong.",
            "probing_questions": [
              "Any new risk that surfaced today?",
              "Anything we punted that needs a date NOW?"
            ],
            "decisions_to_land": [
              "Every action has owner + due date."
            ],
            "fallback_if_blocked": "Schedule a 15-min async follow-up the same day."
          },
          {
            "slot_minutes": 5,
            "segment": "Close & next session",
            "purpose": "Never leave without scheduling the next session.",
            "facilitator_script": "Next session covers X \u2014 confirm the date now.",
            "probing_questions": [
              "Any blocker before the next session?"
            ],
            "decisions_to_land": [
              "Date & agenda for next session locked."
            ],
            "fallback_if_blocked": "Pick a placeholder slot and confirm via email by EOD."
          }
        ],
        "materials_to_prepare": [
          "Printed extract of the relevant section from Agentforce Pacific Haven Properties .docx",
          "Decision-log template with owner + due-date columns",
          "Parking-lot board (physical or digital)",
          "Pre-printed list of requirement IDs from the source documents"
        ],
        "target_outcomes": [
          "Documented current-state journey for top in-scope processes",
          "Top 5 pain points ranked by business impact",
          "Named owner for each pain area"
        ],
        "success_criteria": [
          "Every target outcome from this session has a named owner.",
          "All decisions captured in the live decision log before close.",
          "No open question leaves the room without an owner and a due date."
        ],
        "actual_outcomes": "",
        "open_questions_after": [
          "Any regulatory / data-residency constraint not covered today"
        ],
        "risks_to_watch": [
          "Source docs may not yet name an owner for every requirement \u2014 surface this early."
        ],
        "post_session_actions": [
          {
            "action": "Publish minutes + decision log",
            "owner": "Solution Architect",
            "due": "within 30 minutes"
          },
          {
            "action": "Update RAID log with new risks/dependencies",
            "owner": "Solution Architect",
            "due": "within 24h"
          }
        ]
      },
      {
        "session_number": 2,
        "day_label": "Week 1 \u2014 Day 2",
        "title": "Must-have requirements lock-in",
        "focus": "Convert SOW/BRD bullets into committed requirements with owners.",
        "duration_minutes": 90,
        "format": "hybrid",
        "status": "planned",
        "depends_on": [
          1
        ],
        "attendees": [
          {
            "role": "Solution Architect (you)",
            "why_invite": "Facilitate, capture decisions, drive to closure."
          },
          {
            "role": "Product Owner / Business Lead",
            "why_invite": "Owns prioritization and approval hierarchy."
          },
          {
            "role": "IT / Integration Lead",
            "why_invite": "Commits to integration scope and dates."
          },
          {
            "role": "End-user representatives (2-3)",
            "why_invite": "Validate pain points and to-be flows."
          },
          {
            "role": "Project Sponsor (key sessions only)",
            "why_invite": "Required for scope/exit decisions."
          }
        ],
        "pre_reads": [
          {
            "item": "Latest scope & timeline",
            "source_filename": "Agentforce Pacific Haven Properties .docx",
            "what_to_review": "Confirm in-scope vs out-of-scope before the session."
          }
        ],
        "logical_breakup": [
          {
            "slot_minutes": 5,
            "segment": "Opening, goal, consent",
            "purpose": "Lock the room on the session goal.",
            "facilitator_script": "Our one outcome today: Every must-have requirement has a named business owner.",
            "probing_questions": [
              "Any constraints we should know in the next 90 minutes?"
            ],
            "decisions_to_land": [
              "Recording consent obtained."
            ],
            "fallback_if_blocked": "Switch to scribe-only mode."
          },
          {
            "slot_minutes": 25,
            "segment": "Anchor in source documents",
            "purpose": "Use the relevant section of Agentforce Pacific Haven Properties .docx as the spine.",
            "facilitator_script": "I've pulled the section from Agentforce Pacific Haven Properties .docx that drives today's discussion \u2014 play it back to me.",
            "probing_questions": [
              "Where is this still ambiguous?",
              "Who is the named owner for this area?"
            ],
            "decisions_to_land": [
              "Shared understanding of the anchor section confirmed."
            ],
            "fallback_if_blocked": "Capture disagreement as an open question with an owner."
          },
          {
            "slot_minutes": 40,
            "segment": "Working session on focus theme",
            "purpose": "Convert SOW/BRD bullets into committed requirements with owners.",
            "facilitator_script": "Time-boxing per item to 5 minutes \u2014 let's drive to a decision or park.",
            "probing_questions": [
              "Who is the business owner of this?",
              "What breaks if we defer to Phase 2?",
              "What's the acceptance test for 'done'?"
            ],
            "decisions_to_land": [
              "Every must-have requirement has a named business owner",
              "Sprint/phase target locked for every must-have"
            ],
            "fallback_if_blocked": "Default to 'should' + follow-up with owner."
          },
          {
            "slot_minutes": 15,
            "segment": "Decisions, action items, parking lot",
            "purpose": "Read the decision log back; assign owners + due dates.",
            "facilitator_script": "Before we close, I'm going to read every decision and action \u2014 stop me on anything wrong.",
            "probing_questions": [
              "Any new risk that surfaced today?",
              "Anything we punted that needs a date NOW?"
            ],
            "decisions_to_land": [
              "Every action has owner + due date."
            ],
            "fallback_if_blocked": "Schedule a 15-min async follow-up the same day."
          },
          {
            "slot_minutes": 5,
            "segment": "Close & next session",
            "purpose": "Never leave without scheduling the next session.",
            "facilitator_script": "Next session covers X \u2014 confirm the date now.",
            "probing_questions": [
              "Any blocker before the next session?"
            ],
            "decisions_to_land": [
              "Date & agenda for next session locked."
            ],
            "fallback_if_blocked": "Pick a placeholder slot and confirm via email by EOD."
          }
        ],
        "materials_to_prepare": [
          "Printed extract of the relevant section from Agentforce Pacific Haven Properties .docx",
          "Decision-log template with owner + due-date columns",
          "Parking-lot board (physical or digital)",
          "Pre-printed list of requirement IDs from the source documents"
        ],
        "target_outcomes": [
          "Every must-have requirement has a named business owner",
          "Sprint/phase target locked for every must-have",
          "Parking lot captured for 'should/could' items"
        ],
        "success_criteria": [
          "Every target outcome from this session has a named owner.",
          "All decisions captured in the live decision log before close.",
          "No open question leaves the room without an owner and a due date."
        ],
        "actual_outcomes": "",
        "open_questions_after": [
          "Any regulatory / data-residency constraint not covered today"
        ],
        "risks_to_watch": [
          "Source docs may not yet name an owner for every requirement \u2014 surface this early."
        ],
        "post_session_actions": [
          {
            "action": "Publish minutes + decision log",
            "owner": "Solution Architect",
            "due": "within 30 minutes"
          },
          {
            "action": "Update RAID log with new risks/dependencies",
            "owner": "Solution Architect",
            "due": "within 24h"
          }
        ]
      },
      {
        "session_number": 3,
        "day_label": "Week 1 \u2014 Day 3",
        "title": "Integration & data dependency mapping",
        "focus": "Make the integration map real with owners and dates.",
        "duration_minutes": 90,
        "format": "hybrid",
        "status": "planned",
        "depends_on": [
          1,
          2
        ],
        "attendees": [
          {
            "role": "Solution Architect (you)",
            "why_invite": "Facilitate, capture decisions, drive to closure."
          },
          {
            "role": "Product Owner / Business Lead",
            "why_invite": "Owns prioritization and approval hierarchy."
          },
          {
            "role": "IT / Integration Lead",
            "why_invite": "Commits to integration scope and dates."
          },
          {
            "role": "End-user representatives (2-3)",
            "why_invite": "Validate pain points and to-be flows."
          },
          {
            "role": "Project Sponsor (key sessions only)",
            "why_invite": "Required for scope/exit decisions."
          }
        ],
        "pre_reads": [
          {
            "item": "Latest scope & timeline",
            "source_filename": "Agentforce Pacific Haven Properties .docx",
            "what_to_review": "Confirm in-scope vs out-of-scope before the session."
          }
        ],
        "logical_breakup": [
          {
            "slot_minutes": 5,
            "segment": "Opening, goal, consent",
            "purpose": "Lock the room on the session goal.",
            "facilitator_script": "Our one outcome today: Each integration has an owner and an ETA for API spec hand-off.",
            "probing_questions": [
              "Any constraints we should know in the next 90 minutes?"
            ],
            "decisions_to_land": [
              "Recording consent obtained."
            ],
            "fallback_if_blocked": "Switch to scribe-only mode."
          },
          {
            "slot_minutes": 25,
            "segment": "Anchor in source documents",
            "purpose": "Use the relevant section of Agentforce Pacific Haven Properties .docx as the spine.",
            "facilitator_script": "I've pulled the section from Agentforce Pacific Haven Properties .docx that drives today's discussion \u2014 play it back to me.",
            "probing_questions": [
              "Where is this still ambiguous?",
              "Who is the named owner for this area?"
            ],
            "decisions_to_land": [
              "Shared understanding of the anchor section confirmed."
            ],
            "fallback_if_blocked": "Capture disagreement as an open question with an owner."
          },
          {
            "slot_minutes": 40,
            "segment": "Working session on focus theme",
            "purpose": "Make the integration map real with owners and dates.",
            "facilitator_script": "Time-boxing per item to 5 minutes \u2014 let's drive to a decision or park.",
            "probing_questions": [
              "Who is the business owner of this?",
              "What breaks if we defer to Phase 2?",
              "What's the acceptance test for 'done'?"
            ],
            "decisions_to_land": [
              "Each integration has an owner and an ETA for API spec hand-off",
              "Test data ownership confirmed per integration"
            ],
            "fallback_if_blocked": "Default to 'should' + follow-up with owner."
          },
          {
            "slot_minutes": 15,
            "segment": "Decisions, action items, parking lot",
            "purpose": "Read the decision log back; assign owners + due dates.",
            "facilitator_script": "Before we close, I'm going to read every decision and action \u2014 stop me on anything wrong.",
            "probing_questions": [
              "Any new risk that surfaced today?",
              "Anything we punted that needs a date NOW?"
            ],
            "decisions_to_land": [
              "Every action has owner + due date."
            ],
            "fallback_if_blocked": "Schedule a 15-min async follow-up the same day."
          },
          {
            "slot_minutes": 5,
            "segment": "Close & next session",
            "purpose": "Never leave without scheduling the next session.",
            "facilitator_script": "Next session covers X \u2014 confirm the date now.",
            "probing_questions": [
              "Any blocker before the next session?"
            ],
            "decisions_to_land": [
              "Date & agenda for next session locked."
            ],
            "fallback_if_blocked": "Pick a placeholder slot and confirm via email by EOD."
          }
        ],
        "materials_to_prepare": [
          "Printed extract of the relevant section from Agentforce Pacific Haven Properties .docx",
          "Decision-log template with owner + due-date columns",
          "Parking-lot board (physical or digital)",
          "Pre-printed list of requirement IDs from the source documents"
        ],
        "target_outcomes": [
          "Each integration has an owner and an ETA for API spec hand-off",
          "Test data ownership confirmed per integration",
          "Failure-mode contingency captured per integration"
        ],
        "success_criteria": [
          "Every target outcome from this session has a named owner.",
          "All decisions captured in the live decision log before close.",
          "No open question leaves the room without an owner and a due date."
        ],
        "actual_outcomes": "",
        "open_questions_after": [
          "Any regulatory / data-residency constraint not covered today"
        ],
        "risks_to_watch": [
          "Source docs may not yet name an owner for every requirement \u2014 surface this early."
        ],
        "post_session_actions": [
          {
            "action": "Publish minutes + decision log",
            "owner": "Solution Architect",
            "due": "within 30 minutes"
          },
          {
            "action": "Update RAID log with new risks/dependencies",
            "owner": "Solution Architect",
            "due": "within 24h"
          }
        ]
      },
      {
        "session_number": 4,
        "day_label": "Week 1 \u2014 Day 4",
        "title": "Persona deep-dive & to-be journey design",
        "focus": "Validate to-be flows with end-user representatives.",
        "duration_minutes": 90,
        "format": "hybrid",
        "status": "planned",
        "depends_on": [
          1,
          2,
          3
        ],
        "attendees": [
          {
            "role": "Solution Architect (you)",
            "why_invite": "Facilitate, capture decisions, drive to closure."
          },
          {
            "role": "Product Owner / Business Lead",
            "why_invite": "Owns prioritization and approval hierarchy."
          },
          {
            "role": "IT / Integration Lead",
            "why_invite": "Commits to integration scope and dates."
          },
          {
            "role": "End-user representatives (2-3)",
            "why_invite": "Validate pain points and to-be flows."
          },
          {
            "role": "Project Sponsor (key sessions only)",
            "why_invite": "Required for scope/exit decisions."
          }
        ],
        "pre_reads": [
          {
            "item": "Latest scope & timeline",
            "source_filename": "Agentforce Pacific Haven Properties .docx",
            "what_to_review": "Confirm in-scope vs out-of-scope before the session."
          }
        ],
        "logical_breakup": [
          {
            "slot_minutes": 5,
            "segment": "Opening, goal, consent",
            "purpose": "Lock the room on the session goal.",
            "facilitator_script": "Our one outcome today: Validated to-be journeys for each primary persona.",
            "probing_questions": [
              "Any constraints we should know in the next 90 minutes?"
            ],
            "decisions_to_land": [
              "Recording consent obtained."
            ],
            "fallback_if_blocked": "Switch to scribe-only mode."
          },
          {
            "slot_minutes": 25,
            "segment": "Anchor in source documents",
            "purpose": "Use the relevant section of Agentforce Pacific Haven Properties .docx as the spine.",
            "facilitator_script": "I've pulled the section from Agentforce Pacific Haven Properties .docx that drives today's discussion \u2014 play it back to me.",
            "probing_questions": [
              "Where is this still ambiguous?",
              "Who is the named owner for this area?"
            ],
            "decisions_to_land": [
              "Shared understanding of the anchor section confirmed."
            ],
            "fallback_if_blocked": "Capture disagreement as an open question with an owner."
          },
          {
            "slot_minutes": 40,
            "segment": "Working session on focus theme",
            "purpose": "Validate to-be flows with end-user representatives.",
            "facilitator_script": "Time-boxing per item to 5 minutes \u2014 let's drive to a decision or park.",
            "probing_questions": [
              "Who is the business owner of this?",
              "What breaks if we defer to Phase 2?",
              "What's the acceptance test for 'done'?"
            ],
            "decisions_to_land": [
              "Validated to-be journeys for each primary persona",
              "Acceptance criteria drafted for top 5 user stories"
            ],
            "fallback_if_blocked": "Default to 'should' + follow-up with owner."
          },
          {
            "slot_minutes": 15,
            "segment": "Decisions, action items, parking lot",
            "purpose": "Read the decision log back; assign owners + due dates.",
            "facilitator_script": "Before we close, I'm going to read every decision and action \u2014 stop me on anything wrong.",
            "probing_questions": [
              "Any new risk that surfaced today?",
              "Anything we punted that needs a date NOW?"
            ],
            "decisions_to_land": [
              "Every action has owner + due date."
            ],
            "fallback_if_blocked": "Schedule a 15-min async follow-up the same day."
          },
          {
            "slot_minutes": 5,
            "segment": "Close & next session",
            "purpose": "Never leave without scheduling the next session.",
            "facilitator_script": "Next session covers X \u2014 confirm the date now.",
            "probing_questions": [
              "Any blocker before the next session?"
            ],
            "decisions_to_land": [
              "Date & agenda for next session locked."
            ],
            "fallback_if_blocked": "Pick a placeholder slot and confirm via email by EOD."
          }
        ],
        "materials_to_prepare": [
          "Printed extract of the relevant section from Agentforce Pacific Haven Properties .docx",
          "Decision-log template with owner + due-date columns",
          "Parking-lot board (physical or digital)",
          "Pre-printed list of requirement IDs from the source documents"
        ],
        "target_outcomes": [
          "Validated to-be journeys for each primary persona",
          "Acceptance criteria drafted for top 5 user stories",
          "UX/UI constraints captured"
        ],
        "success_criteria": [
          "Every target outcome from this session has a named owner.",
          "All decisions captured in the live decision log before close.",
          "No open question leaves the room without an owner and a due date."
        ],
        "actual_outcomes": "",
        "open_questions_after": [
          "Any regulatory / data-residency constraint not covered today"
        ],
        "risks_to_watch": [
          "Source docs may not yet name an owner for every requirement \u2014 surface this early."
        ],
        "post_session_actions": [
          {
            "action": "Publish minutes + decision log",
            "owner": "Solution Architect",
            "due": "within 30 minutes"
          },
          {
            "action": "Update RAID log with new risks/dependencies",
            "owner": "Solution Architect",
            "due": "within 24h"
          }
        ]
      }
    ],
    "series_exit_criteria": [
      "All must-have requirements have a named owner and target sprint.",
      "Every integration has a committed date for API spec delivery.",
      "BRD signed off by sponsor and PO.",
      "Discovery RAID log is current with mitigations assigned."
    ],
    "sources_used": [
      {
        "filename": "Agentforce Pacific Haven Properties .docx",
        "doc_type": "sow",
        "how_it_shaped_the_plan": "Anchored session content in Agentforce Pacific Haven Properties .docx."
      }
    ]
  },
  "previous_plan": null,
  "selected_filenames": [
    "Agentforce Pacific Haven Properties .docx"
  ],
  "goal": "Understand the use case requirement, understand the technical dependencies",
  "session_count_override": null,
  "completed_feedback": {},
  "sources": [
    {
      "filename": "Agentforce Pacific Haven Properties .docx",
      "doc_type": "sow",
      "doc_label": "Statement of Work"
    }
  ],
  "discovery_duration": {
    "source": "default"
  },
  "recommended_session_count": 4,
  "effective_session_count": 4,
  "edit_log": [
    {
      "at": "2026-06-19T07:32:10.815476+00:00",
      "kind": "regenerate",
      "summary": "Regenerated workshop series from 1 source document(s)"
    }
  ],
  "updated_at": "2026-06-19T07:32:10.815476+00:00"
}
```

---
_Auto-generated from in-app state. Source field: `pipeline_artifacts.workshop_output + workshop_state`. Last updated: 2026-06-24T05:38:04.181614+00:00._
