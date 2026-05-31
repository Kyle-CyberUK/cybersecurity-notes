# Web Application Basics

## Overview
- Introduces how web applications are structured and how browsers communicate with servers.
- It covers URLs, HTTP requests and responses, and security headers.

## Key Concepts
- `Front End` – HTML (structure), CSS (styling), JavaScript (behaviour).
- `Back End` – Web server, database, and supporting infrastructure.
- `WAF` (Web Application Firewall) – Filters malicious requests before they reach the server.
- URLs are broken into components: scheme, host, port, path, query string, and fragment.
- HTTPS encrypts traffic; always prefer it over HTTP.
- `Typosquatting` — Attackers registering near-identical domains for phishing.
- HTTP messages follow the structure: Start Line > Headers > Body. There are two types:
  - `Request` – sent by the client (method + path + headers + body).
  - `Response` – sent by the server (status code + headers + body).

## Core HTTP Methods
- `GET` - Fetch data; never include secrets in parameters.
- `POST` - Send/create data; sanitise input (SQLi/XSS).
- `PUT / DELETE` - Update/remove; enforce authorisation.

## Status Code Groups
- 1xx - Informational
- 2xx - Success
- 3xx - Redirection
- 4xx - Client error
- 5xx - Server error

## Security Headers
- `Content-Security-Policy` - Restricts resource origins; mitigates XSS.
- `Strict-Transport-Security` - Forces HTTPS connections.
- `X-Content-Type-Options: nosniff` - Prevents MIME type sniffing.
- `Referrer-Policy` - Controls URL info shared on navigation.
- Cookie flags to always set: `Secure` (HTTPS only) and `HttpOnly` (blocks JS access).

## Relevance
- Traffic interception with tools like Burp Suite, identifying misconfigurations, and testing for injection vulnerabilities all depend on knowing how requests and responses work.
- Security headers are a quick, high-impact way to harden a web application.
