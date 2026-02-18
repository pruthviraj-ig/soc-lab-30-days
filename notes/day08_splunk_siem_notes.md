# Day 08 — Splunk SIEM Basics & Log Investigation Notes

## SIEM Overview

SIEM = Security Information and Event Management

Purpose:
- Collect logs from multiple sources
- Normalize and index data
- Enable fast searching and investigation
- Detect suspicious activity
- Support SOC alert triage and investigations

Common SIEM Use Cases:
- Log monitoring
- Alert investigation
- User activity tracking
- IP investigation
- Threat detection
- Incident response support

---

## Splunk Overview

Splunk is a SIEM and log analytics platform used by SOC teams to:

- Collect logs
- Index events
- Search and filter data
- Build dashboards
- Investigate incidents
- Correlate activity

Splunk works on indexed machine data and allows fast search using SPL (Search Processing Language).

---

## Splunk Core Components

### Forwarder
- Installed on endpoints
- Collects logs
- Sends logs to indexer
- Lightweight agent
- Minimal system impact

### Indexer
- Receives log data
- Parses and indexes events
- Stores searchable data
- Makes logs queryable

### Search Head
- Analyst interface
- Runs searches and queries
- Displays dashboards
- Used for investigations

---

## Splunk Interface Areas

### Search & Reporting App
Main SOC analyst workspace.

Used for:
- Running queries
- Filtering events
- Viewing fields
- Building investigations

### Splunk Bar (Top Menu)
Contains:
- Messages
- Settings
- Activity
- Help
- App navigation

---

## Splunk Data Ingestion Process

Steps:

1. Go to **Add Data**
2. Choose data source method
3. Upload or monitor data
4. Select source type
5. Define index
6. Review settings
7. Submit ingestion

After ingestion:
- Data is parsed
- Events are created
- Fields are extracted
- Events become searchable

---

## Source Types

Source type tells Splunk how to interpret logs.

Examples:
- json
- syslog
- apache
- windows_event_log

Correct source type improves field extraction.

---

## Index Concept

Index = logical storage container for logs.

Examples:
- default
- security
- vpn_logs (custom)

Why indexes matter:
- Faster searching
- Better organization
- Scoped investigations
- SOC separation of log types

---

## Lab — VPN Log Dataset
Dataset:
VPNlogs.json

Custom Index Created:
VPN_Logs

Source Type:
json

---

## Important Log Fields Observed

From VPN dataset:

- EventTime
- Source_ip
- Source_Country
- UserName
- action
- protocol
- port
- source_state
- Company

These fields allow:

- IP tracking
- User tracking
- Country filtering
- Event counting
- Activity correlation

---

## Splunk Search Basics (SPL)

### Search by Index

index=VPN_Logs

Returns all events in index.

---
### Search by User
index=VPN_Logs UserName=Maleena

Used for user activity investigation.

---

### Search by IP

index=VPN_Logs source_ip=107.x.x.x

Used for IP reputation investigation.

---

### Exclude Condition

index=VPN_Logs NOT Source_Country=France


Used to filter out specific values.

---

### Count Events


Dataset: index=VPN_Logs | stats count


Used to get total event numbers.

---

## Investigation Skills Practiced Today

SOC L1 relevant skills:

- SIEM navigation
- Log ingestion workflow
- Index creation
- JSON log parsing
- Field-based filtering
- IP investigation
- User investigation
- Event counting
- Query refinement
- Evidence validation

---

## SOC Workflow Mapping

Today’s lab maps to real SOC tasks:

Data Received → Indexed → Queried → Filtered → Investigated → Answered

Equivalent SOC tasks:

- Alert log review
- User activity lookup
- Suspicious IP investigation
- Event correlation
- Evidence extraction

---

## Key Takeaways

- Splunk indexes logs into searchable events
- Source type controls field extraction
- Index design improves investigation speed
- SPL queries are core SOC skill
- Field filtering is primary investigation method
- SIEM investigation is query-driven
- Structured logs make faster analysis possible

---

## Next Skills to Practice

- SPL advanced queries
- Time-range filtering
- stats / chart commands
- Dashboards
- Alert rules
- Detection queries
- MITRE mapping with logs

