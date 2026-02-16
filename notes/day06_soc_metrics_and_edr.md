# Day 06 — SOC Metrics & Introduction to EDR Notes

Platform: TryHackMe  
Modules:
- SOC Metrics and Objectives
- Introduction to EDR

---

## SOC Metrics — Purpose

SOC metrics are used to:

- Measure SOC performance
- Improve detection and response efficiency
- Reduce analyst overload and alert fatigue
- Track response speed and detection quality
- Support SLA (Service Level Agreement) targets

Metrics are also used to evaluate analyst performance and SOC maturity.

---

## Core SOC Metrics

### Alerts Count (AC)
Formula:
AC = Total number of alerts received

Measures:
- Analyst workload
- SIEM alert volume
- Detection noise level

Typical baseline:
5–30 alerts per day per L1 analyst (depends on environment size)

---

### False Positive Rate (FPR)
Formula:
FPR = False Positives / Total Alerts

Measures:
- Alert noise quality
- Detection rule accuracy
- SIEM tuning effectiveness

High FPR leads to:
- Analyst burnout
- Missed real threats
- Alert fatigue

---

### Alert Escalation Rate (AER)
Formula:
AER = Escalated Alerts / Total Alerts

Measures:
- L1 triage accuracy
- Escalation quality
- Analyst experience level

---

### Threat Detection Rate (TDR)
Formula:
TDR = Detected Threats / Total Threats

Measures:
- SOC detection capability
- Tool coverage effectiveness

---

## SOC SLA Time Metrics

### MTTD — Mean Time To Detect
Time between attack occurrence and detection by SOC tools.

Lower is better.

---

### MTTA — Mean Time To Acknowledge
Time between alert creation and analyst acknowledgement.

Measures:
- Analyst responsiveness
- Queue handling efficiency

---

### MTTR — Mean Time To Respond / Remediate
Time from detection to full mitigation.

Includes:
- Investigation
- Escalation
- Containment
- Remediation

---

## Metric Improvement Strategies

- Tune SIEM rules to reduce false positives
- Prioritize high severity alerts
- Improve triage playbooks
- Automate repetitive enrichment tasks
- Improve alert classification accuracy
- Separate IT noise from security alerts

---

# Introduction to EDR — Key Concepts

## What is EDR?

Endpoint Detection and Response (EDR) is a security solution that:

- Monitors endpoint activity
- Detects suspicious behavior
- Records process telemetry
- Provides investigation context
- Supports response actions

EDR focuses on **host-level threats**, not network-level threats.

---

## EDR Key Capabilities

### Visibility
Provides full process and behavior visibility across endpoints.

Includes:
- Process trees
- Command lines
- File activity
- Registry changes
- Network connections

---

### Behavioral Detection

Detects threats based on behavior patterns instead of signatures.

Example:
- winword.exe spawning powershell.exe
- Unusual parent-child process chains

---

### Anomaly Detection

Detects deviation from normal baseline behavior.

Example:
- Rare registry modification
- Unusual startup execution

---

### IOC Matching

Matches activity against:

- Known malicious hashes
- Known domains
- Known IP indicators

---

### MITRE ATT&CK Mapping

EDR maps detections to:

- Tactics
- Techniques
- Attack stages

Example:
Credential dumping → ATT&CK T1003

Helps analysts understand attacker intent and stage.

---

### Machine Learning Detection

Uses models trained on:

- Normal behavior
- Malicious behavior patterns

Detects complex attack chains.

---

## EDR Artefact Collection

EDR supports remote evidence collection:

- Memory dumps
- Event logs
- File artifacts
- Registry hives

Used for:
- Forensics
- Deep investigation
- Incident reporting

---

## EDR Investigation Example Observed

Observed detection:

- Process: syncsvc.exe
- Parent: explorer.exe
- Target: lsass.exe
- Behavior: Credential dumping
- Action: Memory dump written to disk
- Path: AppData Temp directory
- ATT&CK mapping: T1003 Credential Dumping
- Exfil attempt: HTTPS file upload URL observed

Indicators:

- LSASS memory access
- Temp directory executable
- Dump file creation
- Suspicious command line arguments

---

## Analyst Takeaway

EDR provides:

- Deep process visibility
- Behavior-based detection
- ATT&CK mapping context
- Investigation-ready telemetry
- Rapid containment options

Critical tool for SOC L1 triage and escalation.
