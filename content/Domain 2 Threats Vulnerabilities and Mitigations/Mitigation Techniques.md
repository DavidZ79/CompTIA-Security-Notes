---
title: 🛡️ Mitigation Techniques
description: 
draft: false
tags:
  - CompTIA
---

> [!quote] Definition
> **Mitigation techniques** are strategies and controls implemented to reduce the risk and impact of security threats and vulnerabilities. They help protect systems, data, and networks from compromise.

## Network Segmentation

Network segmentation divides a network into smaller parts to limit lateral movement and improve security.

<details>
<summary><strong>Segmentation Techniques</strong></summary>

- Physical segmentation: uses routers, switches, and firewalls
- Virtual Local Area Networks (VLANs): logical network segments within a single switch. Groups devices by department or function, reduces network traffic
- Subnetting: divides an IP network into smaller subnets, each with a subnet mask. Groups devices, efficient use of IP addresses
- Micro-segmentation: security policies for individual workloads or devices. Important in cloud environments and data centers

**Reasons for segmentation:**
- Enhanced security
- Access control
- Compliance requirements: Payment Card Industry Data Security Standard (PCI DSS) card payments in secure environment, among others
- Performance optimization: reduces broadcast domains
- Isolation of critical systems
- Scalability and agility

</details>

## Access Control

Access control restricts access to resources based on policies and user roles.

<details>
<summary><strong>Access Control Methods</strong></summary>

- Access Control Lists (ACLs) used by routers and firewalls. For files and folders, and for network traffic
- Application Allow List: whitelist
- Application Block List: prevents specific applications from running.
- Isolation: self-contained environments within a network for critical systems and data

</details>

## Patch Management and Encryption

Keeping systems up to date and encrypting data are fundamental mitigation strategies.

<details>
<summary><strong>Patching & Encryption</strong></summary>

- Patching
- Encryption

</details>

## Monitoring and Detection

Monitoring tools and techniques help detect and respond to threats in real time.

<details>
<summary><strong>Monitoring & Detection</strong></summary>

- Security Information and Event Management (SIEM): real time centralization of logs from servers and network devices
- Security Orchestration, Automation, and Response (SOAR): real time, uses AI and ML to decipher patterns, detect anomalies, and make data-driven decisions
- Endpoint Detection and Response (EDR) tools: used to react to infrastructure endpoints
  - Continuous monitoring
  - Behavioural analysis
  - Threat detection: Indicators of Compromise (IoCs)
  - Alert generation
  - Response and remediation
  - Forensic analysis
  - Real-time threat mitigation
  - Improved incident response
  - Endpoint visibility
- Host-Based Intrusion Prevention System (HIPS): protects individual computers
- Host-based firewall: firewalls that run on individual devices

</details>

## Principle of Least Privilege

Limiting user and system accounts to the minimum access permissions necessary for their function.

<details>
<summary><strong>Least Privilege</strong></summary>

- Least Privilege: limiting user and system accounts to the minimum access permissions necessary for their function

</details>

## Configuration Enforcement

Standardizing and automating configurations to reduce vulnerabilities and ensure compliance.

<details>
<summary><strong>Configuration Enforcement</strong></summary>

- Standardization: CIS benchmarks 
- Vulnerability mitigation
- Compliance adherence
- Automation

</details>

## Decommissioning and Data Sanitization

Properly retiring and sanitizing assets to prevent data leakage.

<details>
<summary><strong>Decommissioning & Data Sanitization</strong></summary>

- Decommissioning: retiring assets that are no longer needed
  - Documentation: hardware, software, other digital resources
  - Data sanitization: securely wiped or destroyed. Paper sanitization, Media sanitization.

</details>

## Hardening Techniques

Hardening involves securing systems by reducing their attack surface.

<details>
<summary><strong>Hardening Techniques</strong></summary>

- Disabling ports/protocols: See protocol and port table.

</details>
