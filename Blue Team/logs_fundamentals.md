# Logs Fundamentals

## Overview
- Covers what logs are, the different types, and how to analyse them during an investigation.

## Key Concepts
- **Logs** are the digital footprints left behind by any activity on a system.
- They are the primary source of attack traces during an investigation.
- Types of logs:
  - **System** - Troubleshooting OS-level issues
  - **Security** - Authentication and authorisation events
  - **Application** - Events specific to an application
  - **Audit** - System changes and user activity
  - **Network** - Incoming and outgoing network traffic
  - **Access** - Detailed access to resources

## Windows Event Logs
- Windows logs activities across three main categories: Application, System, and Security.
- Each event has a unique event ID, below are some common event IDs:
  - 4624 - Successful user logon attempt
  - 4625 - Failed user logon attempt
  - 4634 - A user account successfully logged off
  - 4720 - A user account was created
  - 4724 - An attempt was made to reset an account's password
  - 4726 - A user account was deleted

## Web Server Access Logs
- Every request made to a web server is logged. Each entry contains:
  - **IP Address** - Who made the request
  - **Timestamp** - When it was made
  - **Request** - HTTP method, URL, status code
  - **User-Agent** - Browser or tool used

## Relevance
- Log analysis is a core daily task for SOC Analysts.
- Being able to read Windows Event Logs and web server logs, filter by Event ID, and use Linux CLI tools to search log files is directly applicable to any SOC analyst work, incident response, and digital forensics investigations.
