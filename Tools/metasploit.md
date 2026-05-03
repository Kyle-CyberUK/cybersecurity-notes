# Metasploit

## Overview
- Metasploit is a widely used exploitation framework for penetration testing.
- It is used to identify, exploit, and interact with vulnerabilities.

## Key Concepts
- Supports vulnerability scanning, exploitation, and post-exploitation.
- Available as **Metasploit Framework** (open-source) and **Metasploit Pro** (commercial).
- `msfconsole` – Primary command-line interface.
- **Modules** – Pre-built code for exploits, payloads, and auxiliary functions.
- **Auxiliary modules** – Used for scanning and vulnerability detection.
- `msfvenom` – Tool for generating custom payloads.
- **Payloads** execute code on a target system after exploitation.
- **Single payloads** – Delivered in one piece.
- **Staged payloads** – Delivered in multiple parts.

## Exploitation Workflow
- Identify a vulnerable service.
- Perform scanning to discover open ports and services.
- Select a matching exploit module.
- Configure target and payload settings.
- Execute the exploit to gain access.
- Perform post-exploitation (privilege escalation, lateral movement).

## Relevance
- Demonstrates the full attack lifecycle: **Recon, Scan, Exploit, Post-exploit**.
- Widely used in penetration testing and red team operations.
- Essential for understanding real-world exploitation techniques.
