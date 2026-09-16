# 🛡️ Network Penetration Testing & Reconnaissance Report

## 📌 Project Overview
This repository contains the official documentation and findings from a comprehensive Network Security & Penetration Testing internship task. The project covers passive footprinting against public targets and active host discovery/network scanning in an isolated lab environment using **Kali Linux** and **VirtualBox**.

## 📄 Key Deliverables
- 📜 **Full PDF Report:** [Download Penetration Testing Report](./PENETRATION%20TESTING%20REPORT.pdf)
- 🖼️ **Lab Screenshots:** Uploaded in the repository directory.

## 🛠️ Tools & Technologies Used
- **OS:** Kali Linux 2025
- **Reconnaissance & Footprinting:** WHOIS, WhatWeb, Nslookup, Curl, Wafw00f, DNSRecon
- **Network Scanning & Discovery:** Zenmap (Nmap GUI)
- **Virtualization:** Oracle VM VirtualBox (NAT Network)

## 🚀 Key Modules Covered
1. **Passive Footprinting & Reconnaissance:** Target web stack analysis (WordPress, Apache), WAF identification (ModSecurity), and DNS record enumeration.
2. **Network Scanning & Topology Mapping:** Zenmap subnet scanning (`10.0.0.0/24`), active host discovery, and network layout visualization.
3. **Risk Analysis & Vulnerability Assessment:** Evaluating potential impact, attack vectors, and information exposure risks.
4. **Defensive Recommendations:** Actionable security hardening, header suppression, and REST API access restriction strategies.

---

## 📸 Step-by-Step Implementation & Evidences

### Step 1: Kali Linux Virtual Machine Setup
Initialized Kali Linux VM environment inside Oracle VirtualBox.
![Kali Linux Environment Setup](./week%202.PNG)

### Step 2: WHOIS Domain Reconnaissance
Extracted domain registration data, registrar info, creation dates, and authoritative name servers for `networkwalks.com`.
![WHOIS Output](./week2%20..PNG)

### Step 3: WhatWeb Technology Stack Fingerprinting
Identified target web server stack (Apache), CMS (WordPress 7.1), hosting IP, and system components.
![WhatWeb Output](./Capture%203.PNG)

### Step 4: Nslookup DNS IP Resolution
Queried public DNS server (8.8.8.8) to resolve `networkwalks.com` to its IPv4 address (`192.232.216.135`).
![Nslookup Query](./task%203.PNG)

### Step 5: HTTP Header & Server Analysis via Curl
Inspected HTTP response headers, HTTP/2 status codes (200 OK), server signatures, and active session cookies.
![Curl Header Inspection](./task%204.PNG)

### Step 6: Web Application Firewall (WAF) Detection
Executed Wafw00f utility and confirmed active protection behind **ModSecurity (SpiderLabs)** WAF.
![Wafw00f Detection](./task%205.PNG)

### Step 7: Comprehensive DNS Record Enumeration
Utilized DNSRecon to extract SOA, NS, MX, SPF, and active autodiscover SRV records.
![DNSRecon Enumeration](./task%206.PNG)

### Step 8: Zenmap Utility Initialization
Configured Zenmap GUI with `nmap -sn 10.0.0.0/24` target parameters for local subnet scanning.
![Zenmap Initialization](./task%207.PNG)

### Step 9: Zenmap Subnet Scanning & Host Discovery
Executed Nmap Ping Scan (`nmap -sn 10.0.0.0/24`) to discover active host nodes (`10.0.0.1`, `10.0.0.2`, `10.0.0.3`).
![Zenmap Host Discovery](./task%208.PNG)

### Step 10: Network Topology Mapping
Visualized internal subnet layout and host linkages in Zenmap interactive Topology viewer.
![Network Topology Map](./task%209.PNG)

---

Mentored by Networkwalks & Waqas Karim (CCIE)

*Disclaimer: This repository is intended strictly for educational and defensive security assessment purposes within an authorized environment.*
