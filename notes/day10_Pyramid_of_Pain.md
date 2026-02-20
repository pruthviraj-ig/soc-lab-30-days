# SOC Investigation Notes — Pyramid of Pain

Platform: TryHackMe  
Room: Pyramid of Pain  
Role Simulation: SOC Analyst Level 1 — Threat Intelligence & Detection Strategy

---

## Objective

Learn how defenders increase attacker cost by detecting higher-level behaviours rather than simple indicators.

---

## Pyramid of Pain Concept

The Pyramid of Pain measures how difficult it is for attackers to change indicators once defenders detect them.

Higher pyramid levels cause greater operational disruption.

---

## Pyramid Levels

### Hash Values (Trivial)

File fingerprints.

Examples:

- MD5
- SHA256

Used in antivirus detection.

Weakness:

Attackers recompile malware easily.

---

### IP Addresses (Easy)

Used to identify attacker infrastructure.

Detection:

Firewall blocking.

Weakness:

Infrastructure rotation.

---

### Domain Names (Simple)

Used in phishing and malware campaigns.

Example:

Typo-squatting domains.

Detection:

DNS monitoring.

Weakness:

Easy domain registration.

---

### Network Artifacts (Annoying)

Communication behaviour.

Examples:

Beacon intervals.

HTTP traffic patterns.

C2 communications.

Detection:

IDS monitoring.

---

### Host Artifacts (Annoying)

System changes.

Examples:

Registry keys.

Scheduled tasks.

File paths.

Detection:

EDR telemetry.

---

### Tools (Challenging)

Malware frameworks.

Examples:

Ransomware payloads.

Remote administration tools.

Detection:

Behaviour signatures.

Impact:

Requires attacker redevelopment.

---

### TTPs (Tough)

Attacker behaviour patterns.

Examples:

Credential dumping.

Privilege escalation.

Persistence mechanisms.

Detection:

Threat hunting.

MITRE ATT&CK mapping.

Highest operational pain.

---

## Threat Intelligence Strategy

Best SOC defence prioritizes:

Behaviour detection > Tool detection > Network artifacts > Domains > IPs > Hashes.

---

## Malware Behaviour Observation (ANY.RUN)

Observed ransomware activity:

Indicators:

- File encryption behaviour.
- Shadow copy deletion using vssadmin.exe.
- Network connections to external servers.

Example Commands:

vssadmin.exe Delete Shadows.

Purpose:

Prevent recovery.

---

## SOC Analyst Key Takeaways

- Do not rely only on hash blocking.
- Behaviour analysis provides long-term protection.
- Combine SIEM + EDR + Threat Intelligence.

---

## Skills Practiced

IOC categorization.

Threat intelligence analysis.

Malware behavioural awareness.

SOC defensive prioritization.
