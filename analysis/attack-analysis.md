# Attack Analysis Report

## Summary
The logs indicate a potential brute-force attack originating from IP address 192.168.1.100. The attacker performed multiple failed login attempts before successfully gaining access to the system.

## Observed Activity
- Multiple failed login attempts targeting the admin account
- Successful login following repeated failures
- Access to sensitive system file `/etc/shadow`
- Privilege escalation activity detected

## Indicators of Compromise
- Repeated failed authentication attempts
- Unauthorized access to sensitive files
- Privilege escalation event

## Analysis
The pattern of repeated failed logins followed by success strongly suggests a brute-force attack. The access to `/etc/shadow` indicates an attempt to retrieve password hashes. The privilege escalation event confirms that the attacker gained elevated access to the system.

## Impact
- Potential compromise of user credentials
- Loss of system integrity
- Increased risk of further system exploitation

## Recommended Actions
- Lock or disable the compromised account
- Enforce strong password policies and MFA
- Monitor login attempts and set alerts
- Restrict access to sensitive files
- Investigate the source IP address
