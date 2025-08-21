# LogAnalysis-UFW-Ubuntu
# 🚨 Log Analysis Basics: Network-Based Attacks on Ubuntu using UFW

This project is part of my journey through I focused on **analyzing firewall logs** to detect **network-based attacks** using **UFW (Uncomplicated Firewall)** on **Ubuntu LTS (Desktop)** in a home lab environment.

---

## 🛠️ Lab Setup

| Component      | Description                 |
|----------------|-----------------------------|
| OS             | Ubuntu 22.04 LTS (Desktop)  |
| Attacker       | Kali Linux (VirtualBox/VMware) |
| Firewall Tool  | UFW (Uncomplicated Firewall) |
| Attack Tool    | Nmap                        |
| Analysis Tools | grep, less, tail       |

---

## ✅ What I Did

- Enabled and configured **UFW** on Ubuntu LTS
- Ran simulated network-based attacks (Nmap scans, brute-force attempts) from Kali Linux
- Monitored firewall logs stored at `/var/log/ufw.log`
- Analyzed logs using Linux CLI tools
- Identified:
  - Suspicious IP addresses
  - Repeated denied attempts
  - Port scan patterns
  - TCP/UDP connection attempts

---

## 🔍 Commands Used

sudo ufw enable

sudo ufw status 

sudo tail -f /var/log/ufw.log

grep 'SRC=' /var/log/ufw.log 
