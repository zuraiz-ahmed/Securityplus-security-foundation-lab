# Incident Analysis Report

## 1. Summary
A user account (jdoe) experienced multiple failed login attempts followed by a successful login. After gaining access, the account accessed and modified a sensitive payroll file, indicating potential unauthorized access or account compromise.

## 2. CIA Triad Impact
- Confidentiality: The payroll file may have been exposed to an unauthorized user.
- Integrity: The payroll file was modified, compromising data accuracy.
- Availability: There is no indication that system availability was affected.

## 3. AAA Mapping
- Authentication: Multiple failed login attempts followed by a successful login suggest possible brute-force or credential compromise.
- Authorization: The user gained access to a sensitive payroll file, indicating excessive or misconfigured permissions.
- Accounting: The system logs captured login attempts, file access, and modification activity, enabling detection and investigation.

## 4. Threat, Vulnerability, Exploit, and Risk
- Threat: A potentially malicious or compromised user account (jdoe).
- Vulnerability: Weak authentication mechanisms and improper access controls.
- Exploit: Unauthorized access and modification of the payroll file.
- Risk: Loss of data integrity and confidentiality, potentially impacting financial accuracy and organizational trust.

## 5. Security Controls
- Preventive: Strong password policies and multi-factor authentication (MFA).
- Detective: Log monitoring and alerting systems.
- Corrective: Incident response actions such as resetting credentials and restoring files from backup.
- Deterrent: Security policies and user awareness training.

## 6. SOC Analyst Response
- Initial action: Investigate suspicious login activity and confirm whether the account is compromised.
- Logs to review: Authentication logs, file access logs, and system event logs.
- Containment steps: Disable or lock the affected account, reset credentials, and restore affected data if necessary.
