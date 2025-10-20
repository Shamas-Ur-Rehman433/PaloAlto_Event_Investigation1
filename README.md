<img width="1076" height="449" alt="14" src="https://github.com/user-attachments/assets/e4b5d19f-ab68-4325-a7da-7b4336d4264f" /># PaloAlto_Event_Investigation1
Dissecting and explaining every part of a Palo Alto Networks threat log entry for cybersecurity and SOC training.


---

### 🕓 1. Timestamp
- **Value:** `Sep 9 17:14:23`
- **Meaning:** Date and time the log was generated.
<img width="1079" height="498" alt="1" src="https://github.com/user-attachments/assets/9ad13ef3-97bc-45ba-a14a-96047507daf9" />

---

### 🌐 2. Source Device
- **Value:** `10.131.24.13/10.131.24.13`
- **Meaning:** IP address of the Palo Alto Firewall sending logs via Panorama.
<img width="1077" height="465" alt="2" src="https://github.com/user-attachments/assets/5a53b339-9e87-4cb2-8848-bcc79376f6e5" />

---

### 🧠 3. Log Source Type
- **Value:** `panfw_via_panorama`
- **Meaning:** Log forwarded through Panorama from the firewall.
<img width="1078" height="473" alt="3" src="https://github.com/user-attachments/assets/afebed7e-e410-45bf-81b8-216a63f6a2d0" />

---

### 🧾 4. Log Version and Date
- **Value:** `v1: 1,2020/09/09`
- **Meaning:** Log format version and creation date.
<img width="1080" height="443" alt="4" src="https://github.com/user-attachments/assets/b394abd0-663b-41a2-a8eb-98c44042dd9b" />

---

### ⚠️ 5. Log Type
- **Value:** `THREAT, url`
- **Meaning:** Indicates a **Threat Log** of subtype **URL Filtering**.
<img width="1080" height="458" alt="5" src="https://github.com/user-attachments/assets/95125810-fefa-4223-80b9-2da1fab3a929" />

---

### 🔢 6. Log ID
- **Value:** `020100177`
- **Meaning:** Unique identifier for this log event.
<img width="1079" height="443" alt="6" src="https://github.com/user-attachments/assets/e8c7f28e-3666-4f75-9ed4-defd3071ca54" />

---

### 🏷️ 7. Virtual System
- **Value:** `vsys 1`
- **Meaning:** Virtual system where traffic was inspected.
<img width="1080" height="448" alt="7" src="https://github.com/user-attachments/assets/3cef0dde-e120-4781-8b95-bdc46558e880" />

---

### 💻 8. Source and Destination IPs
- **Source:** `10.60.3.123`  
- **Destination:** `120.44.239.154`  
- **NAT / Intermediate:** `19.31.169.76`  
- **Meaning:** Shows user, destination, and translated IPs.
<img width="1076" height="460" alt="8" src="https://github.com/user-attachments/assets/55ca9ce5-b8eb-4d6a-a9d2-f5b420fc2016" />

---

### 🌍 9. Security Policy
- **Value:** `AO - Internet Access`
- **Meaning:** Rule allowing internal users outbound internet access.
<img width="1079" height="450" alt="9" src="https://github.com/user-attachments/assets/396ce2ee-de9e-4ea8-8df8-e77e19edbce5" />

---

### ⚙️ 10. Application
- **Value:** `ssl`
- **Meaning:** Identified application (HTTPS traffic).
<img width="1079" height="440" alt="10" src="https://github.com/user-attachments/assets/2986937a-add1-46bd-beb3-03ec5f6ec2f1" />

---

### 🧩 11. Zones
- **Source Zone:** Inside  
- **Destination Zone:** Internet  
- **Meaning:** Traffic flowed from internal to external network.
<img width="1087" height="436" alt="11" src="https://github.com/user-attachments/assets/f352700c-187f-4f7e-a146-cd5088feae39" />

---

### 🔌 12. Interfaces
- **Source Interface:** `ae1.3`  
- **Destination Interface:** `ae1.1`
<img width="1082" height="430" alt="12" src="https://github.com/user-attachments/assets/f7fb600f-04d7-46bd-9eb4-74fb2d28f925" />

---

### 📜 13. Rule / Profile
- **Value:** `LFP - SE, Forwarding Default`
- **Meaning:** Security rule name and action profile used.
<img width="1079" height="435" alt="13" src="https://github.com/user-attachments/assets/d21d5e0c-514f-4f74-b285-14f04cc1cb10" />

---

### ⏰ 14. Event Time
- **Value:** `2020/09/09 17:39:51`
- **Meaning:** Exact time of the detected event.
<img width="1076" height="449" alt="14" src="https://github.com/user-attachments/assets/43ca5994-e5c0-45a8-a9e9-fd8850a7639f" />

---

### 🔑 15. Session Details
- **Session ID:** `672863`  
- **Source Port:** `64422`  
- **Destination Port:** `443 (HTTPS)`  
- **NAT Source Port:** `19882`  
- **Meaning:** TCP connection details of this session.
<img width="1075" height="424" alt="15" src="https://github.com/user-attachments/assets/5bd8b924-d410-482f-92da-5a871f3ae1a9" />

---

### 🔁 16. Session Flags
- **Value:** `0x40b000`
- **Meaning:** Encodes attributes like NAT, SSL inspection, TCP flags, etc.
<img width="1080" height="430" alt="16" src="https://github.com/user-attachments/assets/2051cef7-6c6b-48ef-ac5a-93f0e45adae5" />

---

### 🔒 17. Protocol
- **Value:** `tcp`
- **Meaning:** Transport layer protocol used.
<img width="1081" height="447" alt="17" src="https://github.com/user-attachments/assets/c1e3980c-b767-4295-95de-60a0f14061ee" />

---

### 🚨 18. Action
- **Value:** `alert`
- **Meaning:** Firewall allowed traffic but logged it for monitoring.
<img width="1081" height="433" alt="18" src="https://github.com/user-attachments/assets/2a60fce5-7339-423f-935e-a7379f067128" />

---

### 🌐 19. URL Accessed
- **Value:** `settings-win.data.microsoft.com`
- **Meaning:** The domain or website requested.
<img width="1075" height="434" alt="19" src="https://github.com/user-attachments/assets/628788d3-be14-4ffb-94bc-5f6ef184b682" />

---

### 🏷️ 20. URL Category
- **Value:** `computer-and-internet-info`
- **Meaning:** Categorized as informational content.
<img width="1080" height="438" alt="20" src="https://github.com/user-attachments/assets/2293357d-8763-45a2-8ac5-4b481f3577b7" />

---

### ⚠️ 21. Threat Severity
- **Value:** `informational`
- **Meaning:** Low-risk log; no malicious activity detected.
<img width="1080" height="456" alt="21" src="https://github.com/user-attachments/assets/843116eb-86b8-4733-9a6b-02adc48b6861" />

---

### 🌍 22. Destination Country
- **Value:** `Singapore`
- **Meaning:** Geolocation of the destination IP.
<img width="1086" height="436" alt="22" src="https://github.com/user-attachments/assets/71ebf46e-3be8-4786-a25f-e22bd50f2510" />

---

### 🧱 23. Device Info
- **Value:** `SESYDVIR-FW01.0.0`
- **Meaning:** Hostname or identifier of the firewall device.
<img width="1079" height="454" alt="23" src="https://github.com/user-attachments/assets/2f60e3dc-f286-4514-a8ab-38fe3332b1a4" />

---

### 📂 24. Threat Name / ID
- **Value:** `computer-and-internet-info, low-risk 9bd38d49-07d6-4ddb-a86b-af2ec370d943`
- **Meaning:** Threat category and unique Palo Alto threat ID.
<img width="1079" height="456" alt="24" src="https://github.com/user-attachments/assets/493d2670-5e7b-43aa-9dc1-056d1e55427d" />

---

### 🧩 25. AppThreat ID
- **Value:** `AppThreat-0-0`
- **Meaning:** Indicates a URL filtering log, not a malware or exploit.
<img width="1080" height="443" alt="25" src="https://github.com/user-attachments/assets/feb33f98-3e3f-4130-892f-66f1d1ecd306" />

---

### 🧮 26. Session Counters
- **Values:** `477, 481, 484`  
- **Meaning:** Bytes or packets exchanged in this session.
<img width="1079" height="463" alt="26" src="https://github.com/user-attachments/assets/bf0f2b39-e02b-49a5-8bb0-76306a6d27d2" />

---

### 📊 27. Risk Level
- **Value:** `low-risk`
- **Meaning:** Rated as non-malicious by the firewall.
<img width="1076" height="443" alt="27" src="https://github.com/user-attachments/assets/2d456f17-0552-4f15-8c2c-bda6f7ea7279" />

---

## ✅ Summary Interpretation

- A user with IP **10.60.3.123** accessed **settings-win.data.microsoft.com** (Microsoft telemetry domain).  
- Palo Alto Firewall categorized it as **computer-and-internet-info** and marked it **informational** (not malicious).  
- Traffic was **Inside → Internet**, using **TCP port 443**, and passed through the policy **AO - Internet Access**.  
- The connection was logged but **not blocked**, with a **low risk** rating.

---

### 📘 Author
Created by **Shamas Ur Rehman**  
GitHub Lab: *Firewall Threat Log Analysis*

