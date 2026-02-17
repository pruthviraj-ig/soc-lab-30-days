# SOC Lab Report — SIEM Alert Investigation (TryHackMe Introduction to SIEM)

## Lab Title
SIEM Fundamentals and Alert Investigation — Introduction to SIEM

## Platform
TryHackMe — SOC Level 1 Path

## Lab Type
SIEM Dashboard Analysis + Alert Investigation Simulation

---

## Objective

The objective of this lab was to understand how a SIEM platform collects logs, triggers alerts based on detection rules, and supports SOC analyst investigation and response decisions.

The lab simulated a SIEM dashboard where suspicious activity triggered alerts that required analyst review and classification.

---

## Skills Practiced

• SIEM dashboard navigation  
• Log event analysis  
• Detection rule matching  
• Alert triage workflow  
• Suspicious process identification  
• True Positive vs False Positive classification  
• SOC response decision making  
• Basic MITRE ATT&CK mapping awareness  

---

## SIEM Concepts Reviewed

### SIEM Core Functions

The SIEM platform performs:

• Centralized log collection  
• Event normalization  
• Rule-based detection  
• Alert generation  
• Event correlation  
• Investigation support  

---

## Log Sources Observed

The SIEM dashboard included events from:

• Windows Event Logs  
• Process creation events  
• Authentication activity  
• Host telemetry  
• Network connection records  

---

## Investigation Scenario

A suspicious activity simulation was triggered using a dashboard control. This generated events that matched an existing SIEM detection rule and produced an alert.

The investigation required:

1. Reviewing the triggered alert
2. Identifying the affected host
3. Identifying the suspicious user
4. Finding the suspicious process
5. Checking which rule keyword matched
6. Determining alert validity
7. Selecting appropriate SOC action

---

## Key Investigation Findings

### Suspicious Process Identified
miner.exe
### Detection Rule Match Term
miner
### Affected Host
HR_02
### Alert Classification
True Positive
Reason:
The process behavior matched the SIEM detection rule and indicated unauthorized or suspicious execution consistent with malicious activity.

---

## SOC Analyst Decision

Based on alert validation:

**Selected Action:**  
True Positive → Isolate Host

This reflects correct SOC workflow for confirmed malicious behavior.

---

## SIEM Dashboard Analysis Performed

Reviewed dashboard panels including:

• Top event codes  
• Process execution frequency  
• IP and port destinations  
• Event count trends  
• MITRE ATT&CK technique mapping  
• Detection severity levels  

---

## Detection Workflow Observed

SIEM detection pipeline in this lab:

Log Source → Event Ingestion → Rule Match → Alert Trigger → Analyst Review → Classification → Action

---

## MITRE ATT&CK Mapping Value

The SIEM dashboard showed technique mapping to MITRE ATT&CK categories, which helps analysts:

• Understand attacker behavior stage  
• Classify technique type  
• Improve escalation accuracy  
• Support threat reporting  

---

## SOC L1 Relevance

This lab directly supports SOC Level 1 responsibilities:

• Alert triage  
• Rule-trigger investigation  
• Process analysis  
• Log review  
• Event validation  
• Alert classification  
• Response selection  
• Case documentation  

---

## Outcome

Successfully completed SIEM alert investigation simulation and correctly classified the alert as a True Positive based on rule match and process behavior.

Demonstrated practical understanding of SIEM alert workflow and SOC analyst response decisions.

---

## Evidence

Screenshots captured and stored in:

screenshots file


