DoS Attack & Mitigation Lab (MikroTik) 

Practical laboratory to simulate and mitigate DDoS attacks in a controlled infrastructure

📋 Scenario Overview
- Router: MikroTik RouterOS (RB750Gr3)
- Attacker: Kali Linux (VM VirtualBox)
- Target: Network Gateway
- Objective: Analyze router behavior during a SYN Flood attack and implement firewall mitigations

🚀 Lab Steps

 1. Baseline Observation
Monitored the router's CPU and connection table in a clean state to understand normal system behavior

 2. The Attack (SYN Flood)
Generated a high volume of SYN packets using Kali Linux
- Result: Sudden CPU spike, dozens of open TCP connections, and high log activity

 3. Mitigation Strategies
Implemented layered defenses in MikroTik RouterOS:
- TCP SYN Cookies:** Activated to handle incomplete handshakes
- Firewall RAW Rules:** Dropped malicious traffic at the prerouting stage to save CPU resources
- Connection Limiting:** Restricted the number of simultaneous connections per IP

✅ Final Results
After applying the rules, the firewall successfully dropped the attack packets. The router remained stable and accessible even under heavy attack

🛠️ Tools Used
- MikroTik RouterOS / WinBox
- Kali Linux (hping3/nmap)
- Oracle VM VirtualBox
