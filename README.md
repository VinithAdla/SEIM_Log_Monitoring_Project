# SIEM_Log_Monitoring_Project

## 📌 Project Overview
This project demonstrates a Security Information and Event Management (SIEM) lab setup using **Sysmon**, **Winlogbeat**, **Logstash**, and **Splunk** to detect suspicious processes and visualize activity in a SOC-style dashboard.  
It simulates real-world detection and monitoring use cases that SOC analysts perform daily.

---

## 🔧 Tools & Technologies
- **Sysmon** – Captures detailed Windows event logs (process creation, network connections, etc.)
- **Winlogbeat** – Ships Windows Event Logs to Logstash
- **Logstash** – Parses and forwards logs to Splunk via HTTP Event Collector (HEC)
- **Splunk** – Visualizes logs, detects anomalies, and builds dashboards

---

## 🎯 Project Goals
- Collect and ship Windows logs using Sysmon and Winlogbeat
- Parse and normalize logs with Logstash
- Forward logs to Splunk for indexing and analysis
- Create dashboards to identify suspicious activity such as PowerShell or cmd.exe executions
- Simulate SOC-style alert triage and investigation

---

## 📈 Use Cases
- **Suspicious Process Detection** – Identify execution of potentially malicious processes
- **Host Activity Tracking** – Monitor event frequency and anomalies
- **SOC Visualization** – Use Splunk dashboards for rapid detection and analysis
- **MITRE ATT&CK Mapping** – Link detection logic to adversary tactics and techniques

---

## 📄 MITRE ATT&CK Coverage
| Technique | Tactic           | Description                              |
|-----------|------------------|------------------------------------------|
| T1059.001 | Execution        | PowerShell Command Execution            |
| T1047     | Discovery        | Windows Management Instrumentation (WMI)|
| T1036     | Defense Evasion  | Masquerading of process names            |

