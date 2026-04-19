# Tcpdump

## Overview
- Tcpdump is a command-line tool used to capture and analyse network traffic.
- It is lightweight and runs entirely in the terminal.
- Capturing packets typically requires root or sudo privileges.

## Key Concepts
- Built on the libpcap library.
- `-i <interface>` – Capture packets from a network interface.
- `-w file.pcap` – Save captured traffic to a file.
- `-c <number>` – Limit the number of captured packets.
- `-r file.pcap` – Read and analyse saved captures.
- `-v / -vv / -vvv` – Increase output detail.
- `src host <IP>` / `dst host <IP>` – Filter by source or destination IP.
- `port <number>` – Filter by port (e.g., 80).
- `tcp`, `udp`, `icmp` – Filter by protocol.
- `-n / -nn` – Disable hostname and port resolution.
- `| wc -l` – Count captured packets.

## Relevance
- Widely used in incident response and network analysis.
- Helps detect suspicious traffic and investigate security events.
- Useful for diagnosing network connectivity issues.
