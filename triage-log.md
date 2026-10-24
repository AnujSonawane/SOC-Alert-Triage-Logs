# SOC Alert Triage Log

## Alert #1
**Alert Date:** 2021-04-26T23:03:14+03:00 
**Closed Date:** 2026-10-24T13:17:59.970220+00:00
**Alert Title:** Password Stealer Detected  
**Severity:** Medium  
**Source IP:** Malicious attachment through Email  
**Target:** user@example.com

**Hypothesis:** The provided alert is a TP, Phishing email was set to the users account with not title and content. Email contains a malicious HTML attachment which opens a fake login prompt to steal user data. 

**Evidence:**
- Mail with no Title and content
- Mail attached with malicious HTML fake login - hash value - bd05664f01205fa90774f42468a8743a
- No outgoing/incoming connection to C2 and malicious payload was not downloaded in the users system 

**Classification:** True Positive - Malicious  
**Action Taken:** Deleted mail from user account
**Time to Triage:** 8 minutes  

---

