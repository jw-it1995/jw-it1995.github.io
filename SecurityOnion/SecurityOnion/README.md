# 🧅 Security Onion SOC Lab

This project demonstrates my hands-on experience setting up and using **Security Onion** as a SOC (Security Operations Center) platform. I installed it in VirtualBox, configured the environment, generated alerts using `so-test`, and investigated suspicious traffic.

---

## 🖥️ Lab Environment
- **Host Machine:** Windows 11 Pro, Intel i7, 16 GB RAM
- **Virtualization:** Oracle VirtualBox 7.0
- **Guest VM:** Security Onion 2.4 (ISO install)
- **Resources:** 4 vCPU, 8 GB RAM, 100 GB disk
- **Networking:**  
  - Adapter 1: Bridged Adapter (to capture local network traffic)  
  - Adapter 2: Internal Network (lab segmentation)

This setup simulates a small SOC environment and provides visibility into network events, alerts, and suspicious activity.

---

## 1. Login Page  
![Login Screenshot](screenshots/login.png)  
- Shows successful setup and access to the SOC web console.  
- **Skills:** VM configuration, network setup, SOC access.

---

## 2. List of Alerts  
![Alerts Screenshot](screenshots/alerts.png)  
- Security Onion generated multiple alerts (e.g., Zbot malware, suspicious SMB traffic).  
- **Skills:** Alert recognition, SIEM triage, distinguishing severity levels.

---

## 3. Expanded Alert Details  
![Alert Details Screenshot](screenshots/alert_details.png)  
- Example: `ET MALWARE Zbot Generic URI/Header Struct .bin`.  
- I reviewed the IP (`188.72.243.72`), ASN (Webzilla B.V.), and geolocation (Netherlands).  
- **Skills:** Alert investigation, threat intelligence basics.

---

## 4. Hunt Query  
![Hunt Query Screenshot](screenshots/hunt.png)  
- Queried suspicious IP in Hunt interface to see more logs and events.  
- **Skills:** Threat hunting, correlation of IDS + log data.

---

## 5. Dashboards  
![Dashboard Screenshot](screenshots/dashboard.png)  
- Shows Security Onion dashboards with metrics and traffic patterns.  
- **Skills:** Data visualization, SOC monitoring.

---

## 🔑 Key Takeaways
- Installed and configured Security Onion from scratch.
- Performed **alert → expand → hunt → verify** workflow.
- Investigated Zbot malware alert and extracted indicators (IP, ASN, country).
- Developed SOC analyst skills: triage, investigation, and documentation.
- Built a virtualized SOC environment using Oracle VirtualBox for hands-on practice.

---

