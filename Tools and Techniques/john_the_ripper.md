# John the Ripper

## Overview
- **John the Ripper** is a popular open-source password cracking tool.
- It identifies weak passwords by attempting to crack password hashes.

## Key Concepts
- Cracks password hashes by guessing possible plaintext values.
- Supports many hash formats.
- Works with different types of data such as hashes from files, captured hashes, and encrypted files.
- Multiple modes:
  - Wordlist mode uses a predefined list of passwords, fast for common passwords.
  - Single crack mode uses usernames and related information.
  - Incremental mode is essentially brute force; it tries all possible combinations, very slow but thorough.
- It's important to know the hash type before cracking; use tools like **hashid** or **hash-identifier**.
- John provides utilities to extract hashes from certain files: **zip2john**, **ssh2john**, and **rar2john**.

## Relevance
- Widely used in penetration testing and security auditing to assess password strength.
- Encourages the use of strong passwords, salting, and multi-factor authentication.
