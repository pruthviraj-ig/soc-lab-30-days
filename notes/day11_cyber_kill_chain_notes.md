# SOC Investigation Notes — Cyber Kill Chain Framework

Platform: TryHackMe  
Room: Cyber Kill Chain  
Role Simulation: SOC Analyst Level 1 — Attack Lifecycle Investigation

---

## Objective

Understand attacker methodology and how SOC analysts detect intrusions by analysing each stage of the Cyber Kill Chain.

---

## What is Cyber Kill Chain

Cyber Kill Chain describes how attackers move step-by-step from reconnaissance to achieving their objective.

Developed by:

Lockheed Martin (2011).

Purpose:

- Identify attacker behaviour.
- Improve defensive detection.
- Stop attacks earlier.

---

## Importance for SOC Analysts

Helps analysts:

- Detect threats before compromise.
- Identify missing security controls.
- Improve incident response.

Earlier detection equals lower business impact.

---

## Kill Chain Phases

### 1. Reconnaissance

Attacker gathers information.

Examples:

- OSINT research.
- Domain scanning.
- Employee targeting.

Detection:

- Network scanning alerts.

---

### 2. Weaponization

Payload preparation stage.

Examples:

- Malware creation.
- Exploit development.
- Malicious document creation.

Occurs outside victim network.

Detection is limited.

---

### 3. Delivery

Payload sent to victim.

Methods:

- Spear phishing email.
- Malvertising.
- USB devices.

Example:

Spearphishing attachment.

SOC Controls:

- Email filtering.
- Sandbox analysis.

---

### 4. Exploitation

Vulnerability execution.

Examples:

- Exploit public facing application.
- Software vulnerability abuse.

SOC Detection:

- Endpoint alerts.
- IDS signatures.

---

### 5. Installation

Persistence establishment.

Examples:

- Dynamic linker hijacking.
- Backdoor installation.

Indicators:

- Startup modifications.
- Suspicious services.

---

### 6. Command and Control (C2)

Attacker communicates remotely.

Examples:

- Fallback channels.
- Beacon traffic.

Indicators:

- Periodic outbound connections.

SOC Detection:

- DNS monitoring.
- Proxy logs.

---

### 7. Actions on Objectives

Final attacker goal.

Examples:

- Data exfiltration.
- Credential theft.
- Lateral movement.

Detection:

- Large data transfers.

---

## Practical Scenario Mapping

Mapped attacker actions:

- Spearphishing attachment → Delivery.
- Exploit public application → Exploitation.
- Dynamic linker hijacking → Installation.
- Fallback channels → Command & Control.
- Data from local system → Actions on Objectives.

---

## SOC Analyst Detection Strategy

Best defence:

Stop attacker early stages.

Priority Detection Areas:

- Reconnaissance scanning.
- Email phishing attempts.
- Exploit attempts.

Late detection increases damage risk.

---

## SOC Skills Practiced

- Attack lifecycle analysis.
- Threat intelligence reasoning.
- Incident investigation workflow.

---

## Key Learning

Cyber Kill Chain provides structured understanding of attacker progression allowing SOC analysts to detect threats earlier and implement layered defensive monitoring.

---

## Evidence

Screenshots captured during:

- Kill Chain mapping practical.

Location:

screenshots/
