# 🧠 Home SOC Lab Environment

## 📌 Overview
This project demonstrates how I designed and configured a small-scale Security Operations Center (SOC) environment at home to simulate real-world network defense and threat detection. The setup includes Windows and Linux virtual machines monitored through Splunk and Security Onion to collect and analyze logs for suspicious activity. This lab showcases hands-on experience with SIEM tools, incident detection, and threat analysis.

---

## 🛠️ Tools & Technologies Used
- Splunk Enterprise (Free Edition)
- Security Onion (IDS/IPS)
- Windows 11 & Ubuntu Server (VirtualBox)
- Kali Linux (Red Team Simulation)
- Wireshark
- MITRE ATT&CK Framework (T1110 - Brute Force, T1059 - Command and Scripting Interpreter)
- PowerShell & Python for automation
- Tenable / Nessus Essentials for vulnerability scanning

---

## 🧩 Objective
> Build and operate a realistic home SOC environment to monitor, detect, and analyze simulated attacks using enterprise-style tools and methodologies.

---

## ⚙️ Setup & Configuration
1. Deployed multiple virtual machines using **VirtualBox** (Windows 11, Ubuntu, and Kali Linux).  
2. Installed and configured **Splunk** to collect Security, System, and Application logs.  
3. Set up **Security Onion** for network-based intrusion detection.  
4. Configured **Sysmon** and **Windows Event Forwarding (WEF)** to send host logs to Splunk.  
5. Simulated brute-force attacks using Kali Linux (Hydra) to test detection accuracy.  
6. Integrated **MITRE ATT&CK** mappings into Splunk dashboards for threat correlation.

---

## 🔍 Investigation Process
- Monitored event logs in Splunk for **failed login attempts (Event ID 4625)**.  
- Correlated failed logins from multiple IPs to identify brute-force attempts.  
- Captured traffic in Wireshark and analyzed suspicious PowerShell commands.  
- Validated IDS alerts in Security Onion related to brute-force and exploit attempts.  
- Documented the incident following basic **SOC Level 1 triage** procedures.  

---

## 📊 Findings & Results
- Detected brute-force attempts using Splunk query on Event ID 4625.  
- Identified IP-based attack pattern and verified through packet capture.  
- Correlated host and network logs to confirm the attack timeline.  
- Created a detection rule to automatically alert on similar patterns.  

---

## 🧱 Mitigation & Recommendations
- Implemented account lockout policies after failed login attempts.  
- Restricted RDP access to internal networks only.  
- Recommended enabling MFA and advanced endpoint monitoring for critical accounts.  
- Improved Splunk query performance and dashboard alerting.  

---

## 🧰 Skills Demonstrated
- SOC Operations Fundamentals  
- SIEM Configuration & Log Analysis (Splunk)  
- IDS/IPS Monitoring (Security Onion)  
- Threat Detection & Incident Triage  
- MITRE ATT&CK Technique Mapping  
- Network Traffic Analysis (Wireshark)  
- Basic Automation with PowerShell & Python  

---

## 🧾 Sample Evidence
