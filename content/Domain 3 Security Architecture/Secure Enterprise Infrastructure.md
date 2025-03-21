---
title: Secure Enterprise Infrastructure
description: 
draft: false
tags:
  - CompTIA
---

Infrastructure considerations

Device Placement: See table

Security Zones
- Segmentation
- Data protection
- Access control
- Monitoring and logging: SIEM, SOAR
- Isolation
- Compliance
- Incident containment
- Operational efficiency
- Defense in depth

Attack Surface
- Endpoints
- Network services
- Ports and protocols
- User accounts and credentials
- Third-party integrations
- Cloud services
- Human factor

To minimize attack surface:
- Vulnerability assessment
- Access control
- Network segmentation
- Single point of failure
- Security point of failure
- Security updates
- Strong authentication
- Regular auditing
- Security awareness

Connectivity
- Scalability
- Security
- Redundancy
- Complexity
- Remote work

Failure Modes: Device behaviour when failure occurs. Fail-closed, fail-open

Device Attribute: monitors network flow
- Active devices (firewalls and IPSs)
- Passive devices (IDSs)
- Inline: directly in the path of network traffic (load balancer)
- Tap/monitor: monitor traffic (packet sniffer)

Network Appliances
- Jump server
- Proxy server: client to external server. URL filtering, Content filtering, Web page caching
- Reverse proxy server: in DMZ to secure session and filter incoming traffic
- IPS and IDS
- Load balancer: least utilized host, affinity, DNS round robin