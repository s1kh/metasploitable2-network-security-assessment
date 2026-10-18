# Metasploitable 2 Network Security Assessment

## Overview
A network security assessment of an intentionally vulnerable target (Metasploitable 2)
in an isolated lab network, covering host discovery, port/service enumeration, traffic
analysis, and defensive network design.

## My Contribution
Individual university networking assignment. I performed all scanning, analysis, and
defensive design work.

## Objectives
- Practice host discovery and service enumeration methodology
- Analyze live network traffic and protocol behavior
- Identify high-risk exposed services and propose a defensible network architecture

## Environment
| Component | Details |
|---|---|
| Attacker | Kali Linux |
| Target | Metasploitable 2 |
| Network Mode | VirtualBox Host-Only (isolated) |

## Work Performed
- Verified connectivity and confirmed an isolated Layer 2 network segment
  (ping, ARP table analysis)
- Performed subnet/host discovery and OS fingerprinting with Nmap
- Ran full TCP/UDP port scans and service version detection
- Captured and analyzed traffic with Wireshark (ICMP, TCP 3-way handshake,
  protocol hierarchy)
- Documented high-risk exposed services (FTP, Telnet, HTTP, SMB) and their
  specific risks
- Implemented and verified `iptables` DROP rules for insecure protocols
- Designed a defense-in-depth secure network architecture (DMZ placement,
  firewall/IPS positioning, blocked lateral movement)

## Results
- Identified and documented the target's full exposed attack surface
- Demonstrated working firewall rules that successfully blocked insecure protocols
- Produced a secure network redesign addressing the identified risks

## Documentation
See [`docs/security_assessment.pdf`](./docs/security_assessment.pdf) for the full written report and supporting screenshots.

## Disclaimer
Conducted entirely within an isolated, offline lab network for educational purposes.
