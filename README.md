# 🚨 SIEM Incident Response Lab

## Overview

This project simulates a realistic cybersecurity incident within a controlled lab environment using a SIEM platform.

The goal is to demonstrate how security events are **collected, correlated, and analyzed** to detect and respond to a potential intrusion.

---

## Simulated Incident

The lab simulates a security incident involving unauthorized access and privilege escalation:

- Multiple failed authentication attempts on the target system  
- Successful SSH authentication on the target system
- Execution of privileged commands via `sudo`  
- Creation of a new user account as a persistence mechanism  
- Log collection and correlation via :contentReference[oaicite:0]{index=0}

The SIEM detects suspicious authentication patterns and privilege escalation activity.

Detailed step-by-step analysis is available in the `phases/` directory.

---

## Workflow

The project is structured into the following phases:

1. Environment Setup
2. Wazuh Installation
3. Agent Setup
4. Security Incident Detection
5. Log Analysis and Incident Investigation
6. Final Report

Each phase documents both **technical configuration and analytical reasoning**.

---

## Lab Architecture

The environment consists of three virtual machines:

* **SIEM Platform:** Wazuh Server
* **Monitored Host:** Ubuntu Server
* **Attacker Machine:** Kali Linux

### Network Configuration

* NAT (internet access)
* Host-Only Network (internal communication between machines)

---

## What You Will Find in `phases/`

* Step-by-step SIEM deployment and configuration
* Real log samples (e.g. `/var/log/auth.log`)
* Detection of authentication anomalies and privilege escalation activity
* Event correlation and incident investigation workflow
* Final incident report with findings and conclusions

---

## Key Skills Demonstrated

* SIEM deployment and configuration
* Log collection, parsing, and analysis
* Security event detection and alerting
* Incident investigation methodology
* Threat identification and interpretation
* Technical reporting and communication

---

## Tools Used

* Wazuh
* Ubuntu Server
* Kali Linux

---

## Project Outcome

This project demonstrates practical skills in:

* Security monitoring and centralized logging
* Detection of unauthorized access attempts
* Analysis of authentication logs and attack patterns

It highlights how a SIEM like Wazuh can be used to **identify threats early and support incident response activities** in a real-world scenario.
