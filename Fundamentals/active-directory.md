# Active Directory

## Overview
- Active Directory (AD) allows administrators to manage users, devices, and security policies from a central location called a Windows domain.

## Windows Domain
- A group of users managed centrally through Active Directory.
- The server responsible for Active Directory services is called a Domain Controller (DC).
- Benefits include:
  - Centralized user management.
  - Centralized security policies.
  - Easier administration of larger networks.

## Active Directory Objects
- Active Directory stores information as objects.
- Common objects include:
  - Users - Employees or services
  - Machines - Devices joined with the domain
  - Groups - Collections of users or computers with shared permissions.

## Organizational Units (OUs)
- Containers used to organise users, devices, and groups inside Active Directory.
- Commonly structured based on specific departments such as IT, Marketing, or Sales.
- Help administrators apply different policies to different departments.

## Group Policy Objects (GPOs)
- Collections of rules that control how devices and users behave.
- Examples include:
  - Restricting access to the Control Panel.
  - Enforcing password policies.
  - Locking screens after inactivity.

## Authentication Protocols
- Kerberos is the default authentication protocol for Windows domains that uses tickets which prove a user has already authenticated.
- NetNTLM is an older authentication protocol that uses a challenge-response mechanism to verify credentials.

## Domain Trees and Trusts
- Large organisations may have multiple domains.
- These domains can be connected using:
  - Trees - Multiple domains sharing same namespace.
  - Forests - Groups of domain trees.
  - Trusts - Allows users from one domain to access resources in another domain.

## Relevance
- Understanding how large corporate networks are structured.
- Identifying privilege escalation.
- Investigating compromised accounts.
- Managing authentication and access control.
