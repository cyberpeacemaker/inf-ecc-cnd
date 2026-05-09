# 1.Loggin Concept
- compliance with laws, rules, regulations
- local logging(system crash), centralized logging(addition of network devices)
# 2.Log Analysis on Windows
- `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\EventLog\<Event Log>`
- Event Type
    - Error: significant problem (data loss)
    - Warning possible future problem (disk space is low)
    - Information: successful operation
    - Success Audit
    - Failur Audit
- System log: os, harware, driver, service pack, power on/off
- Application log: software, firewall
- Security log: log on/off, connection, policy
- 4624 (acc logon), 4625 (acc FAILED logon), 4647 (acc logoff)
# 3.Log Analysis on Linux
- `/var/log` in plain ASCII text format
- Security Level ((E)very (A)wesome (C)isco (E)ngineer (W)ill (N)eed (I)cecream (D)aily)
    - Warning(4): Warning conditions
    - Notice(5): Nomral but significant
# 4.Log Analysis on Mac
- Types
    - Security: `/private/var/log`
    - Firewall: `/private/var/log/appfirewall.log`
    - User Specific: `~/Library/Logs`
    - Command Line: `.bach_history`
    - Shared Application: `/Library`
- System Logs: `/private/var/log/system.log`
# 5. Log Analysison Firewall
- Windows Defender: `C:\Windows\System32\LogFiles\Firewall\pfirewall.log`
- Linux iptables: `/var/log/messages`
- MAC OS X: `/privat/var/log/appfirewall.log`
- Cisco ASA Firewall: DoS attack protection, [timestamp, Device ID, Message ID(severity), Message Text]
- Check Point Firewall: integrated with an inspectino module lives in the OS kernel, `fw log`
# 6. Log analysis on Router
# 7. Log analysis on Web Server
- `var/log/httpd/access_log`
# 8. Centralized Log
1. Collection: various src to central location
2. Transmission: logs are transmitted using various log transport mechanisms
3. Storage: size, importance(time), accessibility
4. Nomralization: from heterogeneous source
5. Correlation: rule-based, statistical, algorithmic
6. Analysis: intelligent decision
7. Alerting and Reporting