---
title: Fundamental Security Concepts
description: 
draft: false
tags:
  - CompTIA
---

CIA Triad:
- Confidentiality
- Integrity: Includes Hashing Algorithms such as SHA1 and MD5
- Availability

Non-Repudiation: Prevents denial of actions
- Digital signatures: cryptographic identifiers
- Audit trails
- Acces controls: Identify (SID, Security ID), Authenticate, Authorize

AAA Servers / Framework
- Authenticating people
- Authenticating systems: 802.1X protocol. Each device must have a valid certificate on its endpoint.
- Authorization models: Defines scope of permissible activities
- Accounting
- AAA protocols: 

Remote Authentication Dial-In User Service (RADIUS) 
Wireless Access Points, Routers, Switches. Radius Clients / Server

Diameter: Successor of RADIUS
LTE and WiMAX Access Points, 4G and 5G

Terminal Access Controller Access Control System Plus (TACACS+) (Cisco)
Clients include routers, switches, and firewalls

Gap Analysis: Difference between current and desired security posture. Iterative process.
Assessment, Benchmarking, Identification, Prioritization, Remediation Strategy

Zero Trust: "Never trust, always verify"
See Control Plane diagram

Control Plane: Where user/device authorization managed by Policy Engine and administered by Policy Administrator. Which users/devices can access the network.
Adaptive Identity: User privileges based on context, behaviour, location, device characteristics, instead of static roles/permissions.
Policy Engine: Who gaines access to network based on policies. Per-user basis.
Policy Administrator: Executes decisions made by Policy Engine. Issues Access Tokens.
Policy Enforcement Point: Final check to data plane.

Policy-driven access control: automating responses to specific scenarios

Data Plane: movement of packets within a network.
Subjects initiate data communication, Systems process and forward packets (e.g. routers, switches, firewalls, load balancers, ...)
Implicit Trust Zone: Segment of network considered secure, no need for continuous verification.
Internal Network Zone (LAN): Trusted stuff behind firewall. Includes Domain Controller and Database Servers.
Demilitarized Zone (DMZ, screened subnet): Trusted AND Untrusted devices here. 
External Network Zone (WAN): Internet, Untrusted.

Physical Security: Bollards, Access control vestibule, Fencing, ...

Deception and Desruption Technology
- Honeypot: Decoy web server
- Honeynet: network of honeypots
- Honeyfile
- Honeytoken: dummy data
- Fake Information: DNS sinkhole. DNS queries are redirected to a different IP address.