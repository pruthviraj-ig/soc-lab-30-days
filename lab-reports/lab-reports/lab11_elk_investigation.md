# Lab 10 — Elastic Stack (ELK) Log Investigation & Dashboard Analysis

Platform: TryHackMe  
Room: Investigating with ELK (Elastic Stack)  
Role Simulation: SOC Analyst Level 1 (Log Investigation & Threat Analysis)

---

## Objective

Understand how SOC analysts use the Elastic Stack (ELK) to perform log ingestion, searching, filtering, investigation, visualization creation, and dashboard monitoring for detecting suspicious VPN activity.

---

## Technologies Used

- Elasticsearch
- Kibana Discover
- KQL (Kibana Query Language)
- Elastic Visualizations
- Elastic Dashboards
- VPN Log Dataset Investigation

---

## Key ELK Components Reviewed

- Elasticsearch — Data storage and indexing engine
- Logstash — Log parsing and processing pipeline
- Kibana — Visualization and investigation interface

---

## Tasks Completed

### Task 1 — Introduction

- Reviewed ELK stack capabilities within SOC environments
- Understood how ELK functions as a SIEM-like solution
- Learned log collection and investigation workflow

---

### Task 2 — Elastic Stack Overview

- Studied ELK architecture and SOC analyst workflow
- Learned indexing and log searching concepts

---

### Task 3 — Lab Connection

- Connected to AttackBox investigation environment
- Accessed Kibana interface via browser

---

### Task 4 — Discover Tab Investigation

Performed log analysis using the Discover tab:

Actions performed:

- Selected dataset index `vpn_connections`
- Applied time filters for investigation scope
- Expl​​ored available log fields:

  - Source IP
  - Username
  - Country
  - Source State
  - Timestamp

Activities:

- Reviewed log timelines
- Identified spikes in VPN activity
- Investigated suspicious access patterns

---

### Investigation Results — Discover Tab

Findings:

- Hits between Dec 31 2021 — Feb 02 2022:

2861 Events

- IP with Maximum Connections:

238.163.231.224

- User Responsible for Maximum Traffic:

James

- Username Filter Applied:

UserName: Emanda

Source IP with Maximum Hits:

107.14.1.247

- Spike Observed:

11 January Activity Spike

Responsible IP:

172.201.60.191

- Connections from IP 238.163.231.224 excluding New York:

48 Events

---

### Task 5 — KQL (Kibana Query Language)

Practiced advanced filtering using KQL queries.

Examples Used:

```
UserName : "Emanda"
```

```
Source_country : "United States" AND UserName : ("James" OR "Albert")
```

```
UserName : "Johny Brown"
```

Skills Practiced:

- Boolean operators (AND / OR)
- Field filtering
- Multi-condition searching

Investigation Result:

- Johny Brown activity returned:

1 Hit

Source IP:

175.20.60.191

---

### Task 6 — Creating Visualizations

Created log activity visualizations including:

- Time-based activity charts
- User traffic comparison
- Source IP frequency analysis

Purpose:

- Identify abnormal traffic spikes visually
- Compare user behaviours

---

### Task 7 — Creating Dashboards

Built SOC monitoring dashboards combining:

- Timeline activity visualization
- User traffic metrics
- Source IP statistics

Outcome:

Single pane-of-glass monitoring dashboard suitable for SOC monitoring workflow.

---

### Task 8 — Conclusion

Understood how ELK supports SOC operations through:

- Log ingestion
- Real-time searching
- Threat investigation
- Data visualization
- Behavioural anomaly detection

Practiced investigating VPN traffic to identify suspicious users and IP behaviour patterns.

---

## SOC Skills Practiced

- Log investigation workflow
- KQL query building
- Timeline analysis
- Behavioural anomaly detection
- Threat hunting fundamentals
- Visualization creation
- Dashboard monitoring

---

## SOC Tools Simulated

- Elastic Stack (ELK)
- Kibana Discover
- KQL Query Engine
- Dashboard Monitoring Interface

---

## Key Learning

Elastic Stack provides powerful log searching and visualization capabilities enabling SOC analysts to quickly identify anomalies, suspicious traffic spikes, and high-risk user activity across large datasets.

---

## Evidence

Screenshots captured during:

- Discover investigations
- KQL query filtering
- Visualization creation
- Dashboard analysis

Location:

screenshots 

