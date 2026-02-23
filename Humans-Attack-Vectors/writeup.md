Room: Human Element in Cyber Security
Platform

TryHackMe

Overview

This room focused on understanding how attackers target the human element using social engineering techniques such as phishing, malware delivery, impersonation, and deepfakes. It also explained the role of SOC analysts in detecting and investigating human-targeted attacks, and the importance of mitigation strategies such as anti-phishing tools, endpoint protection, and security awareness training. The room included a practical SOC dashboard simulation where employees at risk were investigated and security policies were improved.

Key Concepts Learned
Human Element as the Weakest Link

Humans are the most vulnerable part of cybersecurity systems

Attackers exploit human psychology instead of technical vulnerabilities

Human errors can lead to credential theft, malware infections, and system compromise

Social engineering is the primary method used to target humans

Social Engineering

Social engineering is the manipulation of individuals to perform actions that compromise security

It exploits trust, urgency, fear, and curiosity

Attackers pretend to be trusted entities such as IT staff, executives, or government organizations

Goal is to steal credentials, install malware, or gain unauthorized access

Phishing Attacks

Phishing is the most common social engineering attack

Attackers send fake emails with malicious links or attachments

Fake login pages are used to steal credentials

Malicious attachments can install malware

Indicators include fake sender addresses, suspicious links, and urgent language

Example attack flow:

User receives phishing email

User clicks malicious link

User enters credentials on fake website

Attacker steals credentials

Malware Delivery Attacks

Malware is often disguised as legitimate software updates or downloads

Fake websites and fake software updates trick users into installing malware

Malware types include data stealers, keyloggers, ransomware, and remote access trojans

Malware allows attackers to steal data and gain system control

Fake CAPTCHA and Malicious Websites

Fake CAPTCHA pages trick users into executing malicious commands

Fake browser update websites install malware instead of legitimate updates

Attackers use SEO poisoning and fake websites to deliver malware

Deepfake Attacks

Deepfakes use AI-generated audio or video to impersonate trusted individuals

Attackers impersonate executives or colleagues

Used for financial fraud and credential theft

Impersonation Attacks

Attackers pretend to be IT support, HR, or executives

Victims are tricked into providing credentials or installing malware

Often conducted through phone calls or emails

Mitigation vs Detection

Mitigation:

Focuses on preventing attacks before they succeed

Includes anti-phishing tools, antivirus, and employee training

Reduces attack success rate

Detection:

Focuses on identifying attacks that bypass mitigation

SOC analysts detect suspicious activity and investigate incidents

SOC acts as the last line of defense

Mitigation Measures

Anti-phishing solutions:

Block phishing emails before reaching users

Antivirus / EDR solutions:

Detect and block malware on endpoints

Security awareness training:

Educate employees to recognize phishing and attacks

Trust but verify principle:

Employees verify suspicious requests before taking action

Role of SOC Analyst

SOC analysts are responsible for:

Monitoring security alerts

Detecting phishing and malware incidents

Investigating suspicious activity

Responding to security incidents

Protecting employees and organizational systems

SOC analysts also collaborate with IT, HR, and security teams.

SOC Dashboard Investigation Simulation

SOC analysts performed tasks such as:

Investigating employees at risk

Identifying compromised accounts

Detecting attack indicators

Improving security policies

Implementing mitigation measures

Tools and Systems Discussed
SIEM (Security Information and Event Management)

Purpose:

Detect suspicious activity

Monitor logs

Generate alerts

Examples:

Splunk

Microsoft Sentinel

IBM QRadar

EDR (Endpoint Detection and Response)

Purpose:

Detect malware on endpoints

Monitor endpoint activity

Prevent malware execution

Examples:

Microsoft Defender

CrowdStrike

SentinelOne

Anti-Phishing Tools

Purpose:

Block phishing emails

Prevent credential theft

Security Awareness Training Platforms

Purpose:

Train employees to detect phishing attacks

Improve security awareness

SOC Monitoring Dashboards

Purpose:

Investigate employees at risk

Monitor incidents

Improve security posture

Commands Practiced

This room focused on SOC investigation using dashboards and security tools rather than command-line interfaces.

Common SOC investigation actions included:

monitor security alerts
investigate suspicious user activity
identify phishing indicators
detect malware infections
analyze compromised accounts
implement mitigation measures
improve security policies
Skills Developed

Understanding social engineering attacks

Phishing detection and analysis

Malware delivery techniques

SOC investigation workflow

Incident detection and response

Security mitigation strategies

Human risk analysis in cybersecurity

SOC dashboard investigation and analysis
