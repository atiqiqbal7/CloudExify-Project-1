# 🔐 CloudExify Project 1 — Network Penetration Testing

**Internship:** CloudExify Cybersecurity Summer 2026  
**Project:** Network Penetration Testing  
**Target:** Metasploitable2 (192.168.164.138)  
**Status:** ✅ Completed

---

## 📋 Overview

This project demonstrates a complete network penetration test on an isolated virtual lab environment. 
The assessment includes network reconnaissance, port scanning, service enumeration, vulnerability 
identification, exploitation verification, and packet analysis.

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| nmap 7.94 | Network discovery, port scanning, service enumeration |
| Wireshark | Packet capture and protocol analysis |
| netstat | Active connection monitoring |
| netcat | Bind shell exploitation testing |
| telnet | Unencrypted login verification |
| ftp | vsftpd backdoor trigger testing |

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `penetration_test_report.pdf` | Complete professional penetration test report |
| `nmap_output.txt` | Raw nmap service version scan output |
| `wireshark_captures.pcap` | Packet capture files from Wireshark |
| `screenshots/` | Evidence screenshots from all testing phases |

## 🎯 Key Findings Summary

- **Total Open Ports:** 23
- **Critical Vulnerabilities:** 9
- **High Risk:** 1
- **Medium Risk:** 9
- **Low Risk:** 2

### Top Critical Findings:
1. 🔴 **vsftpd 2.3.4 Backdoor** (Port 21) — Smile trigger `:) ` opens root shell
2. 🔴 **Bind Shell** (Port 1524) — Direct root access with no authentication
3. 🔴 **Telnet Plaintext** (Port 23) — Credentials sent unencrypted
4. 🔴 **MySQL No Password** (Port 3306) — Empty root password
5. 🔴 **Outdated Apache 2.2.8** (Port 80) — Multiple known exploits

## 📸 Evidence

All screenshots are in the `screenshots/` folder, including:
- Network discovery and host verification
- nmap scanning results (basic, service version, aggressive)
- Successful exploitation (bind shell, telnet, vsftpd backdoor)
- Wireshark packet captures showing plaintext credentials

## ⚠️ Legal Notice

This penetration test was conducted on an **isolated virtual lab environment** (Metasploitable2) 
with full authorization for educational purposes only. No testing was performed on any production 
or third-party systems.

---

**Report Generated:** July 2026  
**Classification:** CONFIDENTIAL — For CloudExify Internship Use Only
