# Casa-IDS-Lab


> **Demonstration of a simple but effective IDS lab with Snort & Splunk in a VM Environment**

## 🧠 Project Goal
To simulate and detect suspicious or malicious network activity using Snort 3.x as IDS and visualize the data using Splunk in a virtualized lab setup. Designed for home defenders, aspiring analysts, and red teamers.

---

## 🧰 Stack
- **Virtualization**: VirtualBox (Windows 11 Pro VM)
- **IDS**: Snort 3.x (manual rules + test rules)
- **Logging/Monitoring**: Splunk (free license)
- **Traffic Analysis**: Wireshark
- **Forwarding**: Syslog integration

---

## 📁 Folder Structure
```
Casa-IDS-Lab/
├── docs/                # Diagrams, setup explanations
├── configs/             # Snort rules, Splunk queries
├── src/                 # Helper scripts (log forwarders etc.)
├── pcaps/               # Test traffic (optional)
├── screenshots/         # Lab demonstration visuals
└── README.md            # This file
```

---

## 🚀 Lab Objectives
1. Install and configure Snort 3.x on the VM
2. Create and test 3+ custom detection rules
3. Forward logs to Splunk
4. Visualize traffic & alerts with Splunk queries
5. Validate alerts with Wireshark (proof of detection)

---

## 🛡️ Detection Focus
- Ping sweeps / port scans
- Suspicious HTTP headers or patterns
- Abnormal SSH behavior (future)

---

## 🔧 Possible Extensions
- Alert forwarding to messenger (e.g. Element )
- Metasploit simulated attack and Snort response
- Bash script for full lab deployment

---

## 📌 Author
**Sergiu-Gelu Stoica**  
[LinkedIn](https://linkedin.com/in/sergiu-gelu-stoica-it)

---

## 💡 Inspiration
Because home defense starts with understanding the attacks. This lab helps build exactly that mindset.
