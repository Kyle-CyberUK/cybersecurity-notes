# IDS Fundamentals

## Overview
- Covers what an Intrusion Detection System is, the different types, and use of Snort (the most widely used open-source IDS solution)

## Key Concepts
- An **IDS (Intrusion Detection System)** monitors network or host activity and alerts security teams when suspicious behaviour is detected.
- Unlike a firewall, an IDS only detects threats.

## Deployment Modes
- **HIDS** (Host-based) - Installed on individual hosts - detailed visibility but resource-intensive.
- **NIDS** (Network-based) - Monitors traffic across the entire network - broader coverage.

## Detection Methods
- **Signature-based IDS** - Matches traffic against known threat patterns - fast but unable to detect zero-day attacks.
- **Anomaly-based IDS** - Flags deviations from normal behaviour - catches unknown threats but creates more false positives.
- **Hybrid IDS** - Combines both methods for broader detection coverage.

## Snort
- **Snort** is the most widely used open-source IDS - uses both signature-based and anomaly-based detection.
- Main Snort directory: `/etc/snort/`
- Snort modes:
  - **Sniffer Mode** - Reads and displays packets in real time.
  - **Packet Logging Mode** - Logs network traffic to a PCAP file.
  - **NIDS Mode** - Primary mode - analyses traffic and generates alerts.
- Snort rule structure:
  - action protocol src_ip src_port -> dst_ip dst_port (options)
- Key rule fields:
  - `msg` - Alert message displayed when rule triggers.
  - `sid` - Unique signature ID for the rule.
  - `rev` - Revision number of the rule.

## Relevance
- IDS solutions like Snort are a core part of any SOC's detection stack.
- Understanding how traffic is monitored, how rules are written, and how alerts are generated is directly applicable to SOC Analyst work, incident response, and network security monitoring.
