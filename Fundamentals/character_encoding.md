# Character Encoding

## Overview
- Computers store and transmit text using character encoding systems, which map characters to numerical values.

## ASCII (American Standard Code for Information Interchange)
- Uses 7 bits, allowing 128 characters.
- Covers letters, digits, punctuation, and control characters.
- Example: Uppercase A = 01000001 (binary) or 41 (hexadecimal).

## Extended ASCII
- Uses 8 bits, allowing 256 characters.
- Includes standards like ISO-8859-1 and ISO-8859-2.
- Different mappings can cause incorrect character display if encoding mismatches occur.

## Unicode
- A universal character encoding standard.
- Supports characters from all languages, symbols, and emojis.
- Each character has a code point (e.g. U+0041 = A)

## UTF Encodings
- UTF-8 – Most common on the web. Uses 1–4 bytes per character. Example: A = 0x41.
- UTF-16 – Uses 2 or 4 bytes per character. Example: A = 0x0041.
- UTF-32 – Uses 4 bytes per character. Simple but wastes space. Example: A = 0x00000041.

## Relevance
- Character encoding is essential because it ensures text portability, data storage and transmission, globalization support, and web and software development.
