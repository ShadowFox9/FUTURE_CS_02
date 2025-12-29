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
