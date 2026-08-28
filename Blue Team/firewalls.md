# Firewalls

## Overview
- Covers what firewalls are, the different types of firewalls, and how rules are configured.

## Key Concepts
- A **firewall** inspects incoming and outgoing traffic on a device or network and allows or denies it based on defined rules.
- It is the first line of defence in any network security architecture.

## Types of Firewalls
- **Stateless** - Filters packets based on static rules (IP, port, protocol) - no connection awareness.
- **Stateful** - Tracks the state of active connections and stores them in a state table - more advanced filtering.
- **Proxy** - Acts as an intermediary, operates on Layer 7 - inspects packet contents and masks internal IPs.
- **Next-Generation (NGFW)** - Operates on Layers 3–7 - includes IPS, heuristic analysis, and SSL/TLS inspection.

## Firewall Rules
- Rules define if traffic is allowed or denied. Each rule specifies:
  - **Source** / **Destination** - IP address or range
  - **Port** - Specific service (e.g. port 22 = SSH, port 443 = HTTPS)
  - **Protocol** - TCP or UDP
  - **Direction** - Inbound or Outbound
  - **Action** - Allow or Deny

## Firewall Tools
- Windows Defender Firewall - Built-in firewall included with Windows OS.
- Linux tools:
  - **Netfilter** - Core Linux kernel framework - handles packet filtering and NAT.
  - **iptables** - CLI tool for managing Netfilter rules.
  - **nftables** - Successor to iptables - more modern syntax.
  - **ufw (Uncomplicated Firewall)** - Simplified frontend for iptables - easier rule management.

## Common ufw Commands
```
ufw enable                        # Enable the firewall
ufw allow 22/tcp                  # Allow SSH
ufw deny outgoing                 # Block all outbound traffic
ufw default deny incoming         # Block all inbound traffic by default
ufw status                        # View current rules
```
## Relevance
- Defenders use firewalls to restrict attack surface; attackers look for misconfigured rules to bypass them.
- Practical knowledge of Windows Defender Firewall and Linux ufw/iptables is directly applicable to SOC, sysadmin, and penetration testing roles.
