# SOC Investigation Notes — Introduction to SOAR (Security Orchestration Automation and Response)

**Platform:** TryHackMe  
**Room:** Introduction to SOAR  
**Role Simulation:** SOC Analyst Level 1 — Automation & Incident Response Workflow

---

## Objective

Understand how Security Orchestration, Automation, and Response (SOAR) improves SOC efficiency by automating investigations, coordinating multiple security tools, and reducing analyst workload through playbooks.

---

## What is SOAR

SOAR (Security Orchestration, Automation, and Response) integrates multiple security technologies into a single platform to automate investigations and response workflows.

SOC analysts can investigate alerts without manually switching between tools.

SOAR provides:

- Tool orchestration
- Automated workflows
- Case management
- Incident tracking

---

## Traditional SOC Challenges

SOC teams commonly face:

- Alert fatigue caused by high alert volume
- Manual investigation workflows
- Switching between multiple security tools
- Communication delays across IT teams
- Slow incident response times

---

## SOC Core Capabilities

SOC operations include:

---

### Monitoring and Detection

- Continuous monitoring using SIEM tools
- Detect suspicious login behaviour or anomalies

Example indicators:

- Multiple failed login attempts
- Login from unknown locations

---

### Recovery and Remediation

SOC analysts act as first responders by:

- Isolating infected endpoints
- Blocking malicious IPs using firewall controls
- Disabling compromised user accounts via IAM

Tools Used:

- EDR
- Firewall
- IAM

---

### Threat Intelligence

SOC teams consume threat intelligence feeds including:

- Malicious IP addresses
- Domains
- File hashes

Used for reputation checking and blocking threats.

---

### Communication

SOC analysts coordinate with:

- IT operations
- Management teams
- Incident response teams

Example:

- Creating tickets for patch validation.

---

## SOAR Core Concepts

SOAR improves SOC workflow through:

---

### Orchestration

Coordinates multiple tools together.

Example integrations:

- SIEM
- Threat Intelligence platforms
- Firewall
- IAM systems
- Ticketing systems

Analysts avoid manual switching between tools.

---

### Automation

Predefined workflows automatically perform investigation steps.

Example automated actions:

- Query SIEM logs
- Check IP reputation
- Validate login behaviour
- Create investigation tickets automatically

Automation reduces analyst workload.

---

### Response

SOAR automatically performs containment actions such as:

- Blocking malicious IPs
- Disabling compromised accounts
- Sending notifications to response teams

---

## SOAR Playbooks

Playbooks are predefined investigation workflows that guide alert handling step by step.

Benefits include:

- Consistent investigations
- Faster response times
- Reduced human error

---

## Example Playbook — VPN Brute Force Investigation

Workflow:

1. Alert received from SIEM
2. Check user login history
3. Verify IP reputation via threat intelligence
4. Query successful login events
5. Escalate containment actions if malicious

Playbooks dynamically change based on investigation results.

---

## Automation Workflow Example

SOAR automatically performs:

1. Receive SIEM alert
2. Query historical login behaviour
3. Perform reputation lookup
4. Open investigation ticket

No manual analyst actions required during initial triage.

---

## Phishing Playbook

SOC investigation workflow:

1. Suspicious email received
2. Create investigation ticket
3. Check email for attachments or URLs

Decision Process:

If no URLs or attachments:

- Notify users.

If URLs present:

- Perform URL reputation checks.

If attachments present:

- Conduct sandbox file analysis.

Perform remediation if confirmed malicious.

---

## CVE Patching Playbook

SOC vulnerability management workflow:

1. Monitor vulnerability advisories.
2. Extract CVE information.
3. Check asset exposure.
4. Assess risk severity.
5. Create patching ticket.
6. Test patch before deployment.
7. Deploy patch to production systems.

Helps prevent vulnerability backlog accumulation.

---

## Threat Intelligence Workflow Practical

### Scenario

Large breach investigation delays occurred due to manual investigation workflows.

### Solution

Implemented SOAR automation workflow.

### Actions Completed

- Configured automated investigation flow
- Enabled manual and automated workflow settings
- Activated required workflow components
- Tested workflow execution
- Achieved successful workflow transition

---

### Flag Received

