# FILE-INTEGRITY-CHECKER

COMPANY: CODTECH IT SOLUTIONS

NAME: Aashray Premkumar Dhone

INTERN ID: CODHC173

DOMAIN: Cyber Security & Ethical Hacking

BATCH DURATION: January 30th, 2025 to March 2nd, 2025

MENTOR NAME: Neela Santhosh Kumar

OUTPUT: 

File Integrity Checker (Python Script) This Python script ensures file integrity by generating and verifying cryptographic hashes. It calculates the hash of a file using a specified algorithm (default: SHA-256) and detects if the file has been modified.

How It Works: Generate Hash: The script calculates and displays the original hash of the file. Check Integrity: After any modifications, it compares the current hash with the original to verify file integrity. Features: Uses cryptographic hash algorithms (default: SHA-256). Detects unauthorized changes or corruption in files. Simple and interactive command-line interface.

1] os:

Handles file paths and system-level interactions (though it's not actively used in the provided code but might be useful for extensions). 2] hashlib:

Provides cryptographic hashing functions (e.g., MD5, SHA-1, SHA-256). Used to create and update the hash for the file.

Here’s a description of how the script works:

How the Script Works Generate File Hash:

The script reads the file in chunks (4096 bytes at a time) to efficiently handle large files. A cryptographic hash (default: SHA-256) is calculated for the file using the hashlib library. The hash value is displayed as the "original hash." Wait for File Modification:

The script pauses after displaying the original hash, allowing the user to modify the file if needed. Check File Integrity:

The script re-calculates the file's hash and compares it with the original hash. If the hashes match, the file is confirmed as "intact." If the hashes differ, the script warns that the file has been "modified."
