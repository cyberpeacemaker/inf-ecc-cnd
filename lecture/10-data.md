# 1. Data Security
- Access Control, Encryption, [Masking, Backup, Destruction], Retention, Harware-based Security
# 2. Data Access Control
- Methods: [Access Control Lists(ACL), Group Policy, Account Restriction, Password/ Acces Token]
# 3. Encryption Data at Rest
- Disk Encryption: [Windows:BitLocker, Mac:FileVault, Linux:dm-crypt], VeraCrypt
- File-level Encryption: [Windows:Encrypting File System(EFS), MacOS:Disk Utility, Linux:GnuPrivacy Guard(GPG)]
- Removable Media Encryption: [Windows:BitLocker]
- Database Encryption: [MS SQL:Transparent Databse Encryption (TDE)], Alwasy Encrypted
# 4. Encryption Data at Transit
# 5. Encryption Data at Transit "Browser <-> Web Server"
- https, CA, Certificate Revocation List (CRL)
# 6. Encryption Data at Transit "Database <-> Web Server"
# 7. Encryption Data at Transit "Email"
- S/MIME
- SSL/TLS
# 8. Masking, Backup, Retention (Compliance)
- Masking(Obfuscation/Anonymization): hiding original data with random character
- Backup: [full/normal, differential, incremental] 
    - recovery drill test
    - Redundant Array of Independent Disk (**RAID**)
    - Direc Attached Storage (**DAS**), Storage Area Netwrok (**SAN**), Network Attached Storage (**NAS**)
# 9. Data Destruction
- [Clearing:[overwriting, Wiping, Erasure], Purging:Degaussing, Destroying:[Disintegration, incineratoin, melting, Shredding]] 
# 10 Data Loss Prevention(DLP)
- do not allow users to send confidential corporate data
- Windows Information Protection (**WIP**)

