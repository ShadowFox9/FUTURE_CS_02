## SOC-001: Repeated Failed Login Attempts

**Alert Type:** Brute Force / Authentication Abuse  
**Severity:** High  
**Data Source:** Splunk (soc_task2_logs)

**Description:**  
Multiple failed login attempts were detected from the same IP addresses over a short period, indicating a possible brute-force attack.

**Potential Impact:**  
Account compromise, unauthorized access, credential stuffing.

**Evidence:**  
See screenshot: `SOC-001_Repeated_Failed_Login_Attempts.png`

**Recommended Response:**  
- Block or rate-limit offending IPs  
- Enable account lockout policies  
- Monitor for successful login attempts from the same IPs

- ## SOC-002: Suspicious IP Activity

**Alert Type:** Anomalous Network Activity  
**Severity:** Medium  
**Data Source:** Splunk (soc_task2_logs)

**Description:**  
Repeated or unusual network connections were observed from a specific IP address, suggesting potential reconnaissance or misuse.

**Potential Impact:**  
Unauthorized access attempts, service abuse, data scraping.

**Evidence:**  
See screenshot: `SOC-002_Suspicious_IP_Activity.png`

**Recommended Response:**  
- Investigate IP reputation  
- Apply rate limiting or blocking if malicious  
- Continue monitoring for escalation

