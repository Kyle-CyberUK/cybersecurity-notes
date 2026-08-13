# Shells Overview

## Overview
- Shells Overview covers the different types of shells used in offensive security; how they work, when to use them, and how attackers deploy them.

## Key Concepts
- A shell is a command-line interface that lets a user interact with an OS.
- What attackers use shells for:
  - Remote system control
  - Privilege escalation
  - Data exfiltration
  - Persistence (backdoors, hidden accounts)
  - Pivoting — Using a compromised system to attack others on the network

## Shell Types
- Using a "reverse shell" allows the target to connect back to the attacker - bypasses firewalls.
- A "bind shell" binds a port on the compromised system and listens for a connection.
- A "web shell" is a malicious script uploaded to a web server; the commands are sent via the URL.

## Shell Listeners
- Rlwrap is a small utility tool that wraps a listener to add arrow keys and command history.
- Ncat is a superior version of Netcat, providing extra features like SSL encryption.
- Socat is a utility tool that creates a socket connection between two data sources - more flexible than nc.

## Shell Payloads
- Commands run on the target to send a shell back.
- Common languages include:
  - Bash
  - PHP
  - Python

## Web Shells
- A script uploaded to a vulnerable web server.
- Example PHP web shell:
```
<?php
    if(isset($_GET['cmd']))
    {
        system($_GET['cmd'] . ' 2>&1');
    }
?>
```
- Common upload vulnerabilities exploited:
  - Unrestricted file upload
  - File inclusion
  - Command injection
- Popular web shells: p0wny-shell, b374k, c99

## Relevance
- Shells are central to the exploitation and post-exploitation phases of penetration testing.
- Understanding how to set up, catch, and use shells manually, without tools like Metasploit, builds deeper knowledge of how attacks work.
