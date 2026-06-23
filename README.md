# Purple-Team Cybersecurity Lab

## Overview
A fully operational purple-team (red + blue) home lab for testing EDR/SIEM detection capabilities against ransomware simulations and network-based attacks.

## Architecture
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

## Screenshots
<img width="1920" height="1080" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/6ea373aa-3c8b-4333-ba7a-98ed4f65516c" />
<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/299fee04-cbb7-4547-acf0-40a8f67887e9" />
<img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/504e16e3-8833-4076-8361-a0fbc84d6ab6" />
<img width="1920" height="1080" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/fdff6a92-88ba-4627-b650-95db12f4deaa" />

## Report
[Purple_Team_Lab_Report.pdf](https://github.com/user-attachments/files/29241901/Purple_Team_Lab_Report.pdf)
