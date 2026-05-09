# 1.Application whitelisting/blacklisting
- AppLocker
- Sofetware Restriction Policies (**SRP**)
# 2.application Sandboxing
- Linux: Firejail
- Sophos: Sandboxie
- Windows Defender Application Guard(WDAG: isolate Microsoft Edge)
# 3.Application Patch Management
- SolarWinds [Microsoft Windows Server Update Services(**WSUS**), System Center Configuration Manager(**SCCM**)]
# 4.Web Application Firewall
- layer 7, rule-based filter
- types
    - hardware/network: all web applications on the network
    - software/host: single web server
    - cloud: controlled by third-party
- benifigt: [cookie, CSRF, parameter tampering, data validatoin issue]
- Microsoft URLSacn: WAF for IIS

---


- Microsoft, Internet Server Application Programming Interface (**ISAPI**)