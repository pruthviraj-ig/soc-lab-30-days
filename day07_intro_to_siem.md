# TryHackMe — Introduction to SIEM (SOC Level 1 Path)

## Lab Summary

Completed the TryHackMe "Introduction to SIEM" room focused on understanding SIEM architecture, log ingestion, alert generation, and SOC analyst investigation workflow.

This lab simulated a SOC dashboard where alerts were triggered based on detection rules and suspicious process activity.

---

## Key Concepts Learned

### What is SIEM

SIEM (Security Information and Event Management) is a centralized platform used to:

• Collect logs from multiple sources  
• Normalize and correlate events  
• Detect suspicious behavior using rules  
• Generate security alerts  
• Support SOC investigation and response  

---

## Log Sources in SIEM

Common log sources ingested into SIEM:

• Windows Event Logs  
• Endpoint security tools  
• Firewall logs  
• Network devices  
• Authentication logs  
• Application logs  
• EDR telemetry  

---

## Alerting Workflow

SIEM alert lifecycle observed in lab:

1. Logs ingested from host
2. Detection rule matched
3. Alert generated
4. Analyst reviews event
5. Process + user + host examined
6. Rule match term identified
7. Decision made:

- True Positive → take action (isolate host)
- False Positive → tune rule

---

## Investigation Skills Practiced

### Alert Investigation

• Reviewed suspicious process execution  
• Identified triggering rule keyword  
• Matched event to detection rule  
• Validated process behavior  
• Determined alert legitimacy  

---

### SOC Decision Making

Practiced analyst response selection:

• True Positive → isolate affected host  
• False Positive → tune detection rule  

---

## SIEM Dashboard Analysis

Reviewed dashboard widgets:

• Top event codes  
• Process execution counts  
• IP + Port destinations  
• MITRE ATT&CK technique mapping  
• RDP connection sources  
• Event timeline trends  

---

## MITRE ATT&CK Mapping

SIEM alerts can be mapped to:

• Techniques  
• Tactics  
• Attack stages  

This helps analysts understand attacker behavior context.

---

## SOC Skills Strengthened

• SIEM alert review  
• Rule-based detection understanding  
• Event log analysis  
• True/False positive classification  
• SOC response workflow  
• Investigation documentation  
• Detection rule reasoning  

---

## Practical SOC Relevance

This lab directly supports SOC L1 responsibilities:

• Alert triage  
• Log review  
• Detection validation  
• Initial incident classification  
• Escalation decision support  
