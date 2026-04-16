# Phase 05 – Incident Analysis and Response

## Objective

The objective of this phase is to analyze the detected security incident, understand its impact, and propose appropriate response actions.

---

## Incident Overview

During monitoring activities, multiple alerts were generated indicating suspicious behavior on the Ubuntu server.

The events suggest that a user account performed unauthorized privileged actions, including repeated failed attempts to execute sudo commands, successful privilege escalation, and the creation of a new user account.

This behavior is consistent with a potential account compromise.

---

## Timeline of Events

The incident followed a clear sequence:

1. Multiple failed attempts to execute privileged commands using `sudo`
2. Successful privilege escalation to root access
3. Creation of a new user account (`backdoor_user`)

This sequence indicates a progression from initial access attempts to full system control and persistence.

---

## Analysis

The detected activity indicates a potential compromise of a legitimate user account.

The repeated failed sudo attempts suggest that the attacker was trying to gain elevated privileges.
Once successful, the attacker executed privileged commands and created a new user account.

The creation of a new account represents a persistence mechanism, allowing continued access to the system.

---

## Impact Assessment

If this incident occurred in a real environment, the impact could be significant:

* Full administrative access to the system
* Ability to modify or delete sensitive data
* Potential lateral movement to other systems
* Long-term persistence through unauthorized accounts

---

## Response and Recommendations

To mitigate and prevent similar incidents, the following actions are recommended:

* Enforce strong password policies
* Limit sudo privileges to necessary users only
* Monitor and alert on failed sudo attempts
* Regularly audit user accounts and remove unauthorized ones
* Implement multi-factor authentication (MFA)
* Enable detailed logging and continuous monitoring

---

## Conclusion

The SIEM successfully detected the suspicious activity and provided visibility into the attack progression.

This phase demonstrates the importance of log analysis and proactive monitoring in identifying and responding to potential security incidents.
