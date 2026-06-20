# snort-ids-lab
# Snort IDS Home Lab

## Project Overview

This project demonstrates the installation, configuration, validation, and live network traffic monitoring using Snort 3 on Kali Linux. The objective was to deploy an Intrusion Detection System (IDS), validate its configuration, and analyze real-time ICMP network traffic.

---

## Tools Used

- Kali Linux
- Snort 3.12.2.0
- Nmap
- Git & GitHub

---

## Installation

Update the package list:

```bash
sudo apt update
```

Install Snort:

```bash
sudo apt install snort -y
```

---

## Verify Installation

```bash
snort -V
```

Expected Output:

```
Snort++ Version 3.12.2.0
```

---

## Validate Configuration

```bash
snort -T
```

Expected Output:

```
Snort successfully validated the configuration (with 0 warnings)
```

---

## Check Network Interface

```bash
ip a
```

Active Interface:

```
eth1
```

---

## Start Packet Capture

```bash
sudo snort -c /etc/snort/snort.lua -i eth1
```

---

## Generate Network Traffic

Open another terminal and run:

```bash
ping 8.8.8.8
```

---

## Sample Output

```
Packet Statistics

Received Packets : 73
Analyzed Packets : 73

ICMP Packets : 58

Runtime : 32 seconds
```

---

## Project Outcome

- Successfully installed Snort 3 on Kali Linux
- Validated Snort configuration
- Captured live network traffic
- Analyzed ICMP packets
- Monitored real-time packet flow
- Demonstrated IDS functionality

---

## Skills Gained

- Intrusion Detection System (IDS)
- Network Packet Analysis
- Snort 3 Configuration
- ICMP Traffic Monitoring
- Kali Linux
- Network Security
- Git & GitHub

---

## Screenshots

Add the following screenshots:

- Snort Version
- Configuration Validation
- Live Packet Capture
- Packet Statistics

---

## Repository Structure

```
Snort-IDS-HomeLab/
│
├── README.md
├── screenshots/
│   ├── snort-version.png
│   ├── configuration-validation.png
│   ├── packet-capture.png
│   └── packet-statistics.png
├── local.rules
├── snort_version.txt
└── validation.txt
```

---

## Author

**Mohit Kumar**

Cyber Security | SOC Analyst | Network Security | IDS | SIEM | Kali Linux
