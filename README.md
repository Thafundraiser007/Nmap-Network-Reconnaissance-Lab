# Nmap-Network-Reconnaissance-Lab
<img width="857" height="272" alt="Screenshot 2026-07-14 222806" src="https://github.com/user-attachments/assets/4be38f19-81b1-4c59-ab90-ca5bdce315d9" />

# Nmap Network Reconnaissance Lab

## Project Overview

This project demonstrates basic network reconnaissance techniques using Nmap on a local network environment.

The purpose of this lab was to identify active hosts, perform service discovery, and document network scanning activities using Nmap, a widely used network scanning tool for network administrators and cybersecurity professionals.

All command screenshots, scan output screenshots, and exported Nmap result files are stored in their respective folders within this repository.

---

# Objectives

The objectives of this lab were:

* Identify local network information
* Determine the network subnet range
* Discover active hosts on the network
* Perform service and version detection scans
* Export Nmap scan results
* Document network reconnaissance activities

---

# Lab Environment

| Component          | Details                  |
| ------------------ | ------------------------ |
| Operating System   | Windows                  |
| Scanning Tool      | Nmap                     |
| Network Type       | Local Area Network (LAN) |
| Scanner IP Address | 10.55.165.88             |
| Subnet Mask        | 255.255.255.0            |
| Network Range      | 10.55.165.0/24           |
| Default Gateway    | 10.55.165.210            |

---

# Tools Used

| Tool                   | Purpose                                |
| ---------------------- | -------------------------------------- |
| Nmap                   | Network discovery and service scanning |
| Windows Command Prompt | Executing network commands             |
| GitHub                 | Documentation and version control      |

---

# Lab Process

## Step 1: Identify Local Network Configuration

Before performing network scanning, the local network information was collected to identify the IP address, subnet mask, and gateway.

Command used:

ipconfig

The information collected:

* IPv4 Address: 10.55.165.88
* Subnet Mask: 255.255.255.0
* Default Gateway: 10.55.165.210

The subnet was calculated as:

10.55.165.0/24

This allowed scanning of addresses between:

10.55.165.0 - 10.55.165.255

The command screenshot and output are stored inside the screenshots folder.

---

## Step 2: Host Discovery Scan

A host discovery scan was performed to identify active devices connected to the local network.

Command used:

nmap -sn 10.55.165.0/24

Explanation:

* -sn performs host discovery only
* 10.55.165.0/24 specifies the subnet being scanned

This scan identifies online hosts without performing a full port scan.

The scan results were exported using:

nmap -sn 10.55.165.0/24 -oN host-discovery.txt

The exported scan result file is stored inside the scan-results folder.

The command screenshot and scan output screenshot are stored inside the screenshots folder.

---

## Step 3: Service Version Detection Scan

A service detection scan was performed to identify open ports and running services on a target device.

Command used:

nmap -sV TARGET-IP

Example:

nmap -sV 10.55.165.210

Explanation:

* -sV enables service version detection
* Identifies services running on open ports
* Helps determine exposed network services

The scan results were exported using:

nmap -sV 10.55.165.210 -oN service-scan.txt

The exported scan result file is stored inside the scan-results folder.

The command screenshot and scan output screenshot are stored inside the screenshots folder.

---

# Repository Structure

Nmap-Network-Reconnaissance-Lab

├── README.md

├── screenshots

│   ├── Network Configuration Screenshot

│   ├── Host Discovery Scan Screenshot

│   └── Service Detection Scan Screenshot

│

└── scan-results

```
├── host-discovery.txt

└── service-scan.txt
```

---

# Skills Demonstrated

* IPv4 addressing
* Subnetting
* TCP/IP fundamentals
* Network reconnaissance
* Nmap scanning techniques
* Service enumeration
* Command-line networking tools
* Technical documentation

---

# Lab Results

Completed activities:

✅ Identified local network configuration

✅ Determined subnet range

✅ Performed host discovery scanning

✅ Identified active network devices

✅ Performed service version detection

✅ Exported Nmap scan results

✅ Documented network reconnaissance activities

---

# Future Improvements

Future improvements for this project include:

* Adding an Ubuntu Server target machine
* Performing advanced port scanning
* Performing operating system detection
* Testing firewall behaviour
* Performing vulnerability scanning
* Creating professional security assessment reports

---

# Conclusion

This lab provided practical hands-on experience using Nmap for network reconnaissance.

The project demonstrates fundamental networking and cybersecurity skills including:

* Network discovery
* IP addressing
* Service identification
* Security scanning methodology
* Technical documentation

This project forms part of my hands-on networking and cybersecurity portfolio.

---

#Author: Jamill Naipao
