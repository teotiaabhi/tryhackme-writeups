Room: SOC Metrics & Performance Improvement

Platform: TryHackMe
Difficulty: Easy
Date Completed: 27-02-2026

🧾 Overview

This room focused on SOC performance metrics and Service Level Agreements (SLA). It explained how Security Operations Centers measure efficiency, detection capability, response speed, and analyst performance.

The room covered core operational metrics such as False Positive Rate, Alert Escalation Rate, Threat Detection Rate, and time-based metrics including MTTD, MTTA, and MTTR.

The objective was to understand how metrics influence SOC efficiency and how L1 analysts can contribute to improving them.

In real-world SOC environments, these metrics are used to evaluate team performance, reduce attacker dwell time, and ensure continuous improvement.

🎯 Learning Objectives

Understand core SOC performance metrics

Learn SLA time-based metrics (MTTD, MTTA, MTTR)

Identify root causes of poor SOC performance

Understand how L1 analysts can improve operational metrics

🔎 Key Concepts Learned
1. False Positive Rate (FPR)

Definition:
Percentage of alerts that are not real threats.

Formula:
FPR = False Positives / Total Alerts

Explanation:

Measures alert noise

High FPR causes analyst fatigue

Indicates detection tuning issues

Why it matters:
High FPR increases risk of missed real attacks.

2. Alert Escalation Rate (AER)

Definition:
Percentage of alerts escalated from L1 to L2.

Formula:
AER = Escalated Alerts / Total Alerts

Explanation:

Reflects L1 experience

High rate = over-escalation

Low rate = possible overconfidence

3. Threat Detection Rate (TDR)

Definition:
Percentage of real threats successfully detected.

Formula:
TDR = Detected Threats / Total Threats

Explanation:

Measures SOC effectiveness

Should ideally be 100%

4. Mean Time to Detect (MTTD)

Definition:
Average time between attack occurrence and detection.

Explanation:

Tool and detection rule performance metric

Lower MTTD reduces attacker dwell time

5. Mean Time to Acknowledge (MTTA)

Definition:
Average time for L1 to start investigating an alert.

Explanation:

Measures analyst responsiveness

Directly controlled by L1 behavior

6. Mean Time to Respond (MTTR)

Definition:
Average time to contain and remediate an attack.

Explanation:

Measures operational maturity

Requires structured playbooks and escalation

🛠️ Tools and Systems Used

SIEM Platform (e.g., Splunk)

Purpose:
Log monitoring and alert generation

Used For:

Alert detection

Log correlation

Threat identification

Detection Rule Engine

Purpose:
Trigger alerts based on defined conditions

Used For:

Threat detection

Reducing MTTD

Notification Systems

Purpose:
Alert analysts in real-time

Used For:

Improving MTTA

💻 Actions Practiced

Calculate False Positive Rate

Calculate Threat Detection Rate

Calculate MTTD, MTTA, MTTR

Identify root cause of performance issues

Assign metric improvement tasks

Match problems with operational fixes

🧠 Investigation Workflow Impact

Metrics affect:

Alert prioritization

Triage speed

Escalation decisions

Response efficiency

Documentation quality

🚨 Indicators Observed

Alert Volume: 760 alerts per shift
Noise Level: 95%
Detection Delay Example: 20 minutes
Response Delay Example: 6 hours

📝 Reporting Structure (5Ws)

Who: SOC L1 and L2 teams
What: High noise, detection delays, response inefficiencies
When: During active monitoring shifts
Where: SOC monitoring environment
Why: Poor tuning, lack of documentation, slow notification systems

Final Verdict:
Metric optimization required

🔐 Security Concepts Reinforced

Performance measurement in SOC

Detection tuning

Alert fatigue risks

Escalation discipline

Continuous improvement mindset

🏗️ Skills Developed

Metric calculation

Root cause analysis

Operational improvement planning

Structured problem-solving

SOC performance evaluation

📌 Key Takeaways

Metrics directly impact security posture

False positives are dangerous long-term

Faster detection reduces breach impact

Documentation reduces response time

L1 performance influences promotions

📈 Career Relevance

SOC L1 Role:
Improves triage speed and escalation quality

Blue Team Operations:
Strengthens detection efficiency

Incident Response:
Reduces containment time

Threat Detection:
Improves rule tuning awareness
