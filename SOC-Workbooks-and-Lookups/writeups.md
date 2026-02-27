Room: SOC Fundamentals – Identity, Asset & Workbook-Based Investigation

Platform: TryHackMe
Difficulty: Easy
Date Completed: 27-02-2026

🧾 Overview

This room focused on understanding how SOC analysts use identity inventory, asset inventory, network diagrams, and structured workbooks to properly triage security alerts.

The main objective was to teach how to add context to alerts before making a verdict and how to follow a standardized investigation workflow.

The room is highly relevant for SOC L1 analysts because it emphasizes structured triage, enrichment processes, and consistent escalation practices.

In real-world SOC environments, analysts must validate users, assets, and network behavior before deciding whether activity is malicious or expected. This room simulates that professional decision-making process.

🎯 Learning Objectives

Understand what identity inventory is and how it supports alert triage

Understand asset inventory and its role in contextual investigations

Learn how network diagrams help reconstruct attack paths

Understand SOC workbooks and structured investigation workflows

🔎 Key Concepts Learned
1. Identity Inventory

Definition:
A centralized catalogue of corporate user accounts, service accounts, and machine identities containing role and privilege information.

Explanation:

Stores employee details such as role and department

Shows working hours and access privileges

Helps validate whether user behavior is expected

Used during enrichment stage of investigation

Why it matters:
Without identity context, analysts cannot determine if activity is normal for a user.

Where it is used:

SOC investigations

HR validation

Access control verification

2. Asset Inventory

Definition:
A database of corporate IT assets including servers and workstations with ownership and purpose information.

Explanation:

Contains hostname, IP, subnet, and department owner

Shows what type of data the server stores

Helps classify asset sensitivity

Assists in access validation

Technical Breakdown:

Example: HQ-FINFS-02

HQ → Headquarters

FIN → Finance

FS → File Server

Likely stores financial records and accounting data.

3. Network Diagrams

Definition:
Visual representation of corporate network layout, subnets, firewall placement, and exposed services.

Explanation:

Maps subnets (VPN, Office, Database)

Shows firewall rules and exposed ports

Helps reconstruct lateral movement

Identifies attack path

Used to analyze scenarios like:

VPN brute force

Internal scanning

Subnet reconnaissance

4. Enrichment Process

Definition:
The process of gathering additional user, host, and IP context before making a verdict.

Explanation:

Uses Threat Intelligence

Checks identity inventory

Checks asset inventory

Reviews historical logs

Purpose: Reduce false positives and avoid premature escalation.

5. SOC Workbooks (Playbooks / Runbooks)

Definition:
Structured investigation documents defining step-by-step triage procedures.

Explanation:

Created by senior analysts (L2/L3)

Used primarily by SOC L1 analysts

Ensures consistent investigations

Prevents missed steps

Workbook structure includes:

Enrichment

Investigation

Escalation

🛠️ Tools and Systems Used
Active Directory

Purpose:
Identity and asset directory service.

Used In This Room For:

Identity lookup

Asset validation

BambooHR

Purpose:
HR identity inventory system.

Used In This Room For:

Verifying user location

Confirming expected working hours

SIEM (e.g., Splunk)

Purpose:
Centralized log analysis platform.

Used In This Room For:

Investigating login events

Reviewing suspicious activity

Correlating logs

Threat Intelligence Platforms

Purpose:
IP/domain reputation checking.

Used In This Room For:

Checking malicious IP indicators

💻 Commands / Actions Practiced

Dashboard-based actions practiced:

Investigate suspicious login

Analyze alert logs

Review network activity

Identify subnet ownership

Validate user role via identity inventory

Analyze email headers (SPF/DKIM)

Perform attachment sandbox analysis

Write investigation report

Escalate alert to L2

🧠 Investigation Workflow (SOC Focused)

Prioritize alert

Assign to analyst

Move to In Progress

Perform enrichment (identity + asset + TI lookup)

Analyze logs in SIEM

Validate findings against business logic

Write 5W investigation summary

Set verdict (Safe / Suspicious / Malicious)

Escalate if required

🚨 Indicators Observed

IP Address: 103.61.240.174
Internal VPN IP: 10.10.0.53
Subnet: 172.16.15.0/24 (Database)
Subnet: 172.16.23.0/24 (Office)
File Name: Financial Report US 2024.xlsx
Username: G.Baker
Shared With: R.Lund

📝 Reporting Structure (5Ws)

Who:
External IP performing VPN brute force and internal scanning.

What:
Unauthorized VPN access followed by subnet scanning.

When:
Observed during firewall log timestamps.

Where:
VPN subnet → Database subnet → Office subnet.

Why:
Likely reconnaissance after successful credential compromise.

Final Verdict:
Escalated to L2 (Suspicious VPN compromise and internal reconnaissance).

🔐 Security Concepts Reinforced

Detection logic for suspicious login behavior

Threat identification using contextual analysis

Log correlation between firewall and VPN logs

Proper incident escalation process

Structured documentation discipline

🏗️ Skills Developed

Identity and asset validation

Network attack path reconstruction

Alert triage methodology

Evidence-based decision making

Structured reporting

Escalation judgment

📌 Key Takeaways

Alerts without context are meaningless.

Identity and asset inventories are critical for correct verdicts.

Network diagrams simplify attack reconstruction.

Workbooks prevent investigation errors.

Enrichment must always precede verdict.

Operational insight:
SOC work is structured analysis — not assumptions.

📈 Career Relevance

This room directly supports:

SOC L1 Role

Teaches structured alert triage

Reinforces enrichment and escalation

Blue Team Operations

Strengthens contextual detection skills

Improves investigation consistency

Incident Response

Builds foundational investigation discipline

Enhances documentation quality
