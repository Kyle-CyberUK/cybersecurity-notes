# Cryptography

## Overview
- Cryptography secures communication by preventing attackers from reading or modifying data as it travels across networks.

## Key Concepts
- Plaintext - The original readable message.
- Ciphertext - The scrambled message after encryption.
- Key - The secret value used to encrypt and decrypt data.
- Algorithm - The mathematical process used to transform plaintext into ciphertext using a key.

## Symmetric Encryption
- Uses the same shared key for encryption and decryption.
- Fast and efficient.
- Used for encrypting large amounts of data.

## Asymmetric Encryption
- Uses two related keys:
  - Public key - Shared openly, used to encrypt messages.
  - Private key - Kept secret, used to decrypt messages.

## Hybrid Encryption
- Combines both symmetric and asymmetric encryption.
- Example: HTTPS
  1. Asymmetric is used to securely exchange a symmetric key.
  2. Symmetric is then used as it is faster.

## Relevance
- Cryptography supports confidentiality by keeping data secure and integrity by preventing modification. It also ensures secure communication over untrusted networks.
