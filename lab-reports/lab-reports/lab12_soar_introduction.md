# Lab 12 — Security Orchestration Automation and Response (SOAR) Investigation Workflow

Platform: TryHackMe  
Room: Introduction to SOAR  
Role Simulation: SOC Analyst Level 1 — Automation & Incident Response Operations

---

## Objective

Understand how Security Orchestration, Automation, and Response (SOAR) platforms improve SOC efficiency by automating investigations, coordinating multiple security tools, and enabling faster incident response through predefined workflows known as playbooks.

---

## Technologies and Concepts Used

- SOAR Platform Workflow Interface
- Security Playbooks
- Threat Intelligence Integration
- Case Management Automation
- Incident Ticketing Systems
- SOC Workflow Automation

---

## Key Concepts Reviewed

### Security Orchestration

Integration of multiple SOC tools into a unified platform.

Examples:

- SIEM
- Threat Intelligence Platforms
- Firewall Controls
- IAM Systems
- Ticketing Systems

Purpose:

Reduce manual tool switching during investigations.

---

### Automation

Predefined workflows automatically execute investigation tasks.

Examples:

- Query SIEM logs
- Perform IP reputation checks
- Validate login activity
- Create investigation tickets

Automation reduces analyst workload and speeds response time.

---

### Response

SOAR platforms automatically perform containment actions including:

- Blocking malicious IP addresses
- Disabling compromised accounts
- Sending investigation notifications

---

## Tasks Completed

---

### Task 1 — Introduction to SOAR

Reviewed SOC operational challenges including:

- Alert fatigue
- Manual investigation processes
- Communication delays
- Multi-tool investigation complexity

Learned how SOAR improves SOC efficiency through automation.

---

### Task 2 — Traditional SOC Workflow

Studied core SOC responsibilities:

- Monitoring and Detection using SIEM
- Incident Response and Remediation
- Threat Intelligence consumption
- Cross-team communication workflows

Examples Observed:

- Failed login monitoring
- Suspicious login detection
- Endpoint containment actions

---

### Task 3 — Understanding SOAR Concepts

Learned three SOAR pillars:

1. Orchestration — tool coordination.
2. Automation — workflow execution.
3. Response — containment actions.

Observed unified investigation workflow inside SOAR interface.

---

### Task 4 — Building SOAR Playbooks

Reviewed automated playbook workflows.

Examples studied:

---

#### VPN Brute Force Investigation Playbook

Workflow:

1. Receive alert from SIEM.
2. Check historical login behaviour.
3. Verify IP reputation using threat intelligence.
4. Query successful login attempts.
5. Escalate containment actions if required.

Outcome:

Standardised investigation workflow.

---

#### Phishing Investigation Playbook

Workflow:

1. Suspicious email received.
2. Investigation ticket created.
3. Check email attachments or URLs.

Decision Handling:

If no malicious indicators:

- Notify affected users.

If URLs detected:

- Perform reputation lookup.

If attachments detected:

- Sandbox file analysis.

Remediation actions applied if malicious.

---

#### CVE Patching Playbook

Vulnerability management automation workflow:

1. Monitor CVE advisories.
2. Extract vulnerability information.
3. Assess asset exposure.
4. Evaluate risk severity.
5. Create patching ticket.
6. Test patch deployment.
7. Deploy patch to production systems.

Outcome:

Reduced vulnerability backlog.

---

### Task 5 — Threat Intelligence Workflow Practical

Scenario:

SOC breach investigation delays caused by manual investigation processes.

Objective:

Implement automated threat intelligence workflow using SOAR.

Actions Performed:

- Configured automated investigation workflow.
- Enabled manual and automated execution modes.
- Activated workflow components.
- Tested automation flow execution.

Result:

Successful automated workflow transition achieved.

---

### Investigation Result

Flag Captured:

THM{AUTOM@T1N6_S3CUR1TY}


---

### Task 6 — Conclusion

Understood how SOAR enhances SOC operations through:

- Automated investigations
- Tool orchestration
- Incident tracking
- Faster containment actions

Observed significant reduction in manual analyst workload.

---

## SOC Skills Practiced

- Incident workflow automation
- Playbook analysis and understanding
- Threat intelligence integration
- SOC orchestration workflow design
- Incident response lifecycle improvement
- Case management workflow tracking

---

## SOC Tools Simulated

- SOAR Automation Interface
- SIEM Platform
- Threat Intelligence Platforms
- Firewall Controls
- IAM Systems
- Ticketing Systems

---

## Key Learning

SOAR platforms significantly improve SOC efficiency by automating repetitive investigation tasks, coordinating multiple security tools, and enabling faster incident response while reducing analyst fatigue.

---

## Evidence

Screenshots captured during:

- Playbook review
- Workflow configuration
- Threat intelligence automation testing
- Successful workflow execution

Location:

screenshots/

---
