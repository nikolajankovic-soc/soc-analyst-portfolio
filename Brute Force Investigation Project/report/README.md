# Brute Force Investigation
This folder contains the report, screenshots, and IOCs for the SOC investigation of the LetsDefend `SOC176 - RDP Brute Force Detected` alert.
SOC176 - RDP Brute Force Detected
Project Overview
This project documents a SOC investigation of the LetsDefend `SOC176 - RDP Brute Force Detected` alert. The case demonstrates SIEM alert triage, log filtering, authentication-event analysis, threat intelligence enrichment, endpoint investigation, MITRE ATT&CK mapping, and remediation recommendations.
Scenario
A brute-force RDP attack targeted host `Matthew` (`172.16.17\\\\\\\[.]148`) from external IP `218.92.0\\\\\\\[.]56`. Repeated failed login attempts were followed by a successful authentication, making the alert a true positive.
Skills Demonstrated
SIEM alert triage
Windows authentication log analysis
Failed login analysis with Event ID 4625
Successful login validation with Event ID 4624
RDP / TCP 3389 investigation
Source IP reputation enrichment
Endpoint security review
MITRE ATT&CK mapping
Incident escalation and remediation planning
Key Findings
Source IP: `218.92.0\\\\\\\[.]56`
Target host: `Matthew`
Target IP: `172.16.17\\\\\\\[.]148`
Protocol: RDP / TCP 3389
Multiple failed login attempts were observed
Successful login occurred after failed attempts
Post-authentication discovery activity was observed
Final assessment: True Positive
.
Defensive Recommendations
Isolate affected endpoint
Reset affected credentials
Enable MFA for RDP / remote access
Implement account lockout policy
Restrict RDP exposure to VPN or approved IP ranges
Tune SIEM alerts for repeated 4625 events followed by 4624 success
MITRE ATT&CK
T1110 - Brute Force
T1078 - Valid Accounts
T1021.001 - Remote Services: RDP
T1033 - System Owner/User Discovery
T1087.001 - Account Discovery: Local Account
T1069.001 - Permission Groups Discovery: Local Groups
T1049 - System Network Connections Discovery
