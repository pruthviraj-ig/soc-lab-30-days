# Lab 03 — SOC L1 Alert Triage Investigation

Platform: TryHackMe  
Module: SOC L1 Alert Triage

## Objective
Practice SOC Level 1 alert triage workflow — reviewing, assigning, investigating, and closing alerts based on evidence.

## Alert Types Reviewed
- Double-extension file creation
- Potential data exfiltration
- GitHub download alert
- Unusual VPN login
- External brute force attempt

## Actions Performed
- Prioritised alerts by severity
- Assigned alerts to analyst queue
- Reviewed alert metadata (user, host, IP, URL)
- Compared activity context with expected behaviour
- Marked alerts as True Positive / False Positive
- Added analyst investigation comments
- Closed alerts after verdict

## Example Investigation — GitHub Download Alert
- Alert triggered on GitHub repository download
- Reviewed accessed URL
- Verified repository legitimacy
- Confirmed business justification
- Marked as False Positive
- Documented reasoning in analyst comment

## Skills Practiced
- Alert prioritisation
- Triage workflow
- Analyst documentation
- Verdict decision making
- SOC ticket handling

## SOC Tools Simulated
- SIEM alert dashboard
- Alert triage queue
- Analyst case notes

## Key Learning
L1 analyst role focuses on filtering noise, validating alerts with context, and escalating only confirmed threats.
