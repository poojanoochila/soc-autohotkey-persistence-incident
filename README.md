# 🛡️ SOC Incident: AutoHotkey Persistence Malware Investigation

## 📌 Overview
This repository documents a real-world security incident involving unauthorized script-based persistence on a Windows system. The investigation identified and removed a multi-stage execution chain leveraging AutoHotkey and Windows scripting.

## 🚨 Key Findings
- Unauthorized AutoHotkey execution
- Malicious scripts in the Public directory
- Multi-stage payload (.vbs → .bat → .exe)
- Persistence mechanism outside standard startup

## 🔍 Highlights
- Identified execution path using command-line analysis
- Detected misuse of the `C:\Users\Public` directory
- Removed persistence via Task Scheduler and registry cleanup

## 📂 Full Report
See: [incident_report.md](incident_report.md)

## 📁 Evidence
Screenshots, and analysis available in `/evidence`

## 🎯 Skills Demonstrated
- Threat detection
- Process analysis
- Persistence identification
- Incident response & remediation
- Basic malware analysis

## 🧠 Note
This investigation was conducted on a personal system to analyze real-world persistence techniques.

---

## 🏷️ Tags
`SOC` `DFIR` `Cybersecurity` `MalwareAnalysis` `BlueTeam`
