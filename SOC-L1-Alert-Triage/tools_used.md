Tools and Commands Used

Room: SOC Alert Triage
Platform: TryHackMe

Tools Used in This Room
1. SIEM (Security Information and Event Management)

Purpose:
Centralized log collection, correlation, and alert generation.

How It Is Used in SOC Context:

Aggregates logs from endpoints, servers, and network devices

Applies detection rules to generate alerts

Provides alert dashboard for SOC analysts

Enables log investigation and correlation

Used in This Room:

Reviewing alert queue

Investigating alert fields (user, host, IP, process, file)

Checking surrounding events

Classifying alerts

Example Platforms:

Splunk

Elastic

2. EDR (Endpoint Detection and Response)

Purpose:
Monitors endpoint-level activity such as processes, file execution, and suspicious behavior.

How It Is Used in SOC Context:

Detects malware execution

Tracks process trees

Monitors suspicious command-line activity

Supports endpoint-level investigation

Used in This Room (Conceptually):

Investigating process execution

Reviewing file creation events

Analyzing suspicious downloads

Example Platforms:

Microsoft Defender for Endpoint

CrowdStrike

3. SOAR (Security Orchestration, Automation, and Response)

Purpose:
Automates alert handling and response workflows.

How It Is Used in SOC Context:

Executes predefined playbooks

Automates repetitive triage steps

Integrates multiple security tools

Used in This Room (Conceptual Understanding):

Understanding alert workflow automation

Workbook / playbook reference

Example Platforms:

Splunk SOAR

Cortex SOAR

4. ITSM / Ticketing System

Purpose:
Manages alert ownership and investigation tracking.

How It Is Used in SOC Context:

Assign alerts to analysts

Track alert status

Maintain documentation

Used in This Room:

Assigning alerts

Moving alerts between statuses

Closing alerts

Example Platforms:

Jira

TheHive

SOC Dashboard Actions Practiced

This room was investigation-based rather than command-line based.

Alert Management Actions

assign alert to yourself
move alert to “In Progress”
review alert name and description
identify alert severity
filter alerts by status
prioritize alerts (Critical → High → Medium → Low)
sort alerts by time (Oldest first)
set alert verdict (True Positive / False Positive)
add structured investigation comment
move alert to “Closed”

Investigation Actions

identify affected user
identify affected host
analyze suspicious login activity
review file creation details
analyze process execution
check suspicious domain or URL
review surrounding logs (before and after event)
validate file hash reputation
validate IP address reputation
determine if escalation to L2 is required

Commands Used

This room did not require terminal-based commands.
All actions were performed within a simulated SOC dashboard environment.

However, the investigation logic aligns with real-world commands such as:

Example (Real SOC Context – Not executed in this lab):

# Search logs for a specific user
index=security_logs user="username"

# Search logs for suspicious IP
index=security_logs src_ip="x.x.x.x"

# Search for file hash
index=security_logs file_hash="hash_value"

These represent how similar investigations would be performed in platforms like Splunk.

Practical Tools Knowledge Gained

Understanding SIEM-based alert investigation

Alert prioritization logic

Indicator-based analysis

Detection rule interpretation

Structured documentation workflow

Escalation decision-making in SOC operations
