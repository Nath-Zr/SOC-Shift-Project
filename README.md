# Work a Real SOC Shift in ServiceNow

A self-contained SOC Analyst portfolio project: triaging a real ticket queue in
ServiceNow, investigating sign-in log evidence, reaching a defensible verdict,
and writing up the ticket the way a reviewer would want to read it.

**Role simulated:** SOC Analyst
**Tools used:** ServiceNow, sign-in log analysis (Entra ID schema), MITRE ATT&CK

## The Scenario

An automated alert flags an "impossible travel" sign-in for user `j.rivera` —
two successful logins from geographically distant locations, minutes apart.
The ticket had to be triaged, investigated against real sign-in evidence, and
resolved with a documented, defensible conclusion.

## Walkthrough

| Step | Screenshot |
|---|---|
| 1. Ticket created and scoped | `01-ticket-created.png` |
| 2. Triaged — urgency escalated, marked In Progress | `02-triage-escalated.png` |
| 3. Evidence — the two flagged sign-in events | `03-evidence-filtered.png` |
| 4. Full sign-in log — the anomaly found in a real 32-event haystack | `04-full-log-haystack.png` |
| 5. Final write-up — reasoning, MITRE ATT&CK mapping, and hold status | `05-writeup-worknotes.png` |

## Files

- `signin_logs_2026-09-08.csv` — the full sign-in log dataset investigated in this project
- `SOC_Shift_SN_Project_Guide.docx` — a complete step-by-step guide to rebuilding this project, including every roadblock hit along the way and how each was resolved

## What This Demonstrates

- Working a real ticket queue — triaging, prioritizing, and moving a ticket through its full lifecycle
- Reading an alert before reacting — pulling actual evidence and calculating facts rather than assuming
- Reaching a defensible verdict — ruling out innocent explanations before concluding compromise
- Writing a ticket a reviewer can actually follow — with an industry-standard MITRE ATT&CK classification
