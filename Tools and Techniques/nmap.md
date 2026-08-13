# Nmap

## Overview
- Nmap (Network Mapper) is a widely used tool for network discovery and security auditing.
- It identifies live hosts, open ports, running services, and system details.

## Key Concepts
- Open-source tool used for host discovery and port scanning.
- Targets can include IP addresses, domains, ranges, or subnets.
- Identifies live hosts using ARP, ICMP, and TCP/UDP scans.
- `-sT` – TCP connect scan (full handshake).
- `-sS` – SYN (stealth) scan (faster, less detectable).
- `-sU` – UDP scan (identifies UDP services).
- Ports are classified as **open**, **closed**, or **filtered**.
- `-O` – OS detection.
- `-sV` – Service and version detection.
- `-A` – Enables OS, version detection, and additional features.
- `-Pn` – Treat all hosts as online (skip host discovery).
- Faster scans are noisier and less accurate; slower scans are stealthier and more reliable.
- **Nmap Scripting Engine (NSE)** uses Lua scripts for automation and vulnerability detection.

## Relevance
- Used in reconnaissance to map network attack surfaces.
- Essential for penetration testing and security assessments.
- Widely used by ethical hackers, SOC analysts, and network engineers.
