Tools and Systems Discussed

This room focused on SOC investigation, phishing detection, malware prevention, and mitigation tools used to protect employees and detect human-targeted attacks.

SIEM (Security Information and Event Management)

Purpose:

Monitor security events and alerts

Detect suspicious user activity

Identify compromised accounts

Investigate phishing and malware incidents

Examples:

Splunk

Microsoft Sentinel

IBM QRadar

Common SOC investigation queries (example format):

index=email_logs
event_type="phishing"
user="employee_name"
action="login_failed"
EDR (Endpoint Detection and Response)

Purpose:

Monitor endpoint devices

Detect malware infections

Identify malicious processes

Investigate compromised endpoints

Examples:

Microsoft Defender for Endpoint

CrowdStrike Falcon

SentinelOne

Common investigation actions:

check endpoint status
analyze suspicious process
isolate infected host
detect malware execution
Anti-Phishing Solutions

Purpose:

Detect and block phishing emails

Prevent credential theft

Protect employees from malicious email attacks

Common detection actions:

scan email for malicious links
detect suspicious sender domain
block phishing email
analyze email attachment
Antivirus / Malware Protection Tools

Purpose:

Detect and block malware

Prevent malicious software execution

Protect endpoint systems

Common actions:

scan system for malware
detect malicious file
quarantine infected file
remove malware
SOC Monitoring Dashboard

Purpose:

Monitor employees at risk

Investigate security incidents

Detect compromised accounts

Improve security policies

Common SOC investigation actions:

investigate employee activity
identify compromised user
analyze attack indicators
respond to security incident
Security Awareness and Mitigation Systems

Purpose:

Prevent social engineering attacks

Improve employee security awareness

Reduce phishing success rate

Common mitigation actions:

enable anti-phishing protection
implement security policy
improve endpoint protection
apply mitigation controls
Commands Practiced (SOC Investigation Actions)

These represent common SOC analyst investigation and response actions practiced in this room:

monitor security alerts
investigate phishing incident
detect compromised account
analyze suspicious login activity
identify malware infection
apply mitigation measures
improve organizational security posture

Note: This room focused on SOC workflows using security dashboards and defensive tools rather than traditional Linux terminal commands.
