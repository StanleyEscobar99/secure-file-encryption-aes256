# Secure File Encryption and Transfer (AES-256)

## Overview
Hands-on cybersecurity lab demonstrating secure file encryption, key management,
secure file transfer, and controlled access to encryption keys using Windows systems.

## Tools Used
- Windows PowerShell
- OpenSSL
- SCP / SSH
- Thunderbird

## Lab Steps Completed

### Step 1 — Generate AES-256 Key (ZYWIN01)
- Generated `finance.key` using OpenSSL.
- Screenshot: LAB.Securing.sensitive.financial.data.1.png

### Step 2 — Transfer Key Using SCP (ZYWIN01 → ZYWIN02)
- Securely transferred the encryption key using SCP.
- Screenshots:
  - LAB.Securing.sensitive.financial.data.2.png
  - LAB.Securing.sensitive.financial.data.2.1.png

### Step 3 — Apply Least-Privilege Permissions (ZYWIN02)
- Granted read-only access to Rina for `finance.key`.
- Screenshot: LAB.Securing.sensitive.financial.data.3.png

### Step 4 — Encrypt Financial Report (ZYWIN01)
- Encrypted `financialReport.xlsx` using AES-256-CBC.
- Screenshot: LAB.Securing.sensitive.financial.data.4.png

### Step 5 — Email Encrypted File
- Sent `financialReport.xlsx.enc` to Rina via email.
- Screenshots:
  - LAB.Securing.sensitive.financial.data.5.png
  - LAB.Securing.sensitive.financial.data.5.1.png

### Step 6 — Decrypt File (ZYWIN02)
- Decrypted the encrypted file using `finance.key`.
- Screenshot: LAB.Securing.sensitive.financial.data.6.png

## Skills Demonstrated
- AES-256 symmetric encryption
- Secure key management
- SCP / SSH secure file transfer
- Access control and least privilege
- Secure data transmission and verification
