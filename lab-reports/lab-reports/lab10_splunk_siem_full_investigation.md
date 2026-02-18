# Lab 10 — Splunk SIEM VPN Log Investigation

## Objective
To understand Splunk SIEM fundamentals including data ingestion, index creation, log searching, and basic investigation queries using VPN log datasets.

## Platform
- TryHackMe — Splunk: The Basics
- Splunk Enterprise (Lab Instance)
- AttackBox VM

## Skills Practiced
- SIEM navigation
- Data ingestion into Splunk
- Creating custom index
- Log search queries
- Field filtering
- IP investigation
- Username correlation
- Country-based filtering
- Event counting

---

## Lab Setup

1. Launched TryHackMe Splunk lab environment.
2. Accessed Splunk Enterprise through provided AttackBox browser.
3. Navigated to **Add Data** section.
4. Uploaded dataset: `VPNlogs.json`.
5. Created new index:VPN_Logs

---

## Data Ingestion Steps

- Selected file upload source.
- Chose JSON format.
- Assigned index = `VPN_Logs`.
- Verified ingestion completed successfully.
- Confirmed logs visible in Splunk search interface.

---

## Investigation Queries Performed

### 1 Total Events in Log File

Query:index=VPN_Logs
Result:2862 events

---

### 2️ Events by Specific User

Query: index=VPN_Logs UserName=Maleena
Result:60 events

---

### 3️ Username Associated with IP

Query:index=VPN_Logs source_ip=107.14.182.38
Result:User name: Smith

---

### 4️ Events from All Countries Except France

Query:index=VPN_Logs NOT Source_Country=France
Result:2814 events


---

### 5️ Events from Specific IP

Query: index=VPN_Logs source_ip=107.3.206.58
Result: 14 events


---

## Key SIEM Concepts Learned

- Splunk components: Forwarder, Indexer, Search Head
- Index-based log organization
- Field extraction from JSON logs
- Filtering by:
  - IP address
  - Username
  - Country
  - Event fields
- Event counting & correlation
- Basic SOC investigation workflow

---

## SOC Analyst Relevance

This lab simulates real SOC L1 responsibilities:

- Log ingestion
- Query-based alert investigation
- User activity tracking
- IP reputation checks
- Event filtering & triage
- SIEM dashboard usage

---

## Evidence

Screenshots stored in: screenshort folder 


Includes:
- Data upload screen
- Index creation
- Search queries
- Result validation
- Event details view

---

## Outcome

Successfully completed Splunk SIEM lab and performed structured log investigations using indexed VPN data. Built practical understanding of SIEM search and SOC investigation workflow.









   
6. Created new index:
index=VPN_Logs
