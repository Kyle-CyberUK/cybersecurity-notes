# Hashing

## Overview
- Hashing is used in cryptography to protect passwords and verify data integrity.

## Key Concepts
- A hash function produces a fixed-length output from input data.
- Hashing is **one-way** and cannot be reversed.
- The same input always produces the same output.
- Passwords are stored as hashes instead of plain text.
- **Salting** adds random data before hashing to prevent rainbow table attacks.
- **Rainbow table attacks** use precomputed hashes to crack passwords.
- Common algorithms include MD5 and SHA-1 (insecure), and SHA-256.
- Hashing is used to verify that data has not been altered.

## Relevance
- Protects passwords from being exposed if compromised.
- Detects tampering with files and data.
- Used in authentication and system security.
