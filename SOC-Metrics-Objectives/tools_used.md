🛠️ Tools & Commands Used

Room: SOC Metrics & Performance Improvement
Platform: TryHackMe

🧰 1️⃣ SIEM Platform (Example: Splunk / Elastic)
🔹 Purpose

Centralized log monitoring and alert generation.

🔹 Used In This Room For

Monitoring alert volume

Measuring detection delay

Reviewing alert timestamps

Calculating MTTA & MTTR

Identifying alert noise

💻 Example SOC Search Queries (Splunk-style)
Check Alert Volume
index=alerts | stats count by severity

Counts alerts grouped by severity.

Check Alert Timestamps
index=alerts alert_id="12345"

Used to identify when alert was triggered.

Calculate Detection Delay
index=alerts | eval detection_time=_time - attack_start_time

Used conceptually to measure MTTD.

🧰 2️⃣ Detection Rule Engine (SIEM Rules)
🔹 Purpose

Trigger alerts based on suspicious patterns.

🔹 Used In This Room For

Understanding why MTTD was high

Identifying slow rule execution

Adjusting rule frequency

🔧 Operational Action Practiced

Tune detection rules to run more frequently

Review detection rule schedule

Exclude trusted system activities

🧰 3️⃣ Notification System
🔹 Purpose

Notify analysts about critical alerts.

🔹 Used In This Room For

Reducing MTTA

Ensuring real-time alert acknowledgement

🔧 Improvement Actions

Enable real-time alert notifications

Configure SMS / Call escalation

Improve alert queue visibility

🧰 4️⃣ SOAR Platform (Conceptual Use)

Examples:

Cortex XSOAR

Splunk SOAR

🔹 Purpose

Automate repetitive alert triage tasks.

🔹 Used In This Room For

Reducing False Positive Rate

Automating common noise alerts

Improving MTTR

🧰 5️⃣ Detection Tuning Process (False Positive Remediation)
🔹 Purpose

Reduce alert noise.

🔹 Used In This Room For

Fixing 95% noise scenario

Improving analyst efficiency

🔧 Practical Actions Practiced

Exclude IT automation scripts

Remove trusted update alerts

Whitelist known safe activity

Adjust rule thresholds

🧰 6️⃣ Metric Calculation (Manual Analytical Skill)

No CLI tool — but analytical formulas practiced.

📊 False Positive Rate
FPR = False Positives / Total Alerts
📊 Threat Detection Rate
TDR = Detected Threats / Total Threats
📊 Alert Escalation Rate
AER = Escalated Alerts / Total Alerts
📊 SLA Metrics
MTTD

Time between attack and detection

MTTA

Time between alert generation and L1 acknowledgment

MTTR

Time between detection and containment

🧠 Actions Practiced (Operational, Not CLI)

Identify root cause of performance issue

Match metric to real-world scenario

Assign remediation tasks to correct role

Improve SOC workflow

Design workbook/playbook improvement

Balance workload distribution

🔥 Most Important Technical Skill Practiced

Not command execution — but:

Root cause analysis using metrics.

This is a senior-level SOC mindset skill.

📌 Important Real-World Tools Related to This Room

Even though not directly used in the lab, these are commonly involved in metric tracking:

Splunk (SIEM)

Elastic SIEM

Microsoft Sentinel

Cortex XSOAR

ServiceNow (ticketing)

Jira (workflow tracking)

PagerDuty (alert notifications)

🎯 Interview Tip

If asked:

“What tools are used to improve SOC metrics?”

Answer:

SIEM rule tuning

SOAR automation

Real-time notification systems

Detection engineering review

Log ingestion optimization
