# Day 03 — SOC L1 Alert Triage Notes

## What is Alert Triage
Alert triage = process of reviewing, prioritising, and validating security alerts before escalation.

SOC L1 goal:
- Filter noise
- Validate alerts
- Close false positives
- Escalate real threats

---

## Common Alert Sources
- SIEM
- EDR
- Email security tools
- IDS / IPS
- VPN logs
- DLP alerts

Examples seen in lab:
- Double extension file
- Data exfiltration alert
- GitHub download alert
- VPN unusual location
- Brute force attempt

---

## L1 Analyst Workflow

1. Sort alerts by severity
2. Assign alert to yourself
3. Move status → In Progress
4. Read alert description
5. Check fields:
   - user
   - host
   - IP
   - URL
   - country
   - activity type
6. Check context (normal vs abnormal)
7. Add analyst comment
8. Set verdict:
   - True Positive
   - False Positive
9. Close or escalate to L2

---

## True vs False Positive

True Positive:
- Real malicious activity
- Policy violation
- Confirmed suspicious behaviour

False Positive:
- Legitimate business activity
- Approved software/site
- User behaviour justified

Always write reason in comment.

---

## Example Decisions

GitHub download alert:
- Checked URL
- Verified trusted repo
- Business usage valid
- Verdict = False Positive

Brute force alert:
- Multiple failed attempts
- External source
- Malicious pattern
- Verdict = True Positive

---

## Good Analyst Practice
- Never close without comment
- Always check context
- Do not trust severity alone
- Verify with evidence
- Follow runbook if available
- Escalate when unsure

---

## Skills Practiced
- Alert prioritisation
- SOC workflow handling
- Investigation reasoning
- Ticket documentation
- Decision justification
