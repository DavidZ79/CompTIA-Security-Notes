---
title: Types of Vulnerabilities
description: 
draft: false
tags:
  - CompTIA
---

Application Vulnerabilities

Time-of-check, time-of-use (TOCTOU)
- Memory injection
- Buffer overflow
- Race conditions
- Malicious update

Operating System Based Vulnerabilities

Web-Based Vulnerabilities
- Structured Query Language Injection (SQLI): use stored procedures or input validation
- Cross-Site Scripting (XSS): HTML script injection

Hardware Vulnerabilities
- Vulnerabilities in firmware:
- End-of-life systems (EOL): product is no longer updated/supported
- Legacy system vulnerabilities

Virtualization Vulnerabilities
- VM escape: unauthorized access to another VM (lateral movement / east to west)
- Resource reuse: misallocated / exhausted resources
- VM sprawl: uncontrolled VM use

Cloud-Specific Vulnerabiltiies
- Risk of shared tenancy: multiple customers sharing the same physical infrastructure
- Inadequate configuration management: mishandling configurations
- Identity and access management flaws: weak user permissions / credentials
- Cloud Access Security Broker (CASB): enforcers of a cloud company's security policies

Supply Chain Vulnerabilities
- Service provider vulnerabilities: gaps in third-party relationships
- Hardware provider vulnerabilities: counterfeit / compromised hardware
- Software provider vulnerabilities: insecure coding practices / third-party libraries

Cryptographic Vulnerabilities
- Certificate authority (CA) compromise: attackers can generate fraudulent certificates
- Key compromise
- Flawed implementation: poorly coded encryption routines / weak key management
- Outdated algorithms: new techniques / more computational power
- Side-channel attacks: power consumption, timing, EM radiation
- Backdoor exploitation
- RNG: dangerous when predicatable
- Certificate revocation lists (CRL) and the Online Certificate Status Protocol (OCSP)
- Secure key management: HSM / key escrow
- SSL stripping: bypass certificate-based protection, turn session into HTTP attack (HTTPS downgrade attack)
- SSL/TLS downgrade: SSL traffic intercepted by server with less secure browser, SSL switches to weaker encryption method. Padding Orable On Downgraded Legacy Encryption (POODLE) attack / man-in-the-middle attack.

Misconfiguration Vulnerabilities
- Network devices: change default configurations, change access control lists (ACL)
- Firewalls: misconfigured firewalls can yield unauthorized access, malware and attacks, and regulatory compliance challenges
- Default credentials/configurations: add multifactor authentication
- Unpatched software
- Excessive privileges
- Data Loss Prevention: Prevents Personal Identifying Information (PII) or sensitive data leaving the company based on pattern matching

Mobile Device Vulnerabilities
- Jailbreaking (Apple): bypass manufacturer or OS restrictions
- Rooting / Unlocking (Android)
- Sideloading: use of Android Application Package (APK files)

Above subject to
- Counterfeit apps
- Software instability
- Security compromises
- Stolen data

Mobile device management (MDM) solutions: policies for installation and protection of mobile devices. (Cloud version is CASB.)

Zero-Day Vulnerabilities: no known patches / security tools

