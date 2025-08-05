# 🛡️ Cybersecurity Internship – Task 2: Phishing Email Analysis

## 🔍 Objective
To analyze a suspicious email for phishing characteristics, understand common attacker tactics, and identify email-based threats using real-world security tools.

---

## 📁 Task Description
Analyze a sample phishing email and identify the following:

- Spoofed sender address
- Header mismatches (SPF, DKIM, DMARC failures)
- Suspicious or mismatched links
- Social engineering and psychological manipulation
- Spelling or grammar issues
- Urgent or misleading language

---

## 🛠️ Tools Used
- 🔎 [MxToolbox – Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
- 🧪 [VirusTotal – URL Scanner](https://www.virustotal.com/)  
- 📨 Email client / image sample of phishing email  
- 📄 Markdown & Word for documentation

---

## 🚨 Phishing Indicators Identified

| Indicator                   | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| 🧑‍💻 **Spoofed Email**         | Domain `amaz0n-security.com` mimics legitimate Amazon domain              |
| ❌ **Authentication Failures** | SPF, DKIM, and DMARC all failed, indicating lack of sender verification   |
| 🔗 **Fake Login URL**        | Redirects to a fake Amazon login page to steal credentials                |
| 📝 **Urgent Tone**           | Attempts to create urgency with fake order information                    |
| ❓ **Unrated on VirusTotal** | URL appears clean but may be newly created for phishing                   |
| ⚠️ **IP from Private Network** | Originates from internal IP `192.168.1.100` – not a public email server     |
| 💬 **Generic Greeting**      | Uses "Hello ," instead of personalized name – a common phishing tactic     |

---

## ✅ Key Findings
- Sender domain was **spoofed** (`amaz0n-security.com`)
- Email failed **SPF**, **DKIM**, and **DMARC** authentication checks
- Embedded link (`amaz0n-alerts.com`) mimicked Amazon's login page
- Link appeared **clean** on VirusTotal, indicating **new or 0-day phishing**
- The email used **urgent language** and **trusted branding** to mislead users

---

## 📄 Files Included
- `README.md` – This summary file
- `Phishing.docx` – Detailed report with screenshots and step-by-step explanation
- `images/` – Folder containing all analysis tool screenshots

---

## 📚 Outcome
- Gained hands-on experience in phishing detection and header analysis
- Understood email authentication failures and domain spoofing
- Practiced using public threat analysis tools
- Developed a strong foundation in identifying phishing tactics

---

## 👩‍💻 Author
**Khushbu Chavda**  

