# Nikto

## Overview
- Nikto is an open-source web server vulnerability scanner written in Perl.
- It automatically tests web servers for dangerous files, outdated software, and common misconfigurations.

## Key Concepts
- Identifies installed software using headers, favicons, and file analysis.
- Nikto is not stealthy; it generates a high volume of requests that will be logged and detected by IDS/WAF.

## Core Flags
- `-h <target>`         - Specify target host or IP
- `-p <port>`           - Specify port (default: 80)
- `-ssl`                - Force SSL/HTTPS scan
- `-o <file>`           - Save output to a file
- `-Format <type>`      - Output format: html, xml, csv, txt
- `-evasion <id>`       - Apply IDS evasion techniques
- `-Tuning <id>`        - Tune scan to specific vulnerability types

## Example Commands
```
nikto -h http://target.com                                  # Basic scan
nikto -h http://target.com -p 8080                          # Scan on a specific port
nikto -h http://target.com -ssl                             # HTTPS scan
nikto -h http://target.com -o results.html -Format html     # Save report
```
## What Nikto Can Detect
- Outdated and unpatched server software.
- Dangerous or exposed files and directories.
- Default credentials and configuration files.
- HTTP methods that should be disabled (e.g. TRACE, PUT).
- Cookie and security header misconfigurations.
- Common vulnerabilities including XSS and SQLi indicators.

## Relevance
- Nikto is a quick and effective reconnaissance tool used early in a pentest to get a broad picture of a web server's attack surface.
- It fits into the scanning phase alongside Nmap - Nmap finds open ports, Nikto investigates what's running on them.
- Output can also be fed into Metasploit for further exploitation.
