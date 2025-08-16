# Vulnerability Scan Report  

## 📊 Scan Summary  
- **Scanner Used**: Nessus Essentials  
- **Target**: Localhost (127.0.0.1)  
- **Scan Type**: Full Scan  
- **Duration**: ~50 minutes  
- **Result**: Detected multiple vulnerabilities of varying severity levels.  

---

## 🐞 Common Vulnerabilities Found  
1. **Outdated Software Versions**  
   - Some applications were flagged as outdated and missing security patches.  
   - Risk: Exploitable by known CVEs.  

2. **Weak SSL/TLS Configurations**  
   - Detected support for deprecated SSL protocols (TLS 1.0/1.1).  
   - Risk: Could allow man-in-the-middle attacks.  

3. **Open Ports**  
   - Several unnecessary ports were open on localhost.  
   - Risk: Could be exploited for unauthorized access.  

4. **Default/Weak Credentials (Potential Risk)**  
   - Scanner suggested that common/default credentials may still exist for certain services.  
   - Risk: Easy target for brute-force attacks.  

---

## 📌 Observations  
- Most vulnerabilities were related to **patch management** (outdated apps).  
- Misconfigured network services and unnecessary open ports increase attack surface.  
- Critical vulnerabilities usually require **immediate patching or mitigation**.  

---

## 🧠 Key Learnings  
1. **Vulnerability Scanning vs. Penetration Testing**  
   - Scanning = detection of known issues.  
   - Penetration Testing = exploitation to validate the impact.  

2. **Importance of CVSS**  
   - Helps in prioritizing vulnerabilities based on severity (Critical > High > Medium > Low).  

3. **Remediation Approach**  
   - Apply software updates and patches.  
   - Disable unnecessary services and ports.  
   - Strengthen password policies.  

4. **Scanning Frequency**  
   - Regular vulnerability scans are essential to keep systems secure.  

---

## ✅ Conclusion  
This task provided hands-on experience with vulnerability scanning, risk identification, and understanding how security tools work in real environments. It highlighted the importance of continuous monitoring, timely patching, and prioritization of vulnerabilities in order to maintain a secure system.  
