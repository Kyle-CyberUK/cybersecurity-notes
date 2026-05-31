# JavaScript Essentials

## Overview
- How JavaScript works and how attackers can abuse legitimate functionality for malicious purposes.

## Key Concepts
- JavaScript is an interpreted language; code runs directly in the browser with no compilation.
- It works alongside HTML and CSS to make pages interactive and dynamic.
- Variables - Store data values — declared with var, let, or const.
- Data Types - Strings, numbers, booleans, objects, and arrays.
- Functions - Reusable blocks of code for specific tasks.
- Loops - Repeat a code block while a condition is true.

## Integrating JS in HTML
- Internal – JS written directly inside the HTML file.
- External – JS linked as a separate .js file.

## Dialogue Functions
- `alert()` - Creates a browser pop-up with a message for the user.
- `prompt()` - Creates a browser pop-up prompting the user to input information.
- `confirm()` - Creates a browser pop-up asking the user to confirm or deny an action.
- Attackers can abuse these for phishing or social engineering attacks.

## Minification & Obfuscation
- Minification – Strips whitespace and shortens code to reduce file size.
- Obfuscation – Makes code harder to read and reverse engineer.
- Both are used in production to hinder attackers — but a determined attacker can still reverse them.

## Secure Coding Practices
- Never store API keys or credentials in JS — it's visible to anyone in the browser.
- Always validate on the server side — client-side validation can be bypassed.
- Sanitise user input to prevent XSS (Cross-Site Scripting) attacks.
- Only use trusted libraries — unknown scripts can introduce malware.

## Relevance
- Understanding how JS works enables recognition of XSS vulnerabilities and malicious script abuse.
