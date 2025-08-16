# Task 4: Firewall Configuration and Testing

## 📌 Objective  
The objective of this task was to configure and test basic firewall rules to allow or block traffic on specific ports using **Windows Defender Firewall with Advanced Security**.

---

## 🛠 Tools Used  
- **Windows 11** (Host machine)  
- **Windows Defender Firewall with Advanced Security**  
- **PowerShell** (for rule creation, testing, and verification)  
- **Python (http.server module)** for simulating services on custom ports  

---

## 🔍 Steps Performed  

1. **Viewed current firewall rules**  
   - Opened *Windows Defender Firewall with Advanced Security* → Inbound Rules.  
   - Verified existing rules including system and application-specific rules.  

2. **Created a block rule for Telnet (TCP 23)**  
   - Used GUI to add a new inbound rule named **Block Telnet TCP 23**.  
   - Action: Block inbound connections on port 23 (TCP).  

3. **Tested connectivity using PowerShell**  
   - Started a temporary listener with Python on port **2323**:  
     ```powershell
     python -m http.server 2323
     ```  
   - Tested connectivity with:  
     ```powershell
     Test-NetConnection -ComputerName 127.0.0.1 -Port 2323
     ```  
   - Result: When blocked, connection failed. When unblocked, connection succeeded.  

4. **Created and tested a custom block rule (port 2323)**  
   - Created via PowerShell:  
     ```powershell
     New-NetFirewallRule -DisplayName "Block Test 2323" -Direction Inbound -Action Block -Protocol TCP -LocalPort 2323
     ```  
   - Verified with **Test-NetConnection** that the port was blocked.  

5. **Removed the block rule**  
   - Deleted the rule after testing to restore original firewall state.  
   - Verified deletion by checking Inbound Rules list and confirming successful connection test.  

---

## 📑 Deliverables  
- Screenshots of firewall rules and PowerShell test outputs (included in report).  
- **report.docx** with observations, outputs, and learnings.  

---

## 🚀 Outcome  
This task provided practical experience with:  
- Creating and deleting firewall rules.  
- Understanding inbound vs outbound rules.  
- Using PowerShell commands to test firewall effects.  
- Demonstrating how firewalls filter and control traffic.  
