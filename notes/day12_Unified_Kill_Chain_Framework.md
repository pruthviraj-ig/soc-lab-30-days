# SOC Investigation Notes — Unified Kill Chain Framework

Platform: TryHackMe  
Room: Unified Kill Chain  
Role Simulation: SOC Analyst Level 1 — Threat Modelling & Attack Lifecycle Investigation

---

## Objective

Understand attacker progression across network compromise stages and improve SOC detection through structured attack lifecycle analysis.

---

## What is a Kill Chain

A Kill Chain represents stages attackers follow during cyber intrusions.

SOC analysts use kill chain analysis to:

- Detect attacks earlier.
- Interrupt attacker progression.
- Improve response actions.

---

## Threat Modelling

Threat modelling identifies:

- Threat actors.
- Attack surfaces.
- Vulnerabilities.
- Defensive gaps.

Helps SOC teams anticipate attacker behaviour.

---

## Unified Kill Chain Goals

---

### Goal In — Initial Foothold

Initial system compromise methods.

Examples:

- Phishing emails.
- Credential theft.
- Web application exploitation.

SOC Indicators:

- Suspicious login attempts.
- Unknown source access.

---

### Goal Through — Network Propagation

Attacker expands access inside network.

Activities:

- Privilege escalation.
- Lateral movement.
- Persistence establishment.

Example:

Repeated administrator login failures.

SOC Detection:

- Account lockout alerts.
- Credential misuse.

---

### Goal Out — Actions on Objectives

Final attacker objectives.

Examples:

- Data exfiltration.
- Ransomware deployment.
- System destruction.

SOC Priority:

Immediate containment.

---

## Attack Lifecycle Phases

Unified Kill Chain tracks:

- Reconnaissance.
- Initial access.
- Expl​​oitation.
- Persistence.
- Privilege escalation.
- Pivoting.
- Command and Control.

---

## Example Investigation Scenario

Alert:

Multiple failed administrator login attempts.

SOC Analysis:

Attacker attempting elevated privileges.

Phase:

Privilege Escalation.

Action:

Escalate investigation.

---

## SOC Benefits

Unified Kill Chain helps analysts:

- Identify lateral movement.
- Detect persistence mechanisms.
- Track attacker intent.

---

## SOC Skills Practiced

- Threat modelling thinking.
- Incident lifecycle analysis.
- Attack stage classification.
- Investigation decision making.

---

## Key Learning

Understanding attacker objectives allows SOC analysts to stop intrusions before data exfiltration or ransomware deployment occurs.

---

## Evidence

Screenshots captured during:

- Practical exercises.
- Scenario analysis.

Location:

screenshots/
