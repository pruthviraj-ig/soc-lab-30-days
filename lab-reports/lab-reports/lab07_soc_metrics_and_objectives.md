# Lab 07 — SOC Metrics & Objectives

Platform: TryHackMe  
Module: SOC Metrics and Objectives  
Focus: SOC performance metrics, SLA concepts, and alert handling efficiency

---

## Objective

Understand how SOC teams measure performance using operational metrics and SLAs.  
Learn how detection, acknowledgement, and response times are tracked and improved to reduce risk and analyst overload.

---

## Core SOC Metrics Studied

### Alerts Count (AC)
- Total number of alerts received by the SOC
- Used to measure analyst workload
- Typical healthy range: ~5–30 alerts per analyst per day

### False Positive Rate (FPR)
- Formula: False Positives / Total Alerts
- Measures alert noise level
- High FPR → analyst fatigue + missed real threats

### Alert Escalation Rate (AER)
- Formula: Escalated Alerts / Total Alerts
- Reflects L1 triage accuracy and experience
- Indicates how often alerts require L2 investigation

### Threat Detection Rate (TDR)
- Formula: Detected Threats / Total Threats
- Measures SOC detection coverage
- Higher rate = better monitoring effectiveness

---

## Time-Based SOC Metrics

### Mean Time to Detect (MTTD)
- Time between attack occurrence and detection by SOC tools
- Driven by SIEM/EDR visibility and detection rules
- Lower MTTD = faster threat discovery

### Mean Time to Acknowledge (MTTA)
- Time between alert creation and analyst acknowledgement
- Measures L1 responsiveness
- Directly affected by queue load and triage process

### Mean Time to Respond (MTTR)
- Time between detection and full containment/remediation
- Includes investigation, escalation, and response actions
- Key SLA performance indicator

---

## Scenario Exercises Completed

### Scenario 1 — Slow Containment Issue
- Identified problem metric: MTTR too high
- Risk: prolonged attacker presence
- Improvement focus: faster response workflow

**Flag Earned:**  
THM{mttr:quick_start_but_slow_response}

---

### Scenario 2 — Detection Delay Issue
- Identified problem metric: MTTD too high
- Risk: late alerting after attack activity
- Improvement focus: better detection rules and monitoring

**Flag Earned:**  
THM{mttd:time_between_attack_and_alert}

---

### Scenario 3 — Analyst Burnout / Noise
- Root cause: High False Positive Rate
- Impact: L1 overload and alert fatigue
- Improvement: tune rules and remove system noise

**Flag Earned:**  
THM{fpr:the_main_cause_of_l1_burnout}

---

## Skills Practiced

- SOC metric interpretation
- SLA understanding
- Detection vs response timing analysis
- Alert noise impact evaluation
- Performance improvement reasoning
- Metric-driven SOC decision making

---

## SOC Concepts Reinforced

- SOC SLAs
- Detection lifecycle timing
- Analyst workload measurement
- False positive reduction strategy
- Metric-driven SOC optimization

---

## Key Learning

SOC effectiveness is measured not only by detection capability but also by response speed and alert quality.  
Reducing false positives and improving MTTD/MTTR directly improves security outcomes and analyst performance.

---
