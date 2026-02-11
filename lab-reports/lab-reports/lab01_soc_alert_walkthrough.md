Lab 01 — SOC Alert Investigation Walkthrough

 Platform Used:
TryHackMe  
Scenario Used:
Alert Investigation Walkthrough  
Alert Summary:
Critical SIEM alert indicating multiple failed SSH login attempts followed by a successful login attempt from the same IP address.

Data Sources Used:
- SIEM alert dashboard  
- Authentication alert logs  
- IP reputation lookup tool  
- Firewall block panel  

Investigation Steps:
- Alert severity and message were checked  
- Multiple failed login attempts were identified  
- Successful login attempt was identified  
- IP was checked via IP reputation lookup tool  
- IP was confirmed to be malicious  
- SOC lead was notified  
- IP was blocked via firewall  

Detection Indicators:
- Brute force login  
- Multiple failed login attempts from the same IP  
- Successful login after failed login attempts  

MITRE ATT&CK:
T1110 — Brute Force  
Outcome:
Incident was escalated, and IP was blocked to prevent future login attempts.
