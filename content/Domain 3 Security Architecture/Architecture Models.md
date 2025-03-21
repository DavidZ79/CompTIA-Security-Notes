---
title: Architecture Models
description: 
draft: false
tags:
  - CompTIA
---

Securing the Network: Use of firewalls, Access Control Lists (ACLs), Intrusion Detection Systems (IDSs), Intrusion Prevention Systems (IPSs), and Security Information and Event Management (SIEM).

Securing the Servers
- Domain controllers: authenticate users
- SQL servers: store sensitive data

Many organizations use cloud storage: Amazon S3, Microsoft Azure Blob Storage, Google Cloud

Securing the Hosts: user devices and endpoints. Can use antivirus software, Endpoint Detection and Response (EDR) tools, and Mobile Device Management (MDM) systems. 

Architecture and Infrastructure Concepts

Cloud Computing: Use a Cloud Service Provider (CSP). Microsoft or Amazon Web Services (AWS)
- Public Cloud (multi-tenant)
- Private Cloud: separate servers
- Community Cloud: companies from the same industry all pay for an application to be written and hosted on the cloud
- Hybrid Cloud: mix of on-premise and cloud infrastructures

Cloud Services:
- Infrastructure as a Service (IaaS): CSP will only provide physical hardware for network infrastructure
- Software as a Service (SaaS): software application accessed through a webserver. Office365
- Platform as a Service (PaaS): environment to build applications. Microsoft Azure, MySQL
- Security as a Service (SECaaS): CSP provides Identity and Access Management (IAM) for secure access to applications from anywhere at any time. 
- Anything as a Service (XaaS): others, such as Network as a Service (NaaS), Desktop as a Service (DaaS), Backup as a Service (BaaS), ...

Responsibility Matrix: Domains between customer and CSP
- Physical Security
- Identification and Access Management
- Security Monitoring
- Application Security
- Configuration Management
- Incident Response
- Awareness Training
- Maintenance

Hybrid Considerations: Data management: consider latency, synchronization, and maintenance overhead. 

Third-party vendors: consider data breaches, security vulnerabilities, compliance challenges, and operational disruption. May be vulnerable to supply chain attacks

Infrastructure as Code (IaC): YAML, JSON
- Efficiency Redefined
- Consistency and Reproducibility
- Version Control and Collaboration
- Providers and Tools (Terraform, Ansible, Puppet, Chef)

Serverless: environment for developers to deploy code. Backend as a Service (BaaS)

Microservices: breakdown application into smaller self-contained services that communicate via API
- Agility: respond to changing business needs
- Scalability
- Faster Development
- Easy Maintenance
- Improved Fault Tolerance
- Decomposition: logical separation into smaller more manageable components
- Independence

Network Infrastructure
See OSI table

- Wireless Access Point (WAP): connects wireless devices to connect to a wired network
- Router: Connects 2 different networks when setting up a host machine (default gateway). Uses routing table, or 0.0.0.0 for unknown, which is usually sent to ISP
- Switch: links devices in LAN, maintains table known as Content Addressable Memory (CAM)
- Address Resolution Protocol (ARP): map IP address to MAC address (1 MAC address per port)
- Layer 3 switch (multilayer switch): operates in layers 2 and 3 of Open Systems Interconnection (OSI) model.
- Load Balancer: distributes incoming traffic evenly onto multiple servers
- Web Application Firewall (WAF): protects web server
- Network Intrusion Prevention System (NIPS): monitors network traffic in real time. Uses signature-based detection, anomaly detection, and behavioral analysis

Physical Isolation: air-gapped network means no wired or wireless connections to devices

Logical Segmentation
- Subnetting: reduce broadcast domain
- VLAN: groups multiple network ports together. Each VLAN has an id tag which is readable by switches. Tags packets with the id tag.

Software-Defined Networking (SDN)
- Management Plane: monitors network traffic
- Control Plane: network's "brain". High-level decisions about traffic routing, policies, and resource allocators
- Data Plane: includes network hardware. Responsible for forwarding packets from the control plane.

On-Premises: organization's presence in a physical building with staff.

Centralized vs Decentralized
- Centralized: decision-making from the top
- Decentralized: distributes decision-making across all levels of the organization

Containerization: all containers sit on docker layer above OS

Virtualization: Virtual Desktop Infrastructure (VDI): CSP has control over desktop image and applications. Ex. Citrix, Microsoft's App-V

Internet of Things (IoT): network of physical objects
- Lack of Standardization
- Data Privacy Concerns
- Insecure Communication
- Lifecycle Management
- Physical Attacks
- Supply Chain Risks
- User Awareness

Industrial Control Systems (ICS) / Supercisory Control and Data Acquisition (SCADA): SCADA are automated ICS
- Plant Level (0): physical equipment. Sensors, Actuators, motors, ...
- Controller Level (1): real-time control of physical devices. Ex Programmable Logic Controllers (PLC)
- Coordinating Computer Level (2): Human-Machine Interface (HMI) systems give centralized view of plant's operations
- Program Logic Controller Level (3): Manages overall production process. Ex. recipe management, scheduling, data logging, ...

SCADA systems deal with services such as
- Energy: electricity from oil and gas
- Facilities
- Manufacturing
- Logistics
- Industrial

Real-Time Operating System (RTOS): Used when timing is most important. Ex. navigation, flight control system

Embedded Systems: computer systems for specific tasks. Ex. Engine Control Units (ECUs), Anti-lock Braking Systems (ABS)

High Availability (HA): System's ability to remain operational despite issues. CSP breaks world down into different regions: Geo-Zone Redundant Storage (GZRS)

Considerations for your Infrastructure
- Availability
- Resilience
- Cost: consider Service-Level Agreement (SLA)
- Responsiveness
- Scalability
- Ease of deployment
- Risk transference
- Easy of recovery
- Patch availability
- Inability to patch
- Power
- Compute