# Gobuster

## Overview
- Gobuster is a web enumeration tool used during reconnaissance to discover hidden content on web servers.
- It helps identify directories, files, subdomains, and virtual hosts that may not be publicly accessible.

## Key Concepts
- Enumeration is the process of discovering information about a target system.
- Gobuster automates this process by using wordlists.
- Gobuster sends requests using entries from a wordlist and reports results based on HTTP responses.
- The effectiveness of enumeration depends on the quality of the wordlist used.

## Directory Enumeration
- Discovers hidden directories and files on a web server.
- Requires the target URL and the provided wordlist.

## Subdomain Enumeration
- Identifies subdomains associated with a target domain.
- Uses DNS requests to brute-force potential subdomains.
- Requires the target domain and the provided wordlist.

## Virtual Host Enumeration
- Discovers multiple websites hosted on the same server/IP address.
- Uses the HTTP 'Host**'** header to identify hidden vhosts.
- Requires the target URL and the provided wordlist.

## Relevance
- Essential reconnaissance tool for penetration testing.
- Often used before vulnerability scanning and exploitation.
