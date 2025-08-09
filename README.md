# Threat-Feed-Report-Nspire-Ransomware
This repository contains the Threat Feed Report for the ransomware strain Nspire (also known as NightSpire Virus). This project documents the ransomware's behavior, technical indicators, attribution, and recommended mitigation strategies. It is intended for cybersecurity professionals, SOC analysts, and threat intelligence teams.
Nspire-Threat-Feed/
│
├── README.md                  # Project overview and usage instructions
├── Nspire-Threat-Feed.pdf     # Detailed threat report document
├── IoCs.csv                   # Extracted Indicators of Compromise
├── ransom_note_sample.txt     # Sample ransom note text
├── screenshots/
│   ├── ransom_note.png         # Screenshot of ransom note
│   └── tor_site.png            # Screenshot of ransom payment portal
└── MITRE_MAPPING.md           # TTP mapping to MITRE ATT&CK framework
📄 Executive Summary

Nspire is a ransomware strain targeting finance, logistics, healthcare, and technology sectors. It encrypts files, appends the .nspire extension, and demands Bitcoin payments through a Tor site. The ransomware is distributed via phishing campaigns and unsecured network connections.

Key Attributes:

Type: Ransomware, Fileslocker, Stealer, Spyware

First Seen: 2025-05-18

Last Seen: 2025-07-07

Threat Sources: VirusTotal, Malware Bazaar, OSINT

Risk Level: High

Data Loss Potential: Confirmed

🛠 Technical Indicators (IoCs)

IOC Type

Value

SHA256 Hash

32e10dc9fe935d7c835530be214142041b6aa25ee32c62648dea124401137ea5

MD5 Hash

2bf543faf679a374af5fc4848eea5a98

File Size

4.2 MB

Extension

.nspire

File Path

C:\ProgramData\System\nspire_payload.exe

C2 Server

213.156.145.22 / nsp1relk6xsxbxi4.onion

Contact

nightspireteam.receiver@onionmail.org

A full CSV file containing IoCs is available in this repository.

🎯 Attribution

Threat Actor: Nspire Ransomware Group

Possible Link: Rebrand of a LockBit affiliate group

Known Victims:

Raja Ferry Port Public Company Limited

M-POWER Information

Al Tadawi Specialty Hospital

60+ unnamed victims

Target Locations: Thailand, Taiwan, UAE

🧠 MITRE ATT&CK Mapping

Tactic

Technique ID

Description

Impact

T1486

Data Encrypted for Impact

Collection

T1005

Data from Local System

Credential Access

T1555

Credentials from Password Stores

Command & Control

T1573

Encrypted Channel (Tor usage)

Initial Access

T1190

Exploit Public-Facing Application

Full mapping is available in MITRE_MAPPING.md.

🚑 Mitigation & Recommendations

Add known file hashes to antivirus and EDR blocklists.

Audit for suspicious scheduled tasks and PowerShell usage.

Isolate infected systems immediately upon detection.

Train employees to recognize phishing and malicious attachments.

Regularly back up critical systems and store backups offline.

📎 References & Attachments

VirusTotal Report: (Link included in PDF)

Malware Bazaar Entry

Sample ransom note

Screenshots of Tor payment portal

🏷 Suggested GitHub Tags

#Cybersecurity #Ransomware #ThreatIntel #MalwareAnalysis #Nspire
#MITRE #IoCs #SOC #IncidentResponse

📌 How to Use This Repository

For SOC Teams: Use the IoCs for detection and prevention.

For Researchers: Study the MITRE mappings and threat behavior patterns.

For Incident Responders: Apply the mitigation recommendations immediately upon suspected infection.

Author: Hitesh SaidDate: 19 July 2025
