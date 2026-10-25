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

## Alert #2  
**Alert Date:** 2024-09-24T08:21:15+03:00  
**Closed Date:** 2026-10-24T13:17:59.970220+00:00  
**Alert Title:** Unauthorized Cloud Region Access Attempt Detected / Web Attack  
**Severity:** Low  
**Source IP:** 134.xxx.xx.xx  
**Target:** 52.xx.xxx.xx

**Hypothesis:** Alert is True positive, There were 25+ login attempts which were blocked. No login attempts were attempted to other systems in the network.

**Evidence:**
- 25+ login attempts in under an hour to the unused cloud region. All login attempts blocked.
- Continuous Post request from unused cloud region.
- Linux AWS server - No syslog and authlogs present.
- Attacker IP 134[.]209.145.73

**Classification:** True Positive  
**Action Taken:** No action as login attempts already blocked
**Time to Triage:** 15 minutes  

---