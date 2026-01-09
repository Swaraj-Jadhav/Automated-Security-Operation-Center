🛡️ End-to-End SOC Platform with SIEM, SOAR, Threat Intelligence & DFIR

## 📌 Project Overview
This project implements a **full-scale Security Operations Center (SOC) platform** using open-source industry tools.  
It covers **log ingestion, detection engineering, threat intelligence enrichment, incident response, DFIR, and SOAR automation** — closely mirroring real-world SOC architectures used by MSSPs and enterprise security teams.

---

## 🏗️ Architecture Overview

<img width="633" height="361" alt="SOAR" src="https://github.com/user-attachments/assets/25f29d1c-a423-4a7b-87b2-bfd9903f9e90" />


---

## 🔧 Tools & Technologies

| Category | Tools |
|-------|------|
| SIEM & Log Analysis | Wazuh Manager, Wazuh Indexer, Graylog |
| Visualization | Wazuh Dashboard |
| Threat Intelligence | MISP |
| Incident Response | TheHive, Cortex |
| DFIR & Threat Hunting | Velociraptor |
| Automation / SOAR | n8n |
| OS | Ubuntu Linux, Windows |

---

## 🟦 SIEM & Log Management (Wazuh + Graylog)

### Implemented Features
- Installed **Wazuh Manager** for centralized log analysis
- Deployed **Wazuh agents** on Linux and Windows endpoints
- Collected logs from:
  - Authentication events
  - System activity
  - Syslog sources
- Forwarded alerts to **Graylog** for log processing
- Used **Wazuh Indexer** for scalable log storage

### Detection Use Cases
- Failed login attempts
- Privilege escalation
- File integrity violations
- Suspicious process execution

---

## 📊 Security Dashboards (Wazuh Dashboard)

- Real-time SIEM dashboards
- MITRE ATT&CK mapped alerts
- Authentication anomaly trends
- Alert severity distribution
- Geo-IP based visualization

---

## 🧠 Threat Intelligence (MISP)

- Installed **MISP** for centralized IOC management
- Ingested public and custom threat feeds
- Managed indicators:
  - IP addresses
  - Domains
  - File hashes
- Enriched Wazuh alerts using MISP intelligence

---

## 🚨 Incident Response & Case Management (TheHive + Cortex)

### TheHive
- Automated case creation from security alerts
- Incident lifecycle management:
  - Triage
  - Investigation
  - Containment
  - Closure

### Cortex
- Automated IOC enrichment using analyzers:
  - VirusTotal
  - AbuseIPDB
  - Threat intelligence feeds


## 🔍 DFIR & Threat Hunting (Velociraptor)

- Endpoint threat hunting
- Artifact collection
- Persistence mechanism detection
- Memory and process analysis
- Insider threat & malware investigation scenarios

---

## ⚙️ SOAR Automation (n8n)

### Automated Workflows
- Wazuh alert ingestion
- IOC enrichment via MISP
- Case creation in TheHive
- Analyst notification (Email / Slack)
- Optional simulated response actions

**SOAR Flow**
