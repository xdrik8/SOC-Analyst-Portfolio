# Phishing Investigation Report – Case 01

**Date:** 2025-02-15  
**Analyst:** Indira  
**Category:** Phishing Email Analysis

---

## 📌 Summary
A suspicious email was reported by a user claiming they received an urgent request to update their bank details. The email contained a malicious URL redirecting to a credential-harvesting phishing site.

---

## 📨 Email Header Analysis
- Sender: `support@account-securebank.com`
- Envelope From: Unknown SMTP server
- SPF: **Fail**
- DKIM: Not signed
- Return-Path: Different from sender domain

**Indicators of compromise:**
- Domain is newly registered  
- Suspicious URL shortener present  
- Mismatch between display name and actual email  

---

## 🔗 Malicious URL Analysis
Tools used:
- VirusTotal  
- URLScan  
- Talos Intelligence  

**URL Result:**  
- 12/90 engines flagged as malicious  
- Hosted on Russian VPS  
- Contains HTML credential-stealing script  

---

## ✔ Conclusion
**Confirmed Phishing Attack**  
The email attempted to steal banking credentials using a fake login page.

---

## 🛡 Recommendations
- Block sender domain  
- Add domain to email security filter  
- Notify affected users  
- Conduct phishing awareness training  
