---
title: 🛡️ Fundamental Security Concepts
description: Core security concepts including CIA triad, AAA framework, non-repudiation, zero trust, and more for CompTIA Security+ exam objective 1.2
draft: false

tags:
  - CompTIA
  - Domain 1
  - Security Concepts
  - CIA Triad
---

> [!quote] Definition
> **Fundamental Security Concepts** are the core principles and frameworks that form the foundation of information security, including the CIA triad, AAA framework, non-repudiation, and modern approaches like zero trust.

## CIA Triad

The three fundamental principles of information security that every security program must address:

<details>
<summary><strong>Confidentiality</strong></summary>

*Ensuring that information is accessible only to those authorized to have access*

**Implementation Methods:**
- **Access Controls** - Authentication and authorization mechanisms
- **Data Encryption** - Protecting data at rest and in transit
- **Data Classification** - Categorizing data by sensitivity level
- **Privacy Controls** - Protecting personal and sensitive information

**Examples:**
- Encrypted file systems and databases
- User authentication and authorization
- Data masking and anonymization
- Secure communication channels

</details>

<details>
<summary><strong>Integrity</strong></summary>

*Maintaining and assuring the accuracy and completeness of data*

**Implementation Methods:**
- **Hashing Algorithms** - SHA1, MD5, SHA-256 for data integrity verification
- **Digital Signatures** - Cryptographic verification of data authenticity
- **Checksums** - Mathematical validation of data integrity
- **Audit Trails** - Logging and monitoring data changes

**Examples:**
- File integrity monitoring (FIM)
- Database integrity constraints
- Version control systems
- Blockchain technology

</details>

<details>
<summary><strong>Availability</strong></summary>

*Ensuring that authorized users have access to information when needed*

**Implementation Methods:**
- **Redundancy** - Backup systems and failover mechanisms
- **Disaster Recovery** - Business continuity planning
- **Load Balancing** - Distributing workload across multiple systems
- **High Availability** - Minimizing downtime through clustering

**Examples:**
- RAID storage systems
- Backup power supplies (UPS)
- Cloud-based redundancy
- Service level agreements (SLAs)

</details>

## Non-Repudiation

**Ensuring that parties cannot deny their involvement in actions or transactions**

<details>
<summary><strong>Digital Signatures</strong></summary>

- **Cryptographic Identifiers** - Unique digital signatures for documents and transactions
- **Certificate-Based Signatures** - PKI-based digital signatures
- **Timestamp Services** - Verifying when signatures were created
- **Signature Verification** - Validating signature authenticity

</details>

<details>
<summary><strong>Audit Trails</strong></summary>

- **Comprehensive Logging** - Log all actions with timestamps and user identification
- **Immutable Logs** - Ensure logs cannot be modified or deleted
- **Chain of Custody** - Track the complete lifecycle of actions
- **Digital Evidence** - Preserve evidence for legal proceedings

</details>

<details>
<summary><strong>Access controls</strong></summary>

- **Screenshots and Recordings** - Visual evidence of activities
- **System Logs** - Technical logs from all affected systems

</details>

## Authentication, Authorization, and Accounting (AAA)

The AAA framework provides comprehensive access control and accountability:

<details>
<summary><strong>Authentication</strong></summary>

**Verifying the identity of users and systems**

**Methods:**
- **Multi-Factor Authentication (MFA)** - Multiple forms of verification
- **Digital Certificates** - PKI-based authentication
- **Biometric Authentication** - Fingerprint, retinal, facial recognition
- **Token-Based Authentication** - Temporary access tokens

**AAA Protocols:**
- **RADIUS** - Remote Authentication Dial-In User Service
  - Used by Wireless Access Points, Routers, Switches
  - Client/server architecture
- **Diameter** - Successor to RADIUS
  - Used by LTE and WiMAX Access Points, 4G and 5G networks
- **TACACS+** - Terminal Access Controller Access Control System Plus (Cisco)
  - Used by routers, switches, and firewalls

</details>

<details>
<summary><strong>Authorization</strong></summary>

**Determining what resources users can access**

**Authorization Models:**
- **Role-Based Access Control (RBAC)** - Access based on job roles
- **Attribute-Based Access Control (ABAC)** - Access based on attributes
- **Discretionary Access Control (DAC)** - Owner-controlled access
- **Mandatory Access Control (MAC)** - System-enforced access

**Implementation:**
- **Security Identifiers (SID)** - Unique identifiers for users and groups
- **Access Control Lists (ACLs)** - Permissions for resources
- **Policy Enforcement** - Automated access control decisions

</details>

<details>
<summary><strong>Accounting</strong></summary>

**Tracking and logging all activities for audit and compliance**

**Components:**
- **Audit Logs** - Comprehensive logging of all activities
- **Session Recording** - Recording user sessions
- **Change History** - Tracking all system changes
- **Compliance Reporting** - Generating reports for regulations

**Applications:**
- **Security Monitoring** - Detecting suspicious activities
- **Compliance Audits** - Meeting regulatory requirements
- **Incident Investigation** - Analyzing security incidents
- **Performance Analysis** - Understanding system usage patterns

</details>

## Gap Analysis

**Identifying the difference between current and desired security posture**

<details>
<summary><strong>Gap Analysis Process</strong></summary>

**Iterative Process:**
1. **Assessment** - Evaluate current security controls and processes
2. **Benchmarking** - Compare against industry standards and best practices
3. **Identification** - Identify specific gaps and vulnerabilities
4. **Prioritization** - Rank gaps by risk and business impact
5. **Remediation Strategy** - Develop plans to address identified gaps

</details>

<details>
<summary><strong>Gap Analysis Components</strong></summary>

- **Security Control Gaps** - Missing or inadequate security controls
- **Process Gaps** - Incomplete or ineffective processes
- **Technology Gaps** - Missing or outdated technology
- **Compliance Gaps** - Non-compliance with regulatory requirements

</details>

## Zero Trust

**"Never trust, always verify" approach to security**

<details>
<summary><strong>Zero Trust Principles</strong></summary>

- **Verify Every Access** - No access is trusted by default
- **Least Privilege Access** - Grant minimal necessary access

</details>

<details>
<summary><strong>Zero Trust Implementation</strong></summary>

- **Identity Verification** - Verify identity before any access
- **Device Trust** - Ensure devices are trusted and secure
- **Network Segmentation** - Isolate networks and systems
- **Continuous Validation** - Continuously validate trust throughout sessions

</details>

## Control Plane vs Data Plane

<details>
<summary><strong>Control Plane</strong></summary>

**Where security decisions and policies are managed**

**Components:**
- **Adaptive Identity** - Flexible approach to identity management based on context and behavior
- **Threat Scope Reduction** - Reducing the attack surface through strategic controls
- **Policy Engine** - Makes access decisions based on policies and context
- **Policy Administrator** - Manages and configures policy rules and settings
- **Policy-Driven Access Control** - Automated access control based on defined policies

**Functions:**
- **Identity Management** - Adaptive identity systems that adjust permissions based on context
- **Attack Surface Management** - Continuously reduce threat scope through policy enforcement
- **Policy Decision Making** - Policy engine evaluates requests and makes access decisions
- **Policy Administration** - Policy administrator configures and maintains access policies

</details>

<details>
<summary><strong>Data Plane</strong></summary>

**Where actual data movement and processing occurs**

**Components:**
- **Implicit Trust Zones** - Trusted areas holding resources that are considered secure
- **Subjects/Systems** - People and devices that are identified and authenticated
- **Policy Enforcement Points** - Monitors and enforces policies within the data plane

**Network Zones:**
- **Internal Network Zone (LAN)** - Trusted systems behind firewall (Domain Controllers, Database Servers)
- **Demilitarized Zone (DMZ)** - Semi-trusted area for public-facing services
- **External Network Zone (WAN)** - Untrusted external networks (Internet)

**Functions:**
- **Resource Access** - Subjects access resources within implicit trust zones
- **Policy Enforcement** - Policy enforcement points monitor and control access
- **Data Movement** - Packets move through routers, switches, firewalls, load balancers

</details>

## Physical Security

**Physical security measures that protect assets**

<details>
<summary><strong>Physical Security Components</strong></summary>

**Access Control:**
- **Bollards** - Physical barriers to prevent vehicle-based attacks
- **Access Control Vestibules** - Controlled entry points with dual-door systems
- **Fencing** - Perimeter protection around critical facilities
- **Security Guards** - Human monitoring and response
- **Biometric Locks** - Advanced authentication for high-security areas

**Environmental Controls:**
- **HVAC Systems** - Climate control for sensitive equipment
- **Fire Suppression** - Automatic fire detection and suppression systems
- **Power Backup** - Uninterruptible power supplies (UPS) and generators
- **Environmental Monitoring** - Sensors for temperature, humidity, and other conditions

</details>

## Deception and Disruption Technology

**Honeypot technologies used to detect and analyze threats**

<details>
<summary><strong>Honeypot Technologies</strong></summary>

**Honeypot** - Decoy systems designed to attract and monitor attackers
- Production, Research, and Low-Interaction types
- Used for threat detection and attack analysis

**Honeynet** - Network of honeypots that simulate entire network environments
- Multiple decoy systems with centralized monitoring
- Used for attack pattern analysis and security research

**Honeyfile** - Decoy files designed to detect unauthorized access
- Realistic files that trigger alerts when accessed
- Used for data access monitoring and insider threat detection

**Honeytoken** - Dummy data or credentials used to detect unauthorized access
- Fake database records, API keys, credentials, and email addresses
- Used for credential monitoring and data breach detection

**DNS Sinkhole** - Redirects DNS queries to prevent access to malicious domains
- Blocks access to known malicious websites
- Prevents malware communication with command and control servers

</details>

> [!note] Vocab Bank
> - **Security Identifier (SID)** - Unique identifier for users, groups, and computers in Windows systems
> - **MITRE ATT&CK** - Knowledge base of adversary tactics, techniques, and procedures used for threat modeling
> - **CVE list** - Common Vulnerabilities and Exposures database of publicly known security vulnerabilities
> - **OAuth** - Open standard authorization protocol for secure third-party access to resources
> - **SAML token** - Security Assertion Markup Language token for single sign-on authentication
> - **SWOT analysis** - Strategic planning tool analyzing Strengths, Weaknesses, Opportunities, and Threats
> - **IDS log** - Intrusion Detection System log containing security event records and alerts

---

*Last updated: July 20, 2025*