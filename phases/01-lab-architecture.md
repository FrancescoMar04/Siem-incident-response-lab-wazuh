# Phase 01 - Lab Architecture and Environment Setup

## Objective
The objective of this phase is to design and prepare the lab environment required to simulate a security incident and perform SIEM-based analysis.

---

## Lab Architecture

The lab environment consists of three virtual machines:

- Wazuh Server (SIEM platform)
- Ubuntu Server (monitored host / victim)
- Kali Linux (attacker machine)

---

## Network Configuration

The environment is configured using:

- NAT network for internet access
- Host-Only network for internal communication between machines

This configuartion allows controlled interaction between the attacker and the victim system.

---

## Roles and Responabilities

- Kali Linux is used to simulate malicious activity
- Ubuntu Server generates logs and acts as the monitored system
- Wazuh Server collects, analyzes, and correlates security events

---

## Outcome

The lab environment is successfully configured and ready for SIEM deployment and monitoring activities.
