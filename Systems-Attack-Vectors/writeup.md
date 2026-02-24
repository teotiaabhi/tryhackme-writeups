Room: Systems as Attack Vectors
Platform

TryHackMe

Overview

This room focused on understanding how attackers target systems such as servers, databases, endpoints, and cloud infrastructure to gain unauthorized access. It covered key attack vectors including weak passwords, software vulnerabilities, misconfigurations, and supply chain attacks. The room also explained how SOC analysts detect compromised systems and apply mitigation strategies such as patch management, antivirus protection, secure configuration, and network access controls. A hands-on SOC dashboard simulation was included to analyze systems at risk and implement remediation plans.

Key Concepts Learned
Systems as Critical Attack Targets

A system is any device or infrastructure component that stores or processes data

Examples include servers, virtual machines, cloud platforms, databases, and laptops

Compromising a system provides attackers with access to sensitive data and internal infrastructure

System compromise can affect multiple users and services

Initial Access Phase

The first goal of attackers is to gain access to a target system

Once inside, attackers can steal data, install malware, deploy ransomware, or escalate privileges

Initial access is a critical stage in cyber attacks

Human-Led System Attacks

Human mistakes often lead to system compromise

Weak passwords and password reuse allow attackers to gain access

Malicious USB devices like Rubber Ducky can execute malware automatically

81% of breaches involve stolen or weak passwords

Example:
Weak password reuse can allow attackers to access accounts easily.

Software Vulnerabilities

Vulnerabilities are weaknesses in software that attackers exploit

Every software triggering software vulnerabilities include operating systems, applications, and servers

Zero-day vulnerabilities are unknown vulnerabilities exploited before patches are released

CVE (Common Vulnerabilities and Exposures) is a unique identifier assigned to vulnerabilities

Examples:
CVE-2017-0144 (EternalBlue)
CVE-2021-34527 (PrintNightmare)

Patch management fixes vulnerabilities and protects systems

Misconfigurations

Misconfiguration is an incorrect system setup that creates security risks

Misconfigurations are caused by human errors, not software bugs

Examples:

Weak passwords

Disabled firewalls

Exposed databases

Open cloud storage access

Misconfigured systems can be easily accessed by attackers.

Supply Chain Attacks

Supply chain attacks target trusted software vendors or libraries

Attackers compromise software updates and distribute malware to users

Supply chain attacks can affect thousands of systems simultaneously

Examples:
SolarWinds attack
3CX attack

Supply chain attacks are difficult to prevent and require SOC detection.

Patch Management

Patch management involves updating systems to fix vulnerabilities

Applying patches reduces risk of exploitation

Unpatched systems remain vulnerable to attacks

Network Protection

Restricting access to systems prevents unauthorized access

Firewalls and access controls protect systems

Limiting access to trusted IP addresses improves security

Antivirus and Endpoint Protection

Antivirus and EDR detect and prevent malware infections

These tools monitor system activity and detect malicious behavior

Endpoint protection reduces system compromise risk

Examples:
Microsoft Defender
CrowdStrike
SentinelOne

Role of SOC Analyst in Protecting Systems

SOC analysts are responsible for:

Monitoring system activity

Detecting suspicious behavior

Investigating security alerts

Identifying compromised systems

Responding to security incidents

Recommending mitigation measures

SOC analysts use SIEM, EDR, and log monitoring tools.

Mitigation vs Detection

Mitigation:

Prevents attacks before they occur

Includes patch management, antivirus, and secure configuration

Detection:

Identifies attacks that bypass mitigation

SOC analysts investigate and respond to incidents

SOC acts as the last line of defense.

Tools and Systems Discussed
SIEM (Security Information and Event Management)

Purpose:

Monitor logs and detect suspicious activity

Generate security alerts

Examples:

Splunk

Microsoft Sentinel

IBM QRadar

EDR (Endpoint Detection and Response)

Purpose:

Detect malware and suspicious activity on endpoints

Monitor system behavior

Examples:

CrowdStrike

Microsoft Defender

SentinelOne

Antivirus Protection

Purpose:

Detect and prevent malware execution

Protect endpoint systems

Patch Management Systems

Purpose:

Update software to fix vulnerabilities

Reduce attack surface

Network Protection Tools

Purpose:

Restrict system access

Prevent unauthorized connections

Examples:

Firewalls

Access control systems

SOC Monitoring Dashboard

Purpose:

Identify systems at risk

Investigate compromised systems

Implement remediation plans

Commands Practiced

This room focused on SOC investigation and system protection using security tools and dashboards rather than traditional command-line commands.

SOC investigation actions included:

monitor system activity
investigate compromised systems
detect vulnerability exploitation
identify misconfigured systems
analyze malware activity
implement remediation measures
apply patch management
Skills Developed

Understanding system attack vectors

Vulnerability and CVE awareness

Misconfiguration detection and prevention

Supply chain attack awareness

System security monitoring

Incident detection and response

SOC investigation workflow

Remediation planning and mitigation
