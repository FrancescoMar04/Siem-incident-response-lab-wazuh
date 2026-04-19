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

This configuration allows controlled interaction between the attacker and the victim system.

---

## Roles and Responsibilities

- Kali Linux is used to simulate malicious activity
- Ubuntu Server generates logs and acts as the monitored system
- Wazuh Server collects logs from monitored endpoints, analyzes them, and correlates security events

The monitored host (Ubuntu Server) generates system and authentication logs, which are forwarded to the Wazuh server for analysis.

---

## Outcome

The lab environment is successfully configured, and communication between all machines is verified. The system is ready for SIEM deployment, log collection, and monitoring activities.
