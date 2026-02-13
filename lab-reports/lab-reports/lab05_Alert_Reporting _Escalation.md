# Lab — SOC L1 Alert Reporting & Escalation

**Platform:** TryHackMe  
**Module:** SOC L1 Alert Reporting  
**Date Completed:** 13 Feb 2026  

---

## Objective

Practice SOC Level 1 reporting and escalation workflow — documenting investigations, applying the Five Ws method, writing structured analyst comments, and escalating high-risk alerts to L2 with proper justification.

---

## Scenario Focus

- Phishing email investigation
- Sensitive document leak alert
- Post-delivery phishing detection
- SOC dashboard escalation workflow

---

## Alert Types Reviewed

- Phishing email marked after delivery
- Spoofed Microsoft support sender alert
- Sensitive data exposure alert
- Suspicious attachment alert (REPORT.rar)

---

## Actions Performed

- Reviewed SOC dashboard alert details
- Opened alert record and examined metadata
- Identified sender, recipient, subject, and indicators
- Verified phishing indicators (spoofed sender, SPF/DKIM fail)
- Applied **Five Ws reporting method**:
  - Who
  - What
  - When
  - Where
  - Why
- Wrote structured analyst investigation comment
- Documented evidence and reasoning
- Set verdict to **True Positive**
- Updated status to **In Progress**
- Escalated alert to assigned L2 analyst
- Saved escalation report for handoff

---

## Example Investigation — Phishing Email Alert

**Trigger:** Email flagged as phishing after delivery  

**Findings:**
- Sender displayed as Microsoft Support
- Sender authentication checks failed (SPF/DKIM)
- Email used urgency and pricing scare tactics
- Suspicious attachment included
- Indicators consistent with spoofed phishing campaign

**Verdict:** True Positive  
**Action:** Escalated to L2 for deeper investigation and response  
**Documentation:** Five Ws report added in analyst comment

---

## Skills Practiced

- SOC alert reporting standards
- Five Ws investigation documentation
- Analyst comment writing
- Escalation justification
- L1 → L2 handoff workflow
- Evidence-based verdict selection
- Phishing indicator recognition
- SOC communication clarity

---

## Tools Simulated

- SOC alert dashboard
- SIEM-style alert view
- Ticket / case management system
- Escalation assignment workflow

---

## Key Learning

SOC L1 analysts must clearly document investigations, not just review alerts. Structured reporting, evidence-backed verdicts, and accurate escalation enable faster and more effective incident response by L2 teams.
