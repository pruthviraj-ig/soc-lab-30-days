# Lab 13 — Pyramid of Pain Threat Intelligence Analysis

Platform: TryHackMe  
Room: Pyramid of Pain  
Role Simulation: SOC Analyst Level 1 — Threat Intelligence & IOC Analysis

---

## Objective

Understand how different Indicators of Compromise (IOCs) impact attackers differently and how defenders can increase adversary operational cost using the Pyramid of Pain model.

The lab focused on identifying IOC categories and understanding how threat detection strategies evolve from simple signatures to behavioural detection.

---

## Technologies Used

- Threat Intelligence Concepts
- IOC Analysis
- ANY.RUN Malware Sandbox (Behaviour Observation)
- Network Traffic Analysis
- SOC Investigation Workflow

---

## Pyramid of Pain Overview

The Pyramid of Pain describes how difficult it is for attackers to change different indicators once detected by defenders.

Lower levels are easier for attackers to modify.

Higher levels significantly disrupt attacker operations.

Hierarchy:

1. Hash Values
2. IP Addresses
3. Domain Names
4. Network Artifacts
5. Host Artifacts
6. Tools
7. TTPs (Tactics Techniques Procedures)

---

## Task 1 — Introduction

Reviewed the Pyramid of Pain framework.

Key Learning:

- Blocking low level IOCs provides temporary protection.
- Behavioural detection provides long-term defence.

---

## Task 2 — Hash Values (Trivial)

Hash values uniquely identify files.

Examples:

- MD5
- SHA1
- SHA256

Usage:

- Malware signature detection.
- Antivirus scanning.

Limitations:

Attackers easily modify malware hashes by recompiling files.

SOC Impact:

Low operational pain to attackers.

---

## Task 3 — IP Addresses (Easy)

IP addresses identify attacker infrastructure.

Examples:

- Command and Control servers.
- Malware download hosts.

Detection:

- Firewall blocking.
- SIEM alerts.

Limitations:

Attackers frequently rotate IP infrastructure.

SOC Impact:

Easy for attackers to replace.

---

## Task 4 — Domain Names (Simple)

Domains are used in phishing campaigns or malware communication.

Example:

Typo-squatting domains.

Detection Methods:

- DNS monitoring.
- Threat intelligence feeds.

Limitations:

Attackers can register new domains quickly.

SOC Impact:

Moderate disruption.

---

## Task 5 — Host Artifacts (Annoying)

Artifacts left on infected systems.

Examples:

- Registry modifications.
- File execution paths.
- Scheduled tasks.

Detection Tools:

- EDR telemetry.
- Endpoint monitoring.

SOC Impact:

Attackers must modify malware behaviour.

Higher operational cost.

---

## Task 6 — Network Artifacts (Annoying)

Observable traffic behaviour.

Examples:

- C2 beaconing traffic.
- Specific HTTP headers.
- DNS request patterns.

Detection:

- Network monitoring.
- IDS/IPS alerts.

SOC Impact:

Attackers must redesign communication protocols.

---

## Task 7 — Tools (Challenging)

Malware frameworks and utilities used by attackers.

Examples:

- Ransomware families.
- Exploitation frameworks.

Detection:

- Behaviour signatures.
- EDR detections.

SOC Impact:

Changing tools requires rebuilding attack infrastructure.

High disruption.

---

## Task 8 — TTPs (Tough)

Tactics Techniques and Procedures describe attacker behaviour.

Examples:

- Privilege escalation methods.
- Lateral movement patterns.

Framework:

MITRE ATT&CK.

Detection:

Behavioural monitoring and threat hunting.

SOC Impact:

Extremely difficult for attackers to change.

Maximum defensive advantage.

---

## Task 9 — Practical Investigation

Completed IOC classification exercise by placing investigation prompts into appropriate Pyramid of Pain tiers.

Examples:

- Infrastructure identification → IP addresses.
- Typo squatting domains → Domain names.
- Payload attribution → Tools.
- Campaign objectives → TTPs.

Successfully completed static investigation workflow.

Flag Obtained:

THM{PYRAMID_OF_PAIN_COMPLETE}

---

## Task 10 — Conclusion

Learned how prioritizing higher-level indicators improves SOC effectiveness.

Behavioural detection significantly increases attacker effort and reduces repeated compromise.

---

## SOC Skills Practiced

- IOC classification.
- Threat intelligence analysis.
- Behavioural detection strategy.
- Malware investigation mindset.
- Defensive prioritization planning.

---

## SOC Tools Simulated

- Threat Intelligence Platforms.
- SIEM detection workflow.
- Malware Sandbox Analysis (ANY.RUN).

---

## Key Learning

Blocking hashes or IPs provides short-term defence.

Detecting tools and attacker behaviours forces adversaries to redesign campaigns entirely.

Behavioural detection provides strongest long-term protection.

---

## Evidence

Screenshots captured during:

- Pyramid classification practical.
- ANY.RUN ransomware behavioural analysis.
- IOC investigation workflow.

Location:

screenshots/
