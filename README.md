 DDoS Mitigation Lab - MikroTik & Kali Linux

This repository documents my hands-on laboratory for simulating DoS attacks and implementing defense strategies

##  Overview
The goal of this lab was to test how a router reacts to various attack vectors and how firewall rules can effectively mitigate these threats in a real-world scenario

##  🛠️ Environment
* Hardware: RouterBoard RB750Gr3
* Firewall: MikroTik RouterOS
* Attacker: Kali Linux
* Target:VM environment via Oracle VirtualBox

## Key Steps
1. Attack Simulation:** Executed a **SYN Flood** attack using Kali Linux, observing high CPU spikes and connection exhaustion
2. Mitigation:** Implemented **TCP SYN Cookies** and **Firewall RAW/Prerouting** rules
3. Result:** Successfully dropped malicious packets, maintaining router stability under stress

##  Status
* **Lab Status:** Active Study & Practice
* **Focus:** Blue Team / Network Security
