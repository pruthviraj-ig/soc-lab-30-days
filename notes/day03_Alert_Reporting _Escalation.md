SOC Investigation Scenario — Alert Reporting & Escalation (Phishing)

Alert:
Phishing email detected after delivery with spoofed sender and suspicious attachment

Scenario Summary:
SOC dashboard flagged an email as phishing post-delivery. Email claimed to be from Microsoft Support and used urgency language about pricing increase. Authentication checks failed and attachment was suspicious.

Steps Taken:
- Opened SOC dashboard alert queue
- Selected phishing alert record
- Reviewed alert metadata (sender, recipient, subject, attachment)
- Checked sender display name vs actual email address
- Verified SPF and DKIM results — both failed
- Reviewed email subject and keyword indicators
- Identified urgency and scare-tactic language
- Noted suspicious attachment (REPORT.rar)
- Applied Five Ws reporting method:
  - Who — recipient and sender details
  - What — phishing email with spoofing indicators
  - When — alert timestamp
  - Where — email delivery context
  - Why — authentication failure + phishing patterns
- Wrote structured analyst comment
- Documented investigation evidence
- Set verdict to True Positive
- Changed alert status to In Progress
- Escalated alert to L2 analyst
- Saved report for escalation handoff

Email Indicators:
- Sender spoofing (Microsoft Support display name)
- SPF check failed
- DKIM check failed
- Urgent financial theme
- Suspicious compressed attachment
- Phishing keyword patterns

Reporting Skills Practiced:
- Five Ws incident reporting
- Analyst comment writing
- Evidence documentation
- Escalation justification
- L1 to L2 handoff process

Key Learning:
Good SOC work is not only detecting malicious activity but clearly documenting findings. Structured reports help L2 teams investigate faster and reduce miscommunication.
