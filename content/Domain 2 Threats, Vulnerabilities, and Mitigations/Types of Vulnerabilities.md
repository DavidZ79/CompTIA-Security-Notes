---
title: 🐞 Types of Vulnerabilities
description: 
draft: false
tags:
  - CompTIA
---

> [!quote] Definition
> **Vulnerabilities** are weaknesses in systems, applications, hardware, or processes that can be exploited by threat actors to compromise confidentiality, integrity, or availability. Understanding different types of vulnerabilities is essential for effective risk management and mitigation.

## Application Vulnerabilities

Application vulnerabilities arise from flaws in software code or logic, making applications susceptible to exploitation.

<details>
<summary><strong>Application Vulnerabilities</strong></summary>

- Time-of-check, time-of-use (TOCTOU)
- Memory injection
- Buffer overflow
- Race conditions
- Malicious update

</details>

## Operating System Vulnerabilities

Operating system vulnerabilities are weaknesses in the OS that can be exploited to gain unauthorized access or control.

<details>
<summary><strong>Operating System Based Vulnerabilities</strong></summary>

<!-- Add specific OS vulnerabilities here if needed -->

</details>

## Web-Based Vulnerabilities

Web-based vulnerabilities target web applications and services, often through user input or insecure configurations.

<details>
<summary><strong>Web-Based Vulnerabilities</strong></summary>

- Structured Query Language Injection (SQLI): use stored procedures or input validation
- Cross-Site Scripting (XSS): HTML script injection

</details>

## Hardware Vulnerabilities

Hardware vulnerabilities stem from flaws in physical devices or their firmware.

<details>
<summary><strong>Hardware Vulnerabilities</strong></summary>

- Vulnerabilities in firmware
- End-of-life systems (EOL): product is no longer updated/supported
- Legacy system vulnerabilities

</details>

## Virtualization Vulnerabilities

Virtualization introduces unique risks related to the management and isolation of virtual machines.

<details>
<summary><strong>Virtualization Vulnerabilities</strong></summary>

- VM escape: unauthorized access to another VM (lateral movement / east to west)
- Resource reuse: misallocated / exhausted resources
- VM sprawl: uncontrolled VM use

</details>

## Cloud-Specific Vulnerabilities

Cloud environments have vulnerabilities related to shared resources, configuration, and access management.

<details>
<summary><strong>Cloud-Specific Vulnerabilities</strong></summary>

- Risk of shared tenancy: multiple customers sharing the same physical infrastructure
- Inadequate configuration management: mishandling configurations
- Identity and access management flaws: weak user permissions / credentials
- Cloud Access Security Broker (CASB): enforcers of a cloud company's security policies

</details>

## Supply Chain Vulnerabilities

Supply chain vulnerabilities arise from third-party providers, hardware, or software dependencies.

<details>
<summary><strong>Supply Chain Vulnerabilities</strong></summary>

- Service provider vulnerabilities: gaps in third-party relationships
- Hardware provider vulnerabilities: counterfeit / compromised hardware
- Software provider vulnerabilities: insecure coding practices / third-party libraries

</details>

## Cryptographic Vulnerabilities

Cryptographic vulnerabilities involve weaknesses in encryption, key management, or cryptographic protocols.

<details>
<summary><strong>Cryptographic Vulnerabilities</strong></summary>

- Certificate authority (CA) compromise: attackers can generate fraudulent certificates
- Key compromise
- Flawed implementation: poorly coded encryption routines / weak key management
- Outdated algorithms: new techniques / more computational power
- Side-channel attacks: power consumption, timing, EM radiation
- Backdoor exploitation
- RNG: dangerous when predictable
- Certificate revocation lists (CRL) and the Online Certificate Status Protocol (OCSP)
- Secure key management: HSM / key escrow
- SSL stripping: bypass certificate-based protection, turn session into HTTP attack (HTTPS downgrade attack)
- SSL/TLS downgrade: SSL traffic intercepted by server with less secure browser, SSL switches to weaker encryption method. Padding Oracle On Downgraded Legacy Encryption (POODLE) attack / man-in-the-middle attack.

</details>

## Misconfiguration Vulnerabilities

Misconfiguration vulnerabilities result from improper setup of devices, software, or security controls.

<details>
<summary><strong>Misconfiguration Vulnerabilities</strong></summary>

- Network devices: change default configurations, change access control lists (ACL)
- Firewalls: misconfigured firewalls can yield unauthorized access, malware and attacks, and regulatory compliance challenges
- Default credentials/configurations: add multifactor authentication
- Unpatched software
- Excessive privileges
- Data Loss Prevention: Prevents Personal Identifying Information (PII) or sensitive data leaving the company based on pattern matching

</details>

## Mobile Device Vulnerabilities

Mobile devices are susceptible to unique vulnerabilities due to their portability and software ecosystem.

<details>
<summary><strong>Mobile Device Vulnerabilities</strong></summary>

- Jailbreaking (Apple): bypass manufacturer or OS restrictions
- Rooting / Unlocking (Android)
- Sideloading: use of Android Application Package (APK files)
- Counterfeit apps
- Software instability
- Security compromises
- Stolen data
- Mobile device management (MDM) solutions: policies for installation and protection of mobile devices. (Cloud version is CASB.)

</details>

## Zero-Day Vulnerabilities

Zero-day vulnerabilities are unknown to the vendor and have no available patches or security tools.

<details>
<summary><strong>Zero-Day Vulnerabilities</strong></summary>

- No known patches / security tools

</details>

