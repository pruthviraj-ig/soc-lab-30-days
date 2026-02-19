# Day 10 — Elastic Stack (ELK) Log Investigation Notes

Platform: TryHackMe  
Room: Investigating with ELK (Elastic Stack)  
Focus: SOC Analyst Log Investigation & Visualization Workflow

---

## Overview

The Elastic Stack (ELK) is widely used in Security Operations Centers (SOC) for centralized log analysis, investigation, visualization, and threat detection. Although not a traditional SIEM, ELK provides SIEM-like capabilities through powerful indexing and search features.

ELK enables analysts to collect, parse, search, and visualize large datasets to detect suspicious behaviour patterns.

---

## ELK Stack Components

### Elasticsearch

- Core search and analytics engine.
- Stores logs in indexed format.
- Enables fast querying across large datasets.
- Supports structured and unstructured log data.

Key Functions:

- Indexing data
- Query searching
- Data aggregation

---

### Logstash

- Data ingestion pipeline.
- Collects logs from multiple sources.
- Parses and transforms logs before storage.

Examples:

- Firewall logs
- VPN logs
- Windows Event Logs
- Web server logs

---

### Kibana

Visualization and investigation interface.

SOC analysts use Kibana to:

- Search logs
- Apply filters
- Investigate alerts
- Build dashboards.

Main Features:

- Discover tab
- Visualizations
- Dashboards
- KQL searching

---

## Lab Environment

Connected using TryHackMe AttackBox.

Accessed Kibana web interface for investigation activities.

Dataset Used:

vpn_connections index.

---

## Discover Tab Investigation

The Discover tab allows analysts to explore raw log events.

Activities Performed:

- Selected index vpn_connections.
- Applied investigation time range filters.
- Reviewed timeline activity graph.

Fields Investigated:

- Source_ip
- UserName
- Source_country
- Source_state
- Timestamp
- Protocol
- Port

Purpose:

Identify abnormal behaviour patterns and suspicious VPN activity.

---

## Discover Investigation Findings

Total Events:

2861 VPN log events between Dec 31 2021 and Feb 02 2022.

Maximum Connection Source IP:

238.163.231.224

User Responsible for Maximum Traffic:

James

User Filter Applied:

UserName = Emanda

Highest Source IP Hits:

107.14.1.247

Traffic Spike Observed:

11 January.

Responsible IP:

172.201.60.191

Filtered Investigation:

Connections from IP 238.163.231.224 excluding New York:

48 Events.

---

## KQL (Kibana Query Language)

KQL allows analysts to perform advanced filtering.

Used For:

- Searching specific users.
- Combining conditions.
- Threat hunting.

Examples Used:

```
UserName : "Emanda"

Source_country : "United States" AND UserName : ("James" OR "Albert")

UserName : "Johny Brown"
```

Skills Practiced:

- Boolean logic (AND / OR).
- Field filtering.
- Multi-condition queries.

Result:

Johny Brown activity returned:

1 Hit.

Source IP:

175.20.60.191

---

## Visualizations

Created visual charts to analyse behaviour patterns.

Visualizations Included:

- Time-based activity histogram.
- User traffic comparison charts.
- Source IP distribution.

Purpose:

- Identify abnormal spikes.
- Detect unusual user behaviour.

---

## Dashboards

Built SOC monitoring dashboards combining:

- Activity timeline.
- User traffic statistics.
- Source IP frequency analysis.

Outcome:

Centralized monitoring dashboard for quick SOC investigation workflow.

Single pane-of-glass visibility improves detection efficiency.

---

## SOC Analyst Skills Practiced

- Log analysis workflow.
- Threat investigation.
- Timeline correlation.
- KQL query construction.
- Behaviour anomaly detection.
- Visualization analysis.
- Dashboard monitoring.

---

## Tools Used

- Elastic Stack (ELK).
- Kibana Discover.
- KQL Query Engine.
- Elastic Visualization Tools.

---

## Key Learning

Elastic Stack enables SOC analysts to quickly search and analyse massive datasets to identify suspicious behaviour patterns, investigate anomalies, and build monitoring dashboards for proactive threat detection.

---

## Evidence

Screenshots captured during:

- Discover investigations.
- Query filtering.
- Visualization creation.
- Dashboard analysis.

Location:

screenshots/
