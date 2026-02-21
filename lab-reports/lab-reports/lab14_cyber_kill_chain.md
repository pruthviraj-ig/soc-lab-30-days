# Lab 14 — Cyber Kill Chain Investigation & Attack Lifecycle Analysis

Platform: TryHackMe  
Room: Cyber Kill Chain  
Role Simulation: SOC Analyst Level 1 — Attack Lifecycle Analysis & Incident Investigation

---

## Objective

Understand the Cyber Kill Chain framework and how SOC analysts use it to identify, detect, investigate, and disrupt cyber attacks by analysing each phase of adversary activity.

---

## Framework Overview

The Cyber Kill Chain was developed by Lockheed Martin to describe the stages attackers follow during a cyber intrusion.

Understanding attacker progression allows SOC analysts to:

- Detect attacks earlier
- Identify missing security controls
- Improve incident response strategy
- Prevent future compromises

---

## Cyber Kill Chain Phases Studied

1. Reconnaissance
2. Weaponization
3. Delivery
4. Exploitation
5. Installation
6. Command and Control (C2)
7. Actions on Objectives

---

## Tasks Completed

### Task 1 — Introduction

- Learned origins of Cyber Kill Chain framework.
- Understood how attackers must successfully complete multiple stages to achieve compromise.
- Reviewed SOC defensive advantages when attacks are stopped early.

---

### Task 2 — Reconnaissance

Studied attacker information gathering techniques.

Examples:

- OSINT collection
- Social media research
- Domain enumeration
- Employee targeting.

SOC Detection Opportunities:

- Suspicious scanning activity.
- Enumeration attempts.

---

### Task 3 — Weaponization

Learned how attackers prepare payloads.

Examples:

- Malware creation.
- Exploit kit preparation.
- Maldoc creation.

Goal:

Combine exploit and payload before delivery.

---

### Task 4 — Delivery

Studied attack delivery mechanisms.

Examples:

- Spear phishing attachments.
- Malicious downloads.
- Drive-by websites.

Practical Scenario:

- Spearphishing attachment mapped to Delivery phase.

SOC Monitoring:

- Email gateway alerts.
- Attachment scanning.

---

### Task 5 — Exploitation

Attackers exploit vulnerabilities.

Examples:

- Exploit public-facing applications.
- Software vulnerability abuse.

Scenario Mapping:

- Exploit public-facing application classified as Exploitation.

SOC Detection:

- IDS alerts.
- Exploit behaviour monitoring.

---

### Task 6 — Installation

Attacker establishes persistence.

Examples:

- Dynamic linker hijacking.
- Malware installation.

Scenario Mapping:

- Dynamic linker hijacking mapped to Installation phase.

SOC Detection:

- Suspicious process creation.
- Persistence registry modifications.

---

### Task 7 — Command and Control (C2)

Attacker establishes remote communication.

Examples:

- Fallback communication channels.
- Beaconing traffic.

Scenario Mapping:

- Fallback channels mapped to C2 phase.

SOC Indicators:

- Periodic outbound connections.
- Unknown infrastructure traffic.

---

### Task 8 — Actions on Objectives

Final attacker goal execution.

Examples:

- Data theft.
- Credential harvesting.
- Lateral movement.

Scenario Mapping:

- Data exfiltration from local systems.

SOC Detection:

- Large outbound transfers.
- Sensitive file access anomalies.

---

### Task 9 — Practical Scenario

Completed Cyber Kill Chain mapping exercise.

Scenario Included:

- Spearphishing attachment.
- Exploit public application.
- Dynamic linker hijacking.
- PowerShell activity.
- Fallback communication channels.
- Data exfiltration.

Activities Performed:

- Analysed attacker activity prompts.
- Classified indicators into correct Kill Chain stages.
- Validated mapping using static site lab.

Outcome:

Successfully completed scenario workflow.

---

### Task 10 — Conclusion

Understood how Cyber Kill Chain helps SOC teams:

- Detect attacks earlier.
- Identify attacker behaviour patterns.
- Improve incident containment strategy.

---

## SOC Skills Practiced

- Attack lifecycle analysis.
- Threat behaviour mapping.
- Incident investigation thinking.
- Detection opportunity identification.
- SOC defensive strategy planning.

---

## SOC Tools Simulated

- SIEM alert analysis concepts.
- Email security gateway monitoring.
- IDS/IPS detection workflows.
- Endpoint monitoring concepts.

---

## Key Learning

Cyber Kill Chain enables SOC analysts to break attacks early by understanding adversary progression. Early detection during Reconnaissance or Delivery significantly reduces organisational impact compared to late-stage detection.

---

## Evidence

Screenshots captured during:

- Practical Kill Chain scenario mapping.
- Attack stage classification exercise.

Location:

screenshots/
