# 🛡️ SOC Incident Report: Script-Based Persistence Malware

## 📌 Incident Summary
An unauthorized persistence mechanism was identified on a Windows system involving repeated AutoHotkey execution triggered by malicious scripts located in a public directory.

- **Severity:** High
- **Type:** Persistence / Script-based Malware
- **Detection:** Manual observation (unexpected popups)

---

## 🔍 Indicators of Compromise (IOCs)

### File Paths
- C:\Users\Public\Documents\PicsArt
- C:\Users\Public\Torrent

### Files
- example.exe
- PicsArtAppampro.vbs
- run.vbs
- 1.bat

---

## 🧪 Investigation

### 1. Detection
User observed repeated AutoHotkey popups.

### 2. Process Analysis
Command-line revealed execution from:
C:\Users\Public\Documents\PicsArt

### 3. File Discovery
Malicious scripts and executable found in public directory.

### 4. Execution Chain
- VBScript (.vbs) launches
- Batch script (.bat) executes commands
- Executable (.exe) runs payload
- AutoHotkey used for persistence

---

## ⚙️ Attack Chain

1. Script Execution (.vbs)
2. Command Execution (.bat)
3. Payload Execution (.exe)
4. AutoHotkey trigger
5. Persistence mechanism

---

## 🧹 Remediation

- Terminated AutoHotkey process
- Deleted malicious directories
- Removed scheduled tasks
- Cleaned registry run keys
- Emptied recycle bin
- Performed full system scan

---

## ✅ Outcome
- Persistence removed
- System restored
- No further execution observed

---

## 🎯 MITRE ATT&CK

- T1059 – Command and Scripting Interpreter
- T1547 – Autostart Execution
- T1036 – Masquerading
- T1204 – User Execution

---

## 🧠 Conclusion
This case highlights how simple scripting techniques can establish persistence using trusted tools and directories.
