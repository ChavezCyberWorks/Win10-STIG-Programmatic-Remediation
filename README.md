
# 🛡️ Win10-STIG-Programmatic-Remediation

**Windows Security Technical Implementation Guides (STIGs)** are configuration baselines developed by the [Defense Information Systems Agency (DISA)](https://stigaview.com/products/win10/v3r4/) to strengthen system hardening and prevent unauthorized access.

This project documents the remediation efforts taken to bring a Windows 10 system into compliance using PowerShell-based automation.

---

## 📆 Scan History

| Scan Date  | ❌ Failed | ⚠️ Warning | ✅ Passed | 🧩 Remediated | 📊 Total STIGs |
|------------|-----------|------------|-----------|---------------|----------------|
| 2025-06-29 | 149       | 15         | 100       | 0             | 264            |
| 2025-07-09 | 140       | 15         | 119       | **9**        | 264            |

> ✨ Progress: Reduced 9 failed STIGs through custom PowerShell remediations.

---

## 🔧 Remediation Table

| STIG ID | Severity | Description | Language | Script |
|--------|----------|-------------|----------|--------|
| WN10-CC-000030 | Low | The system must prevent ICMP redirects from overriding OSPF routes | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-CC-000030%20-%20Disable%20ICMP%20Redirects) |
| WN10-CC-000197 | Low | Microsoft consumer experiences must be turned off| PowerShell | [View]([./remediation/remediate-WN10-CC-000005.ps1](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-CC-000197%20-%20Disable%20Microsoft%20Consumer%20Experiences)) |
| WN10-AC-000005 | Medium | Windows 10 account lockout duration must be configured to 15 minutes or greater. | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-AC-000005%20-%20Lockout%20Duration%20to%2015%2B%20Minutes) |
| WN10-AC-000010| Medium | Camera access from the lock screen must be disabled. | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-AC-000010%20-%20Set%20Logon%20Attempt%20Threshold) |
| WN10-CC-000365 | Medium | Prevent Windows apps from activating by voice while the system is locked. | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-CC-000365%20-%20Prevent%20Voice%20Activation%20While%20Locked) |
| WN10-SO-000005| Medium |  The built-in administrator account must be disabled. | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-SO-000005%20-%20Disable%20Built-in%20Administrator) |
| WN10-SO-000010 | Medium | The built-in guest account must be disabled | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-SO-000010%20-%20Disable%20Guest%20Account) |
| WN10-SO-000255 | Medium |  User Account Control must automatically deny elevation requests for standard users. | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-SO-000255%20-%20UAC%20Deny%20Elevation%20for%20Standard%20Users) |
| WN10-CC-000190| High | Autoplay must be disabled for all drives | PowerShell | [View](https://github.com/ChavezCyberWorks/Win10-STIG-Programmatic-Remediation/blob/d274aebb3fd34b37565d07dd02d261a984415dcb/STIG/WN10-CC-000190%20-%20Disable%20Autoplay%20for%20All%20Drives) |
| *(More remediations coming soon...)* | | | | |

---

## 📁 Repository Layout


---

## ⚙️ Tested On

- **System**: Windows 10 Pro x64 (Virtual Machine)
- **PowerShell**: v5.1+
- **Privileges**: Administrator

---

## 🧠 Goal

Bring total failed STIGs to **zero** by implementing secure configurations that align with DISA guidance — all automated and auditable via version-controlled scripts.

---



