# q11
- S/MIME: RSA
# 13
- sudo netstat -tunlp: list all port. | Displays protocol statistics and current TCP/IP network connections.
# 14
- SOX (Sarbanes-Oxkey Act if 2002): traded company, accountint firm
- GLBA (Gramm-Leach-Bliley Act): financial institution
- FISMA (Federal Information Security Management Act): protect government info
- DMCA (Digital Millennium Copyright Act): Intellectual Property Law
# 16
- SYN scan (-sS)
- NULL, XMAX (-sN, -sX)
- ACK (-sA)
# 18
- DDoS [App/Netwrok]-centric
# 23, 87
- Security Reference Monitor (**SRM**):  kernel-mode | Ntoskrnl.exe | check user/process has the rights to access
- WinLogon and NetLogon: login interface
- Security Account Manager(**SAM**): database file (registry hive) | store user account and group hashed password
- Local Security Ahtuority Subsystem(**:LSASS**): user-mode process | brain of the authentication sub-system | policy, token, audit, log
# 24, 37, 108
- TCP Flag [ack, push, rst, syn, fin]
# 27, 131 UPS
- Standby-Ferro: legacy, home
- line Interactive: small business
- Double Conversion On-Line: isolation, 10kVA, convert AC to DC, mission-crtical DC
- Delta Conversion On-Line: modern double, Large DC
# 34, 127
- AppLocker: Path Rule
# 41
- Integrated NAS: Head, Network Interface, Storage all bundled into a single 'appliance'
- Gateway NSA: independent Head
- FreeNAS: Software
# 44, 91, 117, 121
- RAID 0: dara stripping
- RAID 1: mirror
- RAID 3: partial cks
- RAID 5: 1 disk
- RAID 6: 2 disk
- RAID 50: at least 3
# 45, 136 incident triage
- analysis, classification
- prioritization, notification
- containment, evidence gathering
- eradication, recovery
# 50 SNMP
- TRAPS:PUSH for Help
- INFORM PUSH | SNMPv2c | Need manager send back confirm
- RESPONSE: agent back to manager
- SET: managet to agent
# 51 
- Amazon EC2 (Elastic Compute Cloud): Iaas (Infrastructure as a Service)
# 54 
- REDHAT up2date -d -f -u
# 55, 96
- IoE
- IoA
- IoC
- KRI (Key Risk Indicator): Notify, Identify, backward looking view
# 56
- VPN Concentrator [Security Key, User Address, I/O Operation]
# 58
- SATA: hot plugging
# 59
- risk Assesment: what could go wrong
- BIA: if goes wrong, how abd is it (RTO/RPO)
- Disaster Recovery Strategy: How do we meet (RTO/RPO)
- BCP: final plan everyone follows
# 64, 115
- `Get-WindowsOptionalFeature -Online -Feature smb1 protocol` (NO s)
# 65
- Iris recognition: Front | Colored Ring
- Retianl Scanning: Back | Blood vessel
# 67
- `--cpus="2"`
# 71
- NIST: IoT
# 76
- Azure: MicroBurst | Cloud
# 77, 113
- Risk = Asset + Threat + Vulnerability
- Attack = Motive(goal) + Method + Vulnerability
# 79, 135
- 802.11b
- 802.16: MAM
# 82
- WEP
- WPA
- WPA2
- WPA3
# 83
- Para Virtualization (OS Assisted): it knows it is not running on physical hardware
# 86
- nwtowrk sniffing [Telnet Passwords, DNS traffic, Syslog Traffic]
# 88
- SAS (Serial Attached SCSI): connection type
- SAN (Storage Area Network): independent network connect servers to data storage device
- NAS (Network Attached Storage): lives on existing LAN
# 89, 129
- Debian: apt-get
- Red Hat: up2date > yum > dnf
- Slackware: Swaret
- AutoupdateL RPM
# 90
- SSID cloaking
# 92
- extreme
# 93
- AWS CloudTrial
# 98
- pull-based : client-server
- Network-based
- push-based
- host-based
# 101, 133
- IoT Chip-level: JTAG
- TooL: SET
# 102, 106
- star: easy to expand
- Bus:
- Mesh:
- Ring:
- Ad-Hoc: same channel name and SSID
# 103
- PGP: App Layer
# 104
- AWS Shared Reponsibility Model: [Container, Abstract, Infrastructure]
# 105, 107
- Network access policy [Promiscuous, Permissive, Prudent, Paranoid]
# 109
Authorization
- centralized: RADIUS
- decentralized
- implicit: assumed
- explicit: clearly stated
# 110, 118 BC/DR
- Risk Assesment, Business Impact Analysis, RTO, RPO
- Data-centric
- BC/DR [Prevention, Response, Resumption, Recovery, Restoration]
# 111
- Win: BitLocker, Device Encryption
- Mac: FileVault
- Linux: dm-crypt
# 114
- Dry chemical
# 119
- Apache: /var/log/httpd
# 120
- WASC(Web Application Security Consortium): create, refine and promote internet safety standdards
# 122
- content-basedL payload
- context-based: Header (IP, protocol, cks)
- atomic-signature-based: simge packet
- composite-signature-based: multiple packet
# 124
- registry [Resplendent registrar, Reg.exe, Regedit.exe]
# 125
- Packet filtering: network (IP) | ip
- Circuit-level Gateway: session (transport)| hide private network information
- App-level Gateway: app layer | get, post
# 128
- Reflector Antenna: bossting a standard signal
- Yagi Antenna: point-to-point (between building)
- Dipole Antenna: standard routet "rabbit ears"
- Parabolic Grid Antenna: long range, narrow concentrated beam
# 132 Vulnerability Management
1. Discovery/Mapping
2. Asset Priorization and Allocation
3. Assessment/Scanning
4. Reporting - Technical and Executive
5. Remediation / Treating Risk: Mitigation, Remediation
6. Verification/Rescanning
# 137 Event Correlation
- Rule-Based: if-then
- Field-Based: compares specific field
- Graph-based: visualizing
- Automated Field: exhaustive