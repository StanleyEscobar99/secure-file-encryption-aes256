# secure-file-encryption-aes256

## Overview
This project documents a hands-on Windows cybersecurity lab focused on protecting sensitive financial data using encryption, secure key handling, and secure file transfer.

## Tools Used
- Windows PowerShell
- OpenSSL
- SCP / SSH
- Thunderbird

## Lab Goals Completed (6 Steps)

### Step 1 — Generate AES-256 Key (ZYWIN01)
- Created the EncryptionKeys folder and generated `finance.key` using OpenSSL.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.1`

### Step 2 — Transfer Key Using SCP (ZYWIN01 → ZYWIN02)
- Securely transferred `finance.key` to ZYWIN02 using SCP.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.2`
- - **Screenshot:** `LAB.Securing.sensitive.financial.data.2.1`

### Step 3 — Grant Read-Only Access (ZYWIN02)
- Used file permissions (icacls) to grant read-only access to Rina for `finance.key`.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.3`

### Step 4 — Encrypt Financial Report (ZYWIN01)
- Encrypted `financialReport.xlsx` using AES-256-CBC and saved output as `financialReport.xlsx.enc`.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.4`

### Step 5 — Email Encrypted File (ZYWIN01 → ZYWIN02)
- Emailed `financialReport.xlsx.enc` to Rina for saving in `C:\Users\Rina\Documents` on ZYWIN02.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.5`
- **Screenshot:** `LAB.Securing.sensitive.financial.data.5.1`

### Step 6 — Decrypt Encrypted File (ZYWIN02)
- Decrypted `financialReport.xlsx.enc` using `finance.key`, restoring `financialReport.xlsx`.
- **Screenshot:** `LAB.Securing.sensitive.financial.data.6`

## Skills Demonstrated
- Symmetric encryption (AES-256-CBC)
- Key management and secure storage
- Secure file transfer (SCP/SSH)
- Access control / least privilege
- Secure communication workflow and verification
