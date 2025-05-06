# Kerberoasting Attack & Detection Lab

This project simulates a Kerberoasting attack in an Active Directory environment and detects it using Wazuh SIEM.

## 🧠 Objective
Demonstrate how service ticket hashes can be extracted and cracked, and how to monitor/detect such activity with Event ID 4769 in Wazuh.

## ⚙️ Lab Setup
- Domain Controller: Windows Server 2019 (`lab.local`)
- Service Account with SPN: `svc_sql`
- Attacker VM: Parrot OS with Rubeus & Hashcat
- SIEM: Wazuh + Kibana

## 🧨 Attack Flow
1. Login as domain user
2. Use Rubeus to request TGS
3. Extract and crack hash offline
4. Trigger SIEM detection

## 🔍 Detection
- Wazuh monitored Event ID 4769
- Alerts based on SPN request patterns
- Visualized using Kibana

## 📎 Files Included
- `Report.pdf` – Detailed attack + detection explanation


---

**Created by:** [Simpal Kumari]  
**Role:** SOC Analyst | Cybersecurity Enthusiast
