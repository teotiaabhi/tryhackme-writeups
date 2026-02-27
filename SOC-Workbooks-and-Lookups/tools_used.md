Tools & Commands Notes

Room: SOC Fundamentals – Identity, Asset & Workbook-Based Investigation
Platform: TryHackMe

🧰 1️⃣ Identity Inventory Systems
🔹 Active Directory (AD)

Purpose:
Centralized identity and asset management system.

Used In This Room For:

Searching user accounts (G.Baker, R.Lund)

Verifying job role

Checking group membership

Validating access privileges

Typical SOC Actions:

Lookup user role

Check department

Review last login

Validate account status (enabled/disabled)

Why It Matters:
Helps determine whether activity aligns with job responsibilities.

🔹 BambooHR (HR Identity Source)

Purpose:
HR-based employee information system.

Used In This Room For:

Confirming expected working location

Validating employment status

Reviewing role and manager details

SOC Use Case:
If login from unusual location → check if employee is traveling.

🧰 2️⃣ Asset Inventory Systems
🔹 Active Directory (Computer Objects)

Purpose:
Stores server and workstation objects.

Used For:

Checking hostname ownership

Identifying server purpose

Confirming subnet mapping

Example:
HQ-FINFS-02 → Finance File Server

🔹 SIEM / EDR Asset Lookup

Examples:

Splunk

Elastic

CrowdStrike

Purpose:
Collect host telemetry and metadata.

Used In This Room For:

Identifying internal IP assignment

Mapping IP to subnet

Reviewing endpoint behavior

🧰 3️⃣ SIEM Platform (Example: Splunk)

Purpose:
Centralized log analysis.

Used In This Room For:

Reviewing login events

Analyzing firewall logs

Correlating VPN activity

Tracking subnet scans

💻 Example SOC Search Actions (Splunk-style)
Investigate VPN Login
index=vpn_logs username="G.Baker"

Searches for VPN login events for the user.

Investigate Internal IP Activity
index=firewall_logs src_ip=10.10.0.53

Finds activity performed by internal VPN-assigned IP.

Check Subnet Scanning
index=firewall_logs src_ip=10.10.0.53 dest_ip=172.16.*

Identifies lateral movement attempts.

🧰 4️⃣ Threat Intelligence (TI) Platforms

Examples:

VirusTotal

AbuseIPDB

Internal TI Database

Purpose:
Check IP/domain/file reputation.

Used In This Room For:

Checking 103.61.240.174 reputation

Identifying malicious indicators

SOC Action:
Determine if external IP is known attacker.

🧰 5️⃣ Email Analysis Tools
🔹 EML Analyzer

Purpose:
Analyzes raw email headers and metadata.

Used For:

SPF validation

DKIM verification

Sender domain reputation

Mail routing path

SOC Investigation Step:

Confirm if email spoofed

Check authentication failures

🔹 Sandbox (For Attachment Analysis)

Purpose:
Safely execute suspicious files.

Used For:

Running binary attachments

Observing malicious behavior

Extracting IOCs

Typical Output:

File hash

Network connections

Registry changes

Dropped files

🧰 6️⃣ Network Diagram Usage

Not a tool but critical investigation resource.

Used For:

Understanding subnet layout

Identifying VPN subnet (10.10.0.0/16)

Identifying Database subnet (172.16.15.0/24)

Identifying Office subnet (172.16.23.0/24)

Reconstructing attack path

🧠 Commands / Actions Practiced (Dashboard-Based)

Since this room is mostly conceptual, actions included:

Search user in identity inventory

Search host in asset inventory

Review firewall logs

Analyze VPN login events

Investigate email headers

Run file in sandbox

Review SIEM correlation results

Write alert report

Escalate to L2

📋 Alert Handling Actions Practiced

Move alert to “In Progress”

Perform enrichment

Validate business logic

Collect evidence

Write 5W report

Set verdict

Escalate or Close

🎯 Technical Concepts Practiced Through Tools

VPN brute force detection

Internal reconnaissance detection

Lateral movement identification

Identity validation

Asset sensitivity classification

Email authentication analysis

Structured triage workflow

🔥 Most Important Skill From Tools Section

The key skill was NOT using commands.

The key skill was:

Correlating identity + asset + network + logs before making a verdict.

This is core SOC L1 behavior.
