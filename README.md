# Microsoft Sentinel Threat Hunting and Detection Engineering

![Microsoft Sentinel](https://img.shields.io/badge/SIEM-Microsoft%20Sentinel-0078D4)
![Microsoft Defender XDR](https://img.shields.io/badge/XDR-Microsoft%20Defender%20XDR-5E5E5E)
![Microsoft Defender for Endpoint](https://img.shields.io/badge/EDR-Microsoft%20Defender%20for%20Endpoint-107C10)
![Microsoft Azure](https://img.shields.io/badge/Cloud-Microsoft%20Azure-0078D4)
![KQL](https://img.shields.io/badge/Language-KQL-blue)
![MITRE ATT\&CK](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red)

![PowerShell Threat Hunt](SCREENSHOTS/Figure_08_PowerShell_Threat_Hunt.png)

## Overview

This project demonstrates the deployment, configuration, and operational use of **Microsoft Sentinel** as a cloud-native Security Information and Event Management (SIEM) platform for threat hunting and detection engineering.

A Microsoft Sentinel workspace was integrated with **Microsoft Defender XDR** and **Microsoft Defender for Endpoint (MDE)** to collect endpoint telemetry from a Windows 11 device. Kusto Query Language (KQL) was used to validate telemetry, perform proactive threat hunting, and develop custom detections that simulate common Security Operations Center (SOC) workflows.

---

## Project Objectives

* Deploy and configure Microsoft Sentinel
* Integrate Microsoft Defender XDR
* Validate endpoint telemetry collection
* Perform threat hunting using KQL
* Investigate endpoint process, network, and registry activity
* Develop custom detection rules
* Configure alert enrichment and entity mapping
* Map findings to the MITRE ATT&CK Framework

---

## Lab Environment

| Component           | Technology                      |
| ------------------- | ------------------------------- |
| SIEM                | Microsoft Sentinel              |
| XDR Platform        | Microsoft Defender XDR          |
| Endpoint Protection | Microsoft Defender for Endpoint |
| Operating System    | Windows 11                      |
| Cloud Platform      | Microsoft Azure                 |
| Detection Language  | Kusto Query Language (KQL)      |

---

## Threat Hunting

Three threat hunting exercises were performed using Microsoft Defender Advanced Hunting and Kusto Query Language (KQL).

| Hunt                    | Purpose                                                   |
| ----------------------- | --------------------------------------------------------- |
| PowerShell Activity     | Identify PowerShell execution                             |
| Reconnaissance Activity | Detect discovery commands                                 |
| Persistence Analysis    | Detect registry modifications associated with persistence |

Each hunt has been included as an individual KQL query within the **KQL** directory.

---

## Detection Engineering

Threat hunting results were transformed into custom Microsoft Sentinel detections.

Detection engineering activities included:

* Analytics Rule Creation
* Alert Configuration
* Entity Mapping
* Detection Validation
* Alert Enrichment

---

## MITRE ATT&CK Mapping

| Detection                       | ATT&CK Technique                          |
| ------------------------------- | ----------------------------------------- |
| PowerShell Execution            | T1059.001 – PowerShell                    |
| System Information Discovery    | T1082                                     |
| Account Discovery               | T1087                                     |
| Network Configuration Discovery | T1016                                     |
| User Discovery                  | T1033                                     |
| Registry Persistence            | T1547 – Boot or Logon Autostart Execution |
| Registry Modification           | T1112 – Modify Registry                   |

---

## KQL Queries Included

The repository includes reusable KQL queries for:

* DeviceInfo Telemetry Validation
* DeviceProcessEvents Validation
* DeviceNetworkEvents Validation
* DeviceRegistryEvents Validation
* PowerShell Activity Hunt
* Reconnaissance Activity Hunt
* Persistence Analysis Hunt

---

## Skills Demonstrated

* Microsoft Sentinel Administration
* Threat Hunting
* Detection Engineering
* Kusto Query Language (KQL)
* Microsoft Defender XDR
* Microsoft Defender for Endpoint
* Endpoint Telemetry Analysis
* MITRE ATT&CK Mapping
* Incident Investigation
* SIEM Operations

---

## Repository Structure

```text
Microsoft-Sentinel-Threat-Hunting-and-Detection-Engineering/
│
├── REPORT/
│   └── Microsoft_Sentinel_Threat_Hunting_and_Detection_Engineering_Lab.pdf
│
├── SCREENSHOTS/
│   └── Project Figures
│
├── KQL/
│   ├── DeviceInfo_Telemetry_Check.kql
│   ├── DeviceProcessEvents_Validation.kql
│   ├── DeviceNetworkEvents_Validation.kql
│   ├── DeviceRegistryEvents_Validation.kql
│   ├── PowerShell_Activity_Hunt.kql
│   ├── Reconnaissance_Activity_Hunt.kql
│   └── Persistence_Analysis_Hunt.kql
│
├── LICENSE
└── README.md
```

---

## Documentation

The complete technical report is available in the **REPORT** folder and documents:

* Microsoft Sentinel deployment
* Microsoft Defender XDR integration
* Endpoint telemetry validation
* Threat hunting using Kusto Query Language (KQL)
* Detection engineering
* MITRE ATT&CK mapping
* Findings and lessons learned

---

## Key Takeaways

This project demonstrates practical SOC analyst skills through the deployment of Microsoft Sentinel, proactive threat hunting using Kusto Query Language (KQL), endpoint telemetry validation, detection engineering, and MITRE ATT&CK mapping. It reflects many of the responsibilities performed by security analysts responsible for security monitoring, threat detection, incident investigation, and detection engineering within enterprise environments.

---

## Author

**Eric Johnson**

* GitHub: https://github.com/ericjohnson4
* CompTIA Security+
* CompTIA CySA+
* M.S. Cybersecurity (In Progress)

---
