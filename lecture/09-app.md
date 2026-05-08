# 1.Application whitelisting/blacklisting
- AppLocker
# 2.application Sandboxing
- Linux: Firejail
- Sophos: Sandboxie
- Windows Defender Application Guard(WDAG: isolate Microsoft Edge)
# 3.Application Patch Management
# 4.Web Application Firewall
- layer 7, rule-based filter
- types
    - hardware/network: all web applications on the network
    - software/host: single web server
    - cloud: controlled by third-party
- benifigt: [cookie, CSRF, parameter tampering, data validatoin issue]
- Microsoft URLSacn: WAF for IIS

- Sofetware Restriction Policies (**SRP**), AppLocker
- firejail firefox | Windows Sandbox, Windows Defender Application Guard | Sandboxie
- SolarWinds [Microsoft Windows Server Update Services(**WSUS**), System Center Configuration Manager(**SCCM**)]
- WAF [CSRF, Parameter Tampering, Data Validation Issues]
- Microsoft, Internet Server Application Programming Interface (**ISAPI**)