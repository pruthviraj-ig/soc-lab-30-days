# Lab 08 — SOC Metrics and EDR Investigation

Platform: TryHackMe  
Modules:
- SOC Metrics and Objectives
- Introduction to EDR

---

## Objective

Understand SOC performance metrics and practice endpoint investigation using EDR telemetry, process chains, and threat indicators.

---

## SOC Metrics Covered

- Alerts Count (AC)
- False Positive Rate (FPR)
- Alert Escalation Rate (AER)
- Threat Detection Rate (TDR)
- MTTD — Mean Time To Detect
- MTTA — Mean Time To Acknowledge
- MTTR — Mean Time To Respond

---

## Metrics Understanding

Learned how SOC metrics are used to:

- Measure SOC efficiency
- Evaluate analyst performance
- Reduce alert fatigue
- Improve detection quality
- Support SLA targets

Identified that high False Positive Rate is a major cause of L1 analyst overload and burnout.

---

## EDR Investigation Tasks Performed

- Reviewed EDR dashboard detections
- Analyzed process tree relationships
- Identified suspicious parent-child process chains
- Reviewed command-line execution evidence
- Checked process hash and signature status
- Mapped detection to MITRE ATT&CK technique
- Reviewed registry persistence indicators
- Identified credential dumping behavior
- Observed data exfiltration attempt URL

---

## Key Detection Observed

Detection: Credential dumping via LSASS memory access

Indicators:

- syncsvc.exe execution from Temp directory
- Parent process explorer.exe
- Access to lsass.exe memory
- Dump file creation on disk
- Suspicious command line arguments
- ATT&CK mapping to Credential Dumping (T1003)
- External file upload attempt observed

---

## Skills Practiced

- SOC metric interpretation
- SLA metric understanding
- EDR dashboard navigation
- Process chain analysis
- Behavioral detection review
- ATT&CK mapping usage
- Endpoint investigation workflow
- Threat indicator validation

---

## SOC Tools Simulated

- EDR dashboard
- Process telemetry viewer
- Detection evidence panel
- Threat intelligence mapping
- Endpoint investigation console

---

## Key Learning

SOC metrics guide performance and detection quality, while EDR tools provide deep endpoint visibility required for accurate L1 triage, behavior analysis, and escalation decisions.
