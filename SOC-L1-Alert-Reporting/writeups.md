Room: SOC Reporting, Escalation & Communication

Platform: TryHackMe

Overview

This room covered the post-triage workflow within a Security Operations Center (SOC), focusing on alert reporting, escalation procedures, and cross-team communication. It emphasized the importance of structured documentation, evidence preservation, and proper handover to L2 analysts for deeper investigation and remediation.

The module demonstrated how L1 triage supports efficient incident response and breach containment.

Key Concepts Learned
1. Post-Triage Alert Flow

After L1 triage:

False Positives → Closed with documentation

True Positives → Reported and escalated to L2

Major Incidents → May involve DFIR/IR teams

Workflow:

L1 Triage → Report Writing → Escalation → L2 Investigation → Remediation → Incident Response (if required)

2. Importance of Alert Reporting
Context for Escalation

Provides L2 with structured investigation summary

Reduces redundant analysis

Accelerates containment

Evidence Preservation

Raw logs retained for 3–12 months

Alert reports stored indefinitely

Supports audits and compliance

Skill Development

Enhances structured analytical thinking

Strengthens technical communication

Forces justification of verdict

3. The 5Ws Reporting Framework

A structured SOC reporting model.

Who

Affected user account

Privilege level

Department or role

What

Exact activity performed

Commands executed

Files accessed or downloaded

When

Start time

End time

Timezone reference

Where

Hostname

Source IP

Target IP

Domain or URL

Why

Evidence supporting final verdict

Threat intelligence validation

Behavioral analysis findings

4. Escalation Criteria

Escalate alerts when:

Confirmed malware execution

Credential dumping or domain reconnaissance

Lateral movement indicators

Data exfiltration suspected

Privileged account compromise

Remediation actions required

External communication required

Unclear investigation requiring senior review

5. Escalation Workflow

Operational SOC process:

Move alert to In Progress

Perform full investigation

Write structured 5W report

Set verdict = True Positive

Reassign alert to L2 analyst

Notify L2

L2 continues investigation from L1 documentation.

6. Communication in SOC Operations

SOC may coordinate with:

IT Team → Confirm administrative changes

HR → Validate user activity

Network Team → Confirm firewall updates

Management → Report high-severity incidents

Communication prevents false escalation and ensures proper containment.

Tools and Systems Discussed
SIEM

Purpose:

Centralized log collection and alert generation

SOC Usage:

Alert triage

Log investigation

Correlation analysis

Examples:

Splunk

Elastic

EDR

Purpose:

Endpoint-level monitoring

SOC Usage:

Process tree analysis

Malware detection

Host-based investigation

Examples:

Microsoft Defender

CrowdStrike

ITSM / Ticketing System

Purpose:

Alert tracking and documentation

SOC Usage:

Assigning alerts

Status updates

Maintaining accountability

Examples:

Jira

TheHive

Dashboard Actions Practiced

assign alert to analyst
move alert to “In Progress”
write structured investigation report
set verdict (True Positive / False Positive)
reassign alert to L2
close alert
request L2 support

Skills Developed

Structured incident documentation (5W framework)

Escalation decision-making

Analytical justification of verdicts

Cross-team communication awareness

SOC workflow maturity

Understanding of L1–L2 operational boundary

Incident lifecycle awareness
