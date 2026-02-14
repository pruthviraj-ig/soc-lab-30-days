# Lab — SOC Workbooks and Lookups

**Platform:** TryHackMe  
**Module:** SOC Workbooks and Lookups  
**Date Completed:** 14 Feb 2026  

---

## Objective

Practice SOC Level 1 triage using structured workbooks and lookup resources to enrich alerts, validate context, map assets and subnets, and make consistent escalation decisions using guided investigation workflows.

---

## Scenario Focus

- Workbook-driven alert triage
- Asset and identity enrichment
- Network diagram interpretation
- Subnet classification
- Port-to-service mapping
- VPN brute force attack path analysis
- Structured escalation decision flow

---

## Investigation Areas Covered

- User identity and role lookup
- Asset purpose and access scope
- Network subnet mapping
- Exposed service identification by port
- VPN access workflow
- Internal port scanning scenario
- Email analysis workbook
- PowerShell activity workbook
- Network analysis workbook

---

## Actions Performed

- Reviewed SOC workbook investigation model
- Followed decision-tree style triage flowcharts
- Used asset and identity lookup references
- Mapped IP addresses to correct subnets
- Identified services based on port numbers
- Interpreted network diagram relationships
- Traced attacker path across network segments
- Validated which services were externally exposed
- Determined correct subnet ownership for target hosts
- Applied workbook logic to decide escalation vs closure
- Completed three guided workbooks:
  - Email Analysis
  - PowerShell Analysis
  - Network Analysis

---

## Example Investigation — VPN Brute Force Scenario

**Trigger:** External IP performed repeated VPN login attempts

**Findings:**
- Multiple failed VPN login attempts observed
- Successful login occurred after brute force attempts
- Attacker assigned IP from VPN subnet
- Attempted access toward database subnet
- Firewall rules blocked database subnet scanning
- Attacker shifted targeting toward office subnet

**Verdict:** True Positive  
**Action:** Follow workbook escalation path and investigation workflow

---

## Skills Practiced

- Workbook-based triage methodology
- Alert enrichment using lookup sources
- Asset and identity context building
- Network diagram analysis
- Subnet classification
- Port and service mapping
- Structured decision making
- Repeatable SOC investigation workflow

---

## Tools & Resources Simulated

- SOC investigation workbooks
- Network diagrams
- Asset inventory records
- Identity directory lookup
- Port/service reference tables
- Triage decision flowcharts

---

## Key Learning

SOC workbooks provide standardized investigation paths that reduce analyst guesswork and improve consistency across shifts. Lookup resources and decision trees help L1 analysts enrich alerts faster and make accurate escalation decisions.
