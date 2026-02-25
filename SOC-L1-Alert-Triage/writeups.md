Room: SOC Alert Triage

Platform: TryHackMe

Overview

This room focused on understanding how security alerts are generated, prioritised, and handled within a Security Operations Center (SOC). It covered the complete alert lifecycle — from event logging to alert creation, prioritisation, triage workflow, investigation methodology, verdict classification, and escalation process.

The module emphasized structured thinking, evidence-based investigation, and operational discipline required for SOC L1 analysts.

Key Concepts Learned
1. Event to Alert Lifecycle
Event

An activity occurring within an environment, such as:

User login

Process execution

File download

Network connection attempt

Log

System-generated record of an event

Produced by OS, firewall, cloud platform, or application

Detection Rule

Predefined logic inside SIEM/EDR

Triggers when suspicious pattern matches log data

Alert

Notification generated when a detection rule is triggered

Reduces millions of logs into actionable security signals

Flow:

Event → Log → Detection Rule → Alert

2. Alert Properties

Understanding alert fields is critical for triage.

Alert Time

Time when alert was generated

May differ from event time

Alert Name

Detection rule title

Summarizes suspicious activity

Examples:

Unusual VPN Login Location

Double Extension File Creation

Potential Data Exfiltration

Alert Severity

Indicates urgency:

Low

Medium

High

Critical

Severity is initially defined by detection engineers.

Alert Status

New

In Progress

Closed

Awaiting Action

Alert Verdict

Final classification after investigation:

True Positive (real threat)

False Positive (benign activity)

Alert Assignee

Analyst responsible for investigation

Ensures accountability

Alert Description

Contains:

Detection logic

Risk explanation

Optional investigation guidance

Alert Fields (Indicators)

Examples:

Username

Hostname

IP address

Process name

File path

Hash value

URL

These are primary investigation data points.

3. Alert Prioritisation

When multiple alerts exist, prioritisation is essential.

Step 1: Filter Alerts

Only investigate:

New

Unassigned

Awaiting action

Do not take:

Closed

Already in progress

Step 2: Sort by Severity

Priority order:

Critical

High

Medium

Low

Step 3: Sort by Time

If severity is equal:

Investigate oldest alert first

Prioritisation Logic:

Severity > Time > Ownership

4. Alert Triage Workflow

Alert triage is a structured investigation process.

Phase 1: Initial Actions

Assign alert to yourself

Move alert to “In Progress”

Review alert name and description

Identify key indicators (user, host, IP, file, process)

Purpose:
Establish ownership and prepare for investigation.

Phase 2: Investigation
Identify the Entity at Risk

Affected user

Hostname

Privilege level

Business impact

Understand the Activity

Determine whether alert relates to:

Suspicious login

Malware execution

Phishing

Data exfiltration

Lateral movement

Review Surrounding Events

Analyze:

Activity before alert

Activity after alert

Related authentication attempts

Additional file/process activity

Alerts rarely occur in isolation.

Use Threat Intelligence

Validate:

File hash reputation

IP reputation

Domain reputation

Phase 3: Final Decision

Classify the alert based on evidence.

False Positive

Legitimate user behavior

Corporate VPN usage

Approved administrative activity

No malicious follow-up activity

True Positive

Confirmed malware

Credential dumping tools

Suspicious login followed by data access

Unauthorized data transfer

5. Escalation Logic

Escalate to L2 when:

Confirmed compromise

Privileged account affected

Advanced attack techniques observed

Remediation exceeds L1 scope

6. Closing the Alert

Final required steps:

Set final verdict

Add structured investigation comment

Move alert to Closed status

Proper documentation ensures:

Audit trail

Knowledge transfer

SOC quality assurance

Tools and Systems Discussed
SIEM (Security Information and Event Management)

Purpose:

Log aggregation

Correlation and detection

Centralized alert management

SOC Usage:

Investigate logs

Correlate events

Validate suspicious activity

Examples:

Splunk

Elastic

EDR (Endpoint Detection and Response)

Purpose:

Monitor endpoint activity

Detect malicious processes

SOC Usage:

Analyze process execution

Investigate malware alerts

Examples:

Microsoft Defender

CrowdStrike

SOAR (Security Orchestration, Automation and Response)

Purpose:

Automate alert handling

Execute playbooks

SOC Usage:

Reduce manual workload

Standardize response actions

Examples:

Splunk SOAR

Cortex SOAR

ITSM / Ticketing Systems

Purpose:

Track alert ownership

Document investigation

SOC Usage:

Manage workflow

Assign analysts

Maintain accountability

Examples:

Jira

TheHive

Commands / Actions Practiced

This room was SOC dashboard–based.

Investigation Actions Practiced:

assign alert to analyst
move alert to “In Progress”
review alert description
identify affected user
identify affected host
analyze alert logs
review surrounding activity
validate indicators using threat intelligence
classify alert (True / False Positive)
add investigation notes
close alert

Skills Developed

Alert prioritisation based on severity and time

Structured alert triage workflow

Evidence-based decision making

Detection logic interpretation

Log correlation analysis

Indicator validation

Threat classification (True vs False Positive)

Escalation judgment

Professional SOC documentation practices

Operational discipline in SIEM environments
