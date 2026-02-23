Tools and Systems Discussed

This room introduced core defensive security tools used by SOC teams to monitor, detect, and respond to cyber threats.

SIEM (Security Information and Event Management)

Purpose:

Collects and analyzes logs from multiple systems

Detects suspicious activity

Generates security alerts

Examples:

Splunk

Microsoft Sentinel

IBM QRadar

Common actions performed:

Search logs

Investigate alerts

Monitor suspicious events

Example query syntax (generic SIEM format):

index=security_logs
source="firewall"
event_type="failed_login"
user="admin"
EDR (Endpoint Detection and Response)

Purpose:

Monitors endpoint devices (computers, servers)

Detects malware and suspicious processes

Responds to threats on endpoints

Examples:

CrowdStrike Falcon

Microsoft Defender for Endpoint

Common investigation actions:

Check running processes

Investigate suspicious files

Analyze endpoint activity

Example investigation commands (conceptual):

check process list
analyze suspicious executable
isolate infected endpoint
Log Monitoring Systems

Purpose:

Analyze system and application logs

Identify suspicious activity

Common log sources:

Windows Event Logs

Firewall logs

Authentication logs

Example investigation focus:

failed login attempts
unauthorized access attempts
unusual system activity
Vulnerability Assessment Tools

Purpose:

Identify security vulnerabilities in systems and applications

Used by:

Penetration Testers

Security Engineers

Common tasks:

scan system for vulnerabilities
identify outdated software
detect security misconfigurations
Incident Response and Threat Intelligence Platforms

Purpose:

Analyze attacker behavior

Investigate threat actors

Respond to cyber incidents

Used by:

Threat Intelligence Analysts

Incident Response Teams

Common investigation actions:

analyze threat indicators
investigate attack patterns
track attacker activity
SOC Analyst Core Investigation Actions Practiced

These actions represent typical SOC analyst tasks:

monitor SIEM alerts
triage security alerts
investigate suspicious events
escalate confirmed incidents
analyze system logs
identify malicious activity
Important Note

This room focuses on SOC workflow and concepts, not Linux terminal commands. Most actions are performed inside security tools (SIEM, EDR, dashboards), not traditional command-line interfaces.
