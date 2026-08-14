# SQLMap

## Overview
- How websites interact with databases, how attackers manipulate SQL queries, and how to enumerate and extract data using SQLMap.

## Key Concepts
- Websites interact with databases using SQL queries, like checking login credentials against stored records.
- When user input is not properly sanitised, attackers can manipulate those queries.
- A login form with no input validation can be bypassed using:
  - `password = 'abc' OR 1=1;-- -';`
- This modifies the SQL query so that `1=1` (always true) causes it to succeed regardless of the actual password.
- The `-- -` comments out the rest of the query.
- SQLMap automates this process by detecting injection points and extracting the data.

## Core SQLMap Commands
- `sqlmap -u <URL>` - Test a GET-based URL for SQLi
- `sqlmap -r req.txt` - Test using a saved POST request file
- `--dbs` - List all available databases
- `-D <db> --tables` - List tables in a specific database
- `-D <db> -T <table> --dump` - Dump all records from a table
- `--level=5` - Run deeper, more thorough scans
- `--wizard` - Step-by-step guided mode for beginners

## GET & POST Testing
- GET-based - Parameters visible in the URL (`?email=test&password=test`) — pass directly with `-u`.
- POST-based - Data sent in the request body (login/registration forms) — intercept with Burp Suite, save as a file, and pass with `-r`.

## Relevance
- SQL injection is consistently one of the most exploited web vulnerabilities.
- SQLMap is a core tool in any pentester's toolkit, used for quickly identifying and extracting data from vulnerable databases.
