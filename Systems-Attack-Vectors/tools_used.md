Tools and Systems Discussed

This room focused on SOC monitoring, vulnerability management, endpoint protection, and remediation planning to protect systems from attacks.

SIEM (Security Information and Event Management)

Purpose:

Monitor system logs and detect suspicious activity

Identify exploit attempts and compromised systems

Generate alerts for SOC investigation

Examples:

Splunk

Microsoft Sentinel

IBM QRadar

Common investigation queries (example format):

index=system_logs
event_type="authentication_failure"
source_ip="suspicious_ip"
action="privilege_escalation"
EDR (Endpoint Detection and Response)

Purpose:

Monitor endpoints for malware and suspicious activity

Detect exploit attempts and malicious processes

Isolate compromised systems

Examples:

Microsoft Defender for Endpoint

CrowdStrike Falcon

SentinelOne

Common SOC actions:

check endpoint security status
analyze suspicious process
isolate compromised host
detect malware execution
Vulnerability Scanning Tools

Purpose:

Identify vulnerable and outdated systems

Detect exposed services and weak configurations

Examples:

Nessus

OpenVAS

Qualys

Common scanning actions:

scan system for vulnerabilities
identify outdated software
detect exposed services
generate vulnerability report
Patch Management Systems

Purpose:

Apply software updates to fix vulnerabilities

Reduce attack surface

Examples:

Windows Update

WSUS (Windows Server Update Services)

Linux package managers

Common patching actions:

check patch status
install security updates
verify patch installation
update vulnerable system
Network Protection Tools (Firewall / Access Control)

Purpose:

Restrict unauthorized access

Protect systems from external attacks

Examples:

Firewall

Network Access Control (NAC)

Common protection actions:

block unauthorized IP address
restrict access to trusted networks
monitor network traffic
detect unauthorized connection
Antivirus / Endpoint Protection Tools

Purpose:

Detect and prevent malware infections

Protect endpoint systems

Examples:

Microsoft Defender

CrowdStrike

SentinelOne

Common protection actions:

scan system for malware
detect malicious file
quarantine infected file
remove malware threat
Commands Practiced (SOC Investigation and Response Actions)

These represent common SOC analyst investigation actions practiced in this room:

monitor systems at risk
investigate vulnerability alerts
detect misconfigured systems
analyze exploit attempts
identify compromised systems
apply remediation measures
implement patch management
