# Purple-Team Cybersecurity Lab

## Overview
A fully operational purple-team (red + blue) home lab for testing EDR/SIEM detection capabilities against ransomware simulations and network-based attacks.

## Architecture
[INSERT NETWORK DIAGRAM HERE]

- **Attacker**: Kali Linux (192.168.100.144)
- **Victim**: Windows 10 VM (192.168.100.146) with Sysmon + Elastic Defend
- **SIEM**: Ubuntu Server (192.168.100.150) with Elasticsearch + Kibana + Fleet Server

## Key Technologies
- Elasticsearch 8.19.16 (log aggregation)
- Kibana 8.19.16 (visualization)
- Elastic Defend (EDR)
- Sysmon (Windows system monitoring)
- Infection Monkey (Attack Simulation and Ransomware Execution)
- Atomic Red Team (Built-in Attack simulation)
- Nmap, Hydra, SMBMap (reconnaissance)

## Testing Summary
✓ 4x T1486 (Ransomware) tests executed and detected
✓ SMB brute force: Administrator credentials cracked
✓ Account lockout triggered automatically by EDR
✓ Full pipeline: Sysmon → Agent → SIEM → Alerts

## How to Reproduce
[LINK TO lab-setup/ folder for detailed instructions]

## Findings
[LINK TO incident-report/ for detailed analysis]

## Report
[LINK TO Purple_Team_Lab_Report.docx for full documentation]
