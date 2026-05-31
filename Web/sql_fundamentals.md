# SQL Fundamentals

## Overview
- SQL is used to create, retrieve, modify, and delete data in databases.
- Databases store information in structured tables made of rows and columns.

## Key Concepts
- A database is an organised collection of data stored in tables made of rows and columns.
- Databases are managed by a DBMS (Database Management System) such as MySQL and SQLite.
- A semicolon (;) terminates an SQL command.

## CRUD Operations
- CREATE - Create new records
- READ - Retrieve records
- UPDATE - Modify existing records
- DELETE - Permanently remove records

## Common SQL Statements
- SELECT - Used to retrieve data:
```
SELECT * FROM users;
```
- INSERT - Adds new records:
```
INSERT INTO users (username, password)
VALUES ('admin', 'password');
```
- UPDATE - Modify existing data:
```
UPDATE users
SET password='newpass'
WHERE username='admin';
```
- DELETE - Remove data:
```
DELETE FROM users
WHERE username='admin';
```

## Clauses & Operators
- WHERE - Filter results
- LIKE - Matches a pattern
- AND / OR - Combine conditions
- LIMIT - Restrict returned rows
- UNION - Combine results from multiple queries

## Relevance
- Essential for managing and querying data.
- Forms the foundation of database-driven web applications.
- Crucial for understanding SQL injection vulnerabilities.
