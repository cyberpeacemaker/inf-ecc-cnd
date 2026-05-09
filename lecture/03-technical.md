# 1. Access Control
- [user identification, authentication, authorization]
- Seperation of Duties(Sod), General Data Protection Regulation(GDPR)
# 2. Redefine
- NIST Zero Trust Archietecture (ZTA): [prepare, categorize, select, implement, assess, authorize, monitor]
- Principle of Least Privilege(PoLP)
# 3. Identity and Access Management(IAM)
- right individual with right access at the right time
- User Identity Management(IDM): individual holds a valid identity
- User Access Management (AM): Authentication
- Privilege Access Management (PAM): Authorize the security function
- chanllenge-response authentication mechanism (CRAM)
# 4. Cryptographic Techs
# 5. Cryptogrphaic Algos
- DES(Data Encryption Standard), AES(Advanced Encryption Standard), RC4(WEP)
- DSA(Digital Signature Algorithm), RSA(Rivest-Shamir-Adleman)
- MD5(Message Digest), SHA(Secure Hash Algorithm)
- Hash-based Message Authentication Code (HMAC)
# 6. Network Segmentation
# 7. Solutions
- Firewall, IDS(Snort, Suricata)/IPS, honypot, proxy server, web content filter
- network access control(NAC), SIEM, SOAR(Splunk)
# 8. Protocals
- TACACS+: secure client-server, encrypt [username + password], port:49
- RADIUS: Encrypt only password
- OpenPGP: ElGamal, S/MIME:Deffie-Hellman
- IPsec: [AH, ESP], [Tunnel mode, Transport mdoe]

---

# Extensible Authentication Protocol (EAP) 
是一種廣泛應用於網路存取技術（如 Wi-Fi 和乙太網路）的認證框架。
值得注意的是，EAP 本身並不是一種具體的認證機制，而是一個「傳輸協議」。它定義了認證數據如何在設備（如筆電）與認證伺服器（如 RADIUS）之間傳遞。你可以把它想像成一個「信封」，信封裡面可以裝載不同的認證信件（如密碼、憑證或動態密鑰）。