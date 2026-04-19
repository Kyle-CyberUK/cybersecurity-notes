# Core Networking Protocols

## Overview
- Networking protocols define how data is transmitted, how connections are established, and how devices communicate across networks.

## TCP vs UDP
- Transmission Control Protocol (TCP):
  - Connection-oriented (requires a connection before sending data).
  - Slower but guarantees delivery in the correct order.
  - Uses acknowledgements and retransmissions.
- User Datagram Protocol (UDP):
  - Connectionless (does not require setup).
  - Faster but no guarantee of delivery.

## DNS (Domain Name System)
- Translates domain names into IP addresses.
- Example: google.com > IP address.
- Useful for locating services on the internet.

## HTTP and HTTPS
- Hypertext Transfer Protocol (HTTP):
  - Sends data in plain text (unsecure).
- Hypertext Transfer Protocol Secure (HTTPS):
  - Secure version.
  - Uses encryption via TLS (Transport Layer Security).

## FTP (File Transfer Protocol)
- Used to transfer files between systems.
- Not secure by default (data is unencrypted).
- Replaced by secure alternatives like SFTP (SSH FTP).

## Email Protocols
- SMTP (Simple Mail Transfer Protocol)
  - Used to send emails between mail servers.
- POP3 (Post Office Protocol v3)
  - Downloads emails to a device.
- IMAP (Internet Message Access Protocol)
  - Keeps emails on the server and syncs across multiple devices.

## Relevance
- Understanding networking protocols is essential for:
  - Traffic analysis – Identifying normal vs suspicious network behavior.
  - Security – Recognizing unsecure protocols (e.g. HTTP & FTP).
  - Troubleshooting – Diagnosing connectivity and communication issues.
  - Cybersecurity operations – Used in both defensive monitoring and offensive testing.
