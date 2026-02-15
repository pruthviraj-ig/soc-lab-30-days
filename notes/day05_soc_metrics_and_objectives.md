# Day 05 — SOC Metrics & Objectives Notes

Platform: TryHackMe  
Module: SOC Metrics and Objectives

---

## Purpose of SOC Metrics

SOC metrics are used to:

- Measure SOC performance
- Track detection and response efficiency
- Reduce alert noise
- Improve analyst workflow
- Support SLA (Service Level Agreement) targets
- Identify bottlenecks in triage and response

Metrics help SOC management evaluate:
- Tool effectiveness
- Analyst workload
- Detection quality
- Response speed

---

## Core SOC Metrics

### Alerts Count (AC)
Definition:
Total number of alerts received by SOC.

Use:
- Measures analyst workload
- Helps with staffing decisions

Key Point:
- Too many alerts → overload risk
- Too few alerts → possible visibility gap

Typical healthy range:
- ~5–30 alerts per L1 analyst per day

---

### False Positive Rate (FPR)
Formula:
False Positives / Total Alerts

Measures:
- Alert noise level
- Rule quality

Impact:
- High FPR → analyst fatigue
- Increases risk of missing real threats
- Major cause of L1 burnout

Improvement Methods:
- Tune SIEM rules
- Remove known-good noise sources
- Improve detection logic

---

### Alert Escalation Rate (AER)
Formula:
Escalated Alerts / Total Alerts

Measures:
- L1 triage accuracy
- Analyst experience level

Meaning:
- Very high → L1 unsure / rules too sensitive
- Very low → risk of missed escalations

---

### Threat Detection Rate (TDR)
Formula:
Detected Threats / Total Threats

Measures:
- Detection coverage
- SOC visibility effectiveness

Higher is better.

---

## Time-Based SOC Metrics

### Mean Time To Detect (MTTD)

Definition:
Time from attack occurrence → detection by SOC tools.

Measures:
- Detection speed

Affected by:
- SIEM rules
- EDR coverage
- Log visibility
- Detection engineering

Lower MTTD = faster discovery of threats

---

### Mean Time To Acknowledge (MTTA)

Definition:
Time from alert creation → analyst acknowledgement.

Measures:
- L1 responsiveness

Affected by:
- Alert volume
- Staffing levels
- Queue prioritisation
- Triage process

High MTTA = alerts sitting unreviewed too long

---

### Mean Time To Respond (MTTR)

Definition:
Time from detection → full containment/remediation.

Measures:
- SOC response efficiency

Includes:
- Investigation
- Escalation
- Containment actions
- Coordination

High MTTR = attacker stays longer in environment

---

## SLA (Service Level Agreement) in SOC

SLA defines expected SOC performance targets such as:

- Detection time
- Acknowledgement time
- Response time
- Availability (24/7 vs business hours)

SOC metrics are used to prove SLA compliance.

---

## Scenario Learnings From Lab

### Scenario — Slow Response
Problem Metric:
- MTTR too high

Risk:
- Threat not contained quickly

Fix:
- Improve response workflow
- Faster escalation and containment steps

---

### Scenario — Late Detection
Problem Metric:
- MTTD too high

Risk:
- Attack activity goes unnoticed too long

Fix:
- Improve detection rules
- Better monitoring coverage

---

### Scenario — Analyst Burnout

Problem Metric:
- False Positive Rate too high

Impact:
- Alert fatigue
- Missed real threats
- L1 overload

Fix:
- Detection rule tuning
- Noise reduction
- Exclude trusted system events

---

## SOC L1 Interview Takeaways

Be ready to explain:

- Difference between MTTD, MTTA, MTTR
- Why false positives are dangerous
- How alert noise affects SOC performance
- Why metrics matter to SOC managers
- How tuning rules improves security

---

## Quick Memory Hooks

MTTD → How fast we SEE the attack  
MTTA → How fast we TOUCH the alert  
MTTR → How fast we STOP the attack  
FPR → How noisy the system is

---
