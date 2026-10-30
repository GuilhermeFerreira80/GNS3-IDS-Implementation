# Implementation and Analysis of an Intrusion Detection System (IDS) with Suricata

Project developed for the **Cybersecurity** course as part of the BSc in Informatics Engineering at **ISEC** (Coimbra Institute of Engineering)

### Overview
This project focuses on the implementation, configuration, and experimental validation of **Suricata IDS** within a segmented network environment (WAN, LAN, and DMZ) simulated in **GNS3**, running on top of **Security Onion**.

The sensor was deployed in a passive (*Out-of-Band*) monitoring setup via a DMZ hub to inspect traffic targeting critical services without introducing network latency or single points of failure. Custom signature rules with event thresholds were implemented to effectively prevent alert fatigue.

### Tested Attack Scenarios
- **Network Reconnaissance:** TCP SYN port scanning using Nmap.
- **Brute Force:** Automated SSH credential-guessing attacks using Hydra.
- **Denial of Service (DoS):** Volumetric ICMP and UDP flood attacks using hping3.
- **Baseline Connectivity:** ICMP Echo Request analysis to validate signature parsing and rule coexistence.

### Tech Stack & Tools
- **IDS & Platform:** Suricata, Security Onion
- **Network Simulation:** GNS3
- **Security Auditing & Attack Tools:** Kali Linux (Nmap, Hydra, hping3)
