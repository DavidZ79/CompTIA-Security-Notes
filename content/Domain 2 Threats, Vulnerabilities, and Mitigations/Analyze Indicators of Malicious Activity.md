---
title: Analyze Indicators of Malicious Activity
description: 
draft: false
tags:
  - CompTIA
---

Malware Attacks

Potentially Unwanted Programs (PUPs): programs downloaded inside other programs. Grayware that takes computer resources, neither malicious nor legitimate.

Ransomware: encrypts files and demands payment in cryptocurrency or prepaid cards.

Trojans: Appears as legitimate software or files, executes malicious programs, can be embedded in a web page through code injection. Can use Portable Executable (PE) files, which is a common file format for executable binary files in Windows.

Remote Access Trojans (RATs): trojans that allow remote access

Worms: malware that self-propogates and resides in computer memory.

Spyware: Uses computer resources to send information to a third party.

Bloatware: Unwanted programs that disguises itself as helpful.

Viruses

Polymorphic Viruses: modifies its own code to appear unique

Keyloggers: unknowningly records keystrokes

Logic Bombs: malware that triggers given a certain condition

Rootkits: embeds itself in the operating system to possess system-level access

Malware Inspection uses sandboxes such as Cuckoo for inspection, patching, and testing

Physical Attacks
- Physical Brute Force: Breaks into building to steal
- Radio Frequency Identification (RFID) cloning / skimming
- Environmental: power outages, floods, fires, earthquakes

Network Attacks
- Pivoting: access a network via vulnerable host. On a virtual network, it's called VM escape. Attackers use Network Mapper (nmap) tool to map out the whole network
- Distributed Denial-of-Service (DDoS): group of computers (botnet) attack victim to take its services down. Overwhelm victim with SYN flood attack. Target expects ACK packet (third part of TCP handshake), but never receives it, using up resources.
- 3 types of DDoS attacks: 
- Amplified: small request triggers large response. Internet Control Message Protocol (ICMP), smurf attack
- Reflected: attacker obtains victim's IP address to craft packet from the victim, then sent to server which resends to victim.

ARP Poisoning (Address Resolution Protocol, Layer 2): Maps IP address to MAC (Media Access Control) addresses. Can only happen on LAN. Victim's LAN is flooded with fake ARP message with victim's IP address matching attacker's MAC address. Then, traffic meant for victim is sent to attacker.

DNS attacks: DNS server uses DNS resolution to convert URL to IP address

1. DNS cache: on local machine

2. HOSTS file

3. Root hints: forwards resolution to other DNS servers on the internet

4. DNS sinkhole: identifies known malicious domains and sends back false information to potential attackers

5. DNS cache poisoning / spoofing: poisoning DNS cache / HOSTS file

DNS Commands:
- ipconfig / displaydns: To view the DNS cache
- ipconfig / flushdns: To clear the DNS cache
- dnslookup/: To check the DNS record in the DNS server, appending the command with the name of the computer you want to check, e.g. dnslookup computer 1

DNS Tools: DNSenum collects DNS information. DNSSEC uses digital signatures to counter DNS cache poisoning attacks.

Wireless Attacks:
- Rogue access points: pretends to be legitimate Wireless Access Point (WAP), tricks users to connect to them
- Evil twin: Rogue access point, but intercepts communications. Duplicate network with same name (SSID). Telltale: can't access company data, because you are on another network
- Deauthentication (disassociation) and jamming attacks: disconnect target computer from network
- MAC spoofing and device impersonation: impersonate authorized devices on the network
- Wi-Fi analyzer: listens to network signals

On-path (man-in-the-middle) attacks: Rogue access points, evil twins, DNS and ARP poisoning attacks are examples.

Session Replay: When user connects to web server, session token is created (may be saved as a cookie). May intercept token with Cross-Site Scripting (XSS).

Replay Attack: on-path attack that intercepts data but resends (replays) data later. Windows network with Kerberos authentication yields different USN numbers, and will be rejected out of sequence.

Credential Replay: malicious code, keyloggers, packet sniffers (Wireshark or tcpdump)
- Credential replay attacks: Replace telnet with Secure Shell (SSH). Don't use Windows' legacy NT LAN Manager (NTLM)
- Credential stuffing: attackers try the same credentials for other accounts with other services

Malicious code
- Bash shell attacks: Bash scripts can execute unauthorized commands. Privilege escalation, file manipulation, system reconnaissance. 

See bash script example.

- Python: see keylogger script example.
- JavaScript: used for client-side attacks.

Application Attacks: exploit vulnerabilities in software
- Injection Attack: SQL and XSS injection
- Buffer Overflow: Windows OS uses Data Execution Prevention (DEP)
- Privilege Escalation: exploit vulnerabilities to gain elevated privileges
- Forgery Attacks: impersonates users or applications. Cross-Site Request Forgery (CSRF), Server-Side Request Forgery (SSRF)

Directory Traversal
- Input validation
- Stored procedures: predefined SQL scripts that prevent manipulation 

Cryptographic Attacks
- Downgrade Attacks: intercepts communication and downgrades encryption. SSL/TLS downgrade, SSL stripping
- Collision: malicious and benign document with the same hash. Benign signed, then swaps to malicious one
- Birthday: probability phenomenon: in a group of 23 people, there's a 50% chance that two individuals share the same birthday (excluding year). Likelihood of two distinct inputs sharing the same hash value. More bits the better.
- Pass-the-Hash Attack: Older OS victim to rainbow tables and hashcat. NTLM user passwords were stored in Local Security Authority Subsystem Service (LSASS). NTLM later replaced with Active Directory (Kerberos authentication)

Password Attacks
- Dictionary attack: cracking passwords with words from dictionary
- Password spraying: sprayers focus on guessing a few common usernames
- Brute force: rainbow tables
- Hybrid attack: mix of dictionary and brute-force

Online password attack: guesses made live on login interface

Offline password attack: take password storage and crack them offline

Indicators of Attack (IoAs)
- Account lockout
- Concurrent session usage
- Blocked content: log access-denied message
- Impossible travel: 2 logins from across the world
- Resource consumption
- Out-of-cycle logging: attackers may manipulate logs
- Published/documented: malicious actors are attracted to published vulnerabilities
- Missing logs
