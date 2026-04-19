<div align="center">

# Sam — Offensive Security Portfolio

**Penetration Tester in Training | HTB Player | Pursuing CJCA → OSCP**

[![HTB Profile]([https://img.shields.io/badge/HackTheBox-s4mjx-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://app.hackthebox.com/profile/overview](https://app.hackthebox.com/users/1975686?profile-top-tab=machines&ownership-period=1M&profile-bottom-tab=prolabs))
[![GitHub](https://img.shields.io/badge/GitHub-s4mjx-181717?style=for-the-badge&logo=github)](https://github.com/s4mjx)

</div>

---

## About

Offensive security practitioner building hands-on penetration testing skills through HackTheBox machines and Sherlocks. Every engagement is documented with a professional penetration test report following industry methodology: reconnaissance → enumeration → exploitation → post-exploitation → reporting.

Currently focused on **Active Directory attacks**, **Web Application Security**, and **Digital Forensics & Incident Response (DFIR)**, working toward the HTB Certified Junior Cybersecurity Analyst (CJCA) certification.

---

## HTB Machines Completed

> Full professional PDF reports available in each folder.

| Machine | OS | Difficulty | Key Techniques | Report |
|---|---|---|---|---|
| [Meow](./htb-machines/meow/) | Linux | Very Easy | Telnet enumeration, default credentials | [PDF](./htb-machines/meow/Meow_Report.pdf) |
| [Fawn](./htb-machines/fawn/) | Linux | Very Easy | FTP enumeration, anonymous login | [PDF](./htb-machines/fawn/Fawn_Report.pdf) |
| [Dancing](./htb-machines/dancing/) | Windows | Very Easy | SMB enumeration, null session | [PDF](./htb-machines/dancing/Dancing_Report.pdf) |
| [Lame](./htb-machines/lame/) | Linux | Easy | CVE-2007-2447, Samba usermap_script | [PDF](./htb-machines/lame/Lame_Report.pdf) |
| [Legacy](./htb-machines/legacy/) | Windows | Easy | MS08-067, EternalBlue concept | [PDF](./htb-machines/legacy/Legacy_Report.pdf) |
| [Devel](./htb-machines/devel/) | Windows | Easy | FTP + IIS misconfiguration, MS11-046 LPE | [PDF](./htb-machines/devel/Devel_Report.pdf) |

---

## HTB Sherlocks Completed

> DFIR investigations analyzing real forensic artifacts.

| Sherlock | Category | Difficulty | Key Techniques | Report |
|---|---|---|---|---|
| [Campfire-1](./htb-sherlocks/campfire-1/) | DFIR | Very Easy | Kerberoasting detection, EVTX analysis, Prefetch forensics | [PDF](./htb-sherlocks/campfire-1/Campfire1_Report.pdf) |

---

## Technical Skills

**Penetration Testing**
- Network enumeration with Nmap, enum4linux, smbclient
- Exploitation with Metasploit and manual techniques
- Post-exploitation: privilege escalation, lateral movement concepts
- Professional reporting: CVSSv3 scoring, remediation recommendations

**DFIR & Threat Hunting**
- Windows Event Log analysis (EVTX) with Chainsaw
- Prefetch file forensics with PECmd / scca-info
- PowerShell ScriptBlock log analysis
- Kerberoasting detection (Event ID 4769 / Ticket Encryption Type 0x17)

**Tools**
`nmap` `metasploit` `msfvenom` `smbclient` `chainsaw` `PECmd` `Wireshark` `Burp Suite` `gobuster` `ffuf`

**Environments**
`Kali Linux` `Arch Linux` `Windows` `Active Directory` `HackTheBox VPN`

---

## Certification Roadmap

| Certification | Status | Target |
|---|---|---|
| CompTIA A+ | In Progress | 2026 Q3 |
| CompTIA Network | In Progress | 2016 Q4 |
| HTB CJCA | Preparing | 2027 Q1 |
| CompTIA Security+ | Preparing | 2027 Q1 |
| HTB CPTS | Planned | 2027 Q2 |
| HTB CDSA | Planned | 2027 Q2 |
| HTB CAPE | Planned | 2027 Q3 |
| OSCP | Planned | 2027 Q4 |

---

## Report Methodology

Every machine and Sherlock in this repository is documented following a professional penetration testing report structure:

1. **Executive Summary** — business impact, overall risk rating
2. **Scope & Methodology** — tools used, assessment type
3. **Findings** — CVSSv3 score, technical description, evidence, remediation
4. **Attack Chain** — complete kill chain narrative
5. **Recommendations** — hardening beyond specific findings

Reports are generated with Python (ReportLab) and follow CVSSv3 scoring, CWE classification, and MITRE ATT&CK mapping.

---

## Currently Working On

- [ ] HTB Tracks: Detecting Active Directory Attacks
- [ ] HTB Academy: CJCA CERTIFICATION PATH
- [ ] HTB Retired Machines: Easy

---

> *"Discipline beats motivation."*

> All content in this repository represents my own work for educational and portfolio purposes within the HackTheBox platform. No copyrighted course material is reproduced.
