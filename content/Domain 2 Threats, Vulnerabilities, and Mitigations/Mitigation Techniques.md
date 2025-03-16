---
title: Mitigation Techniques
description: 
draft: false
tags:
  - CompTIA
---

Segmentation: compartmentalize network, limiting lateral movement
- Physical segmentation: uses routers, switches, and firewalls
- Virtual Local Area Networks (VLANs): logical network segments within a single switch. Groups devices by department or function, reduces network traffic
- Subnetting: divides an IP network into smaller subnets, each with a subnet mask. Groups devices, efficient use of IP addresses
- Micro-segmentation: security policies for individual workloads or devices. Important in cloud environments and data centers

Reasons for segmentation:
- Enhanced security
- Access control
- Compliance requirements: Payment Card Industry Data Security Standard (PCI DSS) card payments in secure environment, among others
- Performance optimization: reduces broadcast domains
- Isolation of critical systems
- Scalability and agility

Access Control
- Access Control Lists (ACLs) used by routers and firewalls. For files and folders, and for network traffic

Application Allow List: whitelist

Application Block List: prevents specific applications from running.

Isolation: self-contained environments within a network for critical systems and data

Patching

Encryption

Monitoring
- Security Information and Event Management (SIEM): real time centralization of logs from servers and network devices
- Security Orchestration, Automation, and Response (SOAR): real time, uses AI and ML to decipher patterns, detect anomalies, and make data-driven decisions

Least Privilege: limiting user and system accounts to the minimum access permissions necessary for their function

Configuration Enforcement
- Standardization: CIS benchmarks 
- Vulnerability mitigation
- Compliance adherence
- Automation

Decommissioning: retiring assets that are no longer needed
- Documentation: hardware, software, other digital resources
- Data sanitization: securely wiped or destroyed. Paper sanitization, Media sanitization.

Hardening Techniques

Endpoint Detection and Response (EDR) tools: used to react to infrastructure endpoints
- Continuous monitoring
- Behavioural analysis
- Threat detection: Indicators of Compromise (IoCs)
- Alert generation
- Response and remediation
- Forensic analysis
- Real-time threat mitigation
- Improved incident response
- Endpoint visibility

Host-Based Intrusion Prevension System (HIPS): protects individual computers

Host-based firewall: firewalls that run on individual devices

Disabling ports/protocols: See protocol and port table.
