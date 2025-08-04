# cybersecurity-internship-elevate-labs
# 🔐 Cyber Security Internship Task 1: Port Scanning

## 📌 Objective
  --To perform network reconnaissance using Zenmap (Nmap GUI) and analyze packet data with Wireshark.

---

## 🧰 Tools Used
- **Zenmap** for TCP SYN scanning
- **Wireshark** for packet capture
- **Windows cmd** (`ipconfig`) to identify local network IP

---

## 🔍 Target Network
- **Local IP:** 10.51.100.219
- **Subnet:** 255.255.255.0 → **Scanned Range:** `10.51.100.0/24`

---

## 📊 Scan Results

### 1. Host: `10.51.100.182`
- **Port 53 (DNS)** – Open  
  → Likely DNS service  
  → Risk: Could be exploited for DNS amplification if exposed

### 2. Host: `10.51.100.219` (My Device)
- **Port 135 (MSRPC)** – Windows service
- **Port 139 (NetBIOS-SSN)** – File sharing
- **Port 445 (Microsoft-DS)** – SMB  
  → Risks: Exploited in ransomware attacks like WannaCry  
  → Recommendation: Close unused ports or apply firewall rules

---

## 🧪 Wireshark Analysis

Captured packet data during scanning. Key points:
- SYN packets sent to detect open ports
- TCP handshake attempts visible
- Useful for validating scan behavior

File: `task1.pcapng` (included)

---

## ✅ Outcome
- Learned how to identify live hosts and open ports using Zenmap.
- Understood potential risks of exposed services.
- Observed scanning behavior in Wireshark to complement port analysis.

---

## 📎 Files Included
- `scan_results_nmap` – Raw Nmap scan nmap
- `task1.pcapng` – Wireshark capture



