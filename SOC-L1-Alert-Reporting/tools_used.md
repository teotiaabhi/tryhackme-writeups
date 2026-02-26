Tools and Commands Used

Room: SOC Reporting, Escalation & Communication
Platform: TryHackMe

Tools Used in This Room
1. SIEM (Security Information and Event Management)

Purpose:
Centralized log collection, correlation, and alert generation.

How It Is Used in SOC Context:

Receives alerts for L1 triage

Displays alert properties (severity, status, verdict, assignee)

Allows analysts to review logs and indicators

Enables alert documentation and escalation

Used in This Room:

Reviewing alert details

Writing structured 5W reports

Setting verdict (True/False Positive)

Reassigning alert to L2

Moving alert between statuses

Example Platforms:

Splunk

Elastic

2. EDR (Endpoint Detection and Response)

Purpose:
Monitors endpoint-level activity such as process execution, parent-child process relationships, and command-line behavior.

How It Is Used in SOC Context:

Analyze suspicious processes

Investigate command execution

Detect reverse shells or malware

Used in This Room (Conceptual Investigation):

Reviewing process tree

Identifying suspicious parent process (e.g., web server spawning reverse shell)

Detecting domain discovery commands

Example Platforms:

Microsoft Defender for Endpoint

CrowdStrike

3. ITSM / Ticket Management System

Purpose:
Tracks investigation ownership, documentation, and escalation workflow.

How It Is Used in SOC Context:

Assign alerts to analysts

Maintain investigation history

Escalate tickets to L2

Preserve long-term records

Used in This Room:

Assigning alert to L2

Saving structured report

Managing alert lifecycle

Example Platforms:

Jira

TheHive

4. Corporate Communication Tools (Operational Context)

Purpose:
Facilitate communication between SOC analysts and other departments.

How It Is Used in SOC Context:

Notify L2 of escalated alerts

Request clarification from IT/HR

Coordinate containment actions

Examples:

Internal chat systems

Email

Incident communication platforms

SOC Dashboard Actions Practiced

This room focused on operational workflow rather than command-line execution.

Alert Handling Actions

filter alerts by status
prioritize alerts by severity
assign alert to yourself
move alert to “In Progress”
review alert description
analyze affected user and host
review process execution chain
identify suspicious commands
write structured 5W report
set verdict (True Positive / False Positive)
reassign alert to L2
save and close alert

Investigation Actions Practiced

identify domain discovery activity
analyze command execution (whoami, net group, nltest)
review process hierarchy (parent-child-grandparent)
identify reverse shell behavior
validate authentication failures (SPF/DKIM in phishing scenario)
assess business impact
determine escalation requirement

Command-Line Context (Real-World Equivalent Examples)

Although this room was dashboard-based, the investigation aligns with commands commonly used in real environments:

Example – Log search in SIEM:

index=security_logs user="username"
index=security_logs host="hostname"
index=security_logs process_name="cmd.exe"

Example – Searching for specific command execution:

index=security_logs command_line="whoami"
index=security_logs command_line="nltest"

Example – Filtering phishing email indicators:

index=email_logs sender="support@microsoft.com"
index=email_logs spf_result="fail"
Practical Tool Competencies Gained

SIEM-based alert investigation

Process tree analysis

Escalation workflow management

Structured SOC documentation

Threat indicator validation

Operational communication awareness
