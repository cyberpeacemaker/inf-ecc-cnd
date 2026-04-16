# q11
- S/MIME: RSA
# 13
- sudo netstat -tunlp: list all port. | Displays protocol statistics and current TCP/IP network connections.
# 14, 208
- SOX (Sarbanes-Oxkey Act if 2002): traded company, accountint firm
- GLBA (Gramm-Leach-Bliley Act): financial institution
- FISMA (Federal Information Security Management Act): protect government info
- DMCA (Digital Millennium Copyright Act): Intellectual Property Law
- PCI DSS: payment card
# 16
- SYN scan (-sS)
- NULL, XMAX (-sN, -sX)
- ACK (-sA)
# 18
- DDoS [App/Netwrok]-centric
# 23, 87, 296
- Security Reference Monitor (**SRM**):  kernel-mode | Ntoskrnl.exe | check user/process has the rights to access
- WinLogon and NetLogon: login interface
- Security Account Manager(**SAM**): database file (registry hive) | store user account and group hashed password
- Local Security Ahtuority Subsystem(**:LSASS**): user-mode process | brain of the authentication sub-system | policy, token, audit, log
# 24, 37, 108, 178, 279, 287 wireshark
- TCP Flag [ack, push, rst, syn, fin]
- tcp.flags [000, 029, 02b]
- tcp.options.wscale_val==20
- tcp.dstport/udp.dstport==7
# 27, 131, 243 UPS
- Standby-Ferro: legacy, home
- line Interactive: small business
- ture online: double conversion
- Double Conversion On-Line: isolation, 10kVA, convert AC to DC, mission-crtical DC
- Delta Conversion On-Line: modern double, Large DC
# 34, 127
- AppLocker: Path Rule
# 41
- Integrated NAS: Head, Network Interface, Storage all bundled into a single 'appliance'
- Gateway NSA: independent Head
- FreeNAS: Software
# 44, 91, 117, 121, 289
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
# 54 
- REDHAT up2date -d -f -u
# 55, 96, 159, 299
- IoE
- IoA: Remote code Execution, Beaconing attempt
- IoC
- KRI (Key Risk Indicator): Notify, Identify, backward looking view
# 56
- VPN Concentrator [Security Key, User Address, I/O Operation]
# 58
- SATA: hot plugging
# 59, 110, 118, 156 , 246, 253 BC/DR
- risk Assesment: what could go wrong
- BIA: if goes wrong, how abd is it
- RTO: tolerable len, lost revenue | time frame, solution for DR/BC
- Disaster Recovery Strategy: How do we meet (RTO/RPO)
- BCP: final plan everyone follows
- Risk Assesment, Business Impact Analysis
- Data-centric
- BC/DR [Prevention, Response, Resumption, Recovery, Restoration]
# 64, 115
- `Get-WindowsOptionalFeature -Online -Feature smb1 protocol` (NO s)
# 65, 203
- Iris recognition: Front | Colored Ring
- Retianl Scanning: Back | Blood vessel
# 67
- `--cpus="2"`
# 71, 138, 175, 270
- NIST: IoT, SDLC
- ISO 27005: risk management
- ISO 27007: Auditing Guidance
- ISO 27018: Cloud
- COBIT: Governance & Alignment | IT and Businiess
# 76, 158
- Azure: MicroBurst | Cloud
- Azure Key Vault: data at rest in Azure services
# 77, 113, 196, 231
- Risk = Asset + Threat + Vulnerability
- Attack = Motive(goal) + Method + Vulnerability
- risk factor = likelihood * impact 
# 79, 135, 163, 262 Wireless
- 802.11: IEEE standard
- 802.11b
- 802.16: MAM
# 82, 168
- WEP
- WPA
- WPA2: CCMP, CBC-MAC
- WPA3: IoT
# 83
- Para Virtualization (OS Assisted): it knows it is not running on physical hardware
# 86
- nwtowrk sniffing [Telnet Passwords, DNS traffic, Syslog Traffic]
# 88, 160
- SAS (Serial Attached SCSI): connection type
- SAN (Storage Area Network): independent network connect servers to data storage device
- NAS (Network Attached Storage): lives on existing LAN
# 89, 129, 146
- Debian: apt-get
- Red Hat: up2date > yum > dnf
- Slackware: Swaret
- AutoupdateL RPM
# 90
- SSID cloaking
# 92
- extreme
# 51, 93, 222
- Amazon EC2 (Elastic Compute Cloud): Iaas (Infrastructure as a Service)
- AWS CloudTrial
- AWS IAM identity: Inline Policy
# 98, 241
- push-based: syslog, SNMP
- pull-based : FTP
- Network-based
- host-based
# 101, 133, 145
- IoT Chip-level: JTAG
- TooL: SET
- Architecture layer [Device/Perception, Communication/Network, Platfform/Cloud (**Dashboard**), Application/Process]
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
# 105, 107, 174, 277
- Network access policy [Promiscuous, Permissive, Prudent, Paranoid]
# 109
Authorization
- centralized: RADIUS
- decentralized
- implicit: assumed
- explicit: clearly stated
# 111, 206, 234, 261
- Win: BitLocker, Device Encryption, EFS(encryptied File System) (only on NTFS)
- Mac: FileVault
- Linux: dm-crypt
# 114, 280 fire suppress
- Class A: (water)
- Class B: Carbon dioxide
- Dry chemical
- Class K: Foam(Wet chemical)
# 119, 258 path 
- Apache: /var/log/httpd
- default pwd policy: /etc/login.defs
- HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\EventLog\<Event Log>
# 120
- WASC(Web Application Security Consortium): create, refine and promote internet safety standdards
# 122, 252
- content-basedL payload
- context-based: Header (IP, protocol, cks)
- atomic-signature-based: simge packet
- composite-signature-based: multiple packet
# 124
- registry [Resplendent registrar, Reg.exe, Regedit.exe]
# 125, 141, 216, 220
- Packet filtering: network (IP) | ip
- Circuit-level Gateway: session (transport)| hide private network information
- App-level Gateway: app layer | get, post
# 128
- Reflector Antenna: bossting a standard signal
- Yagi Antenna: point-to-point (between building)
- Dipole Antenna: standard routet "rabbit ears"
- Parabolic Grid Antenna: long range, narrow concentrated beam
# 132, 152, 190, 238, 294 Vulnerability Management
1. Discovery/Mapping: acquisition of required docs, reviewing of sec policies and comppliance
2. Asset Priorization and Allocation
3. Assessment/Scanning | adhere to the risk analysis
4. Reporting - Technical and Executive
5. Remediation / Treating Risk: Mitigation, Remediation
6. Verification/Rescanning
# 137, 195 Event Correlation
- Rule-Based: if-then
- Field-Based: compares specific field
- Graph-based: visualizing
- Automated Field: exhaustive algo, systematically and intentionally
# 140, 161, 217, 242, 290 IPSec
- Tunnel Mode: new IP header
- Transport Mode: payload
- AH(Authentication Header): IA
- ESP(Encapsulating Security Payload): IA + Confidentiality(Encryption)
- VPN pipe Model: one customer edge to another
# 142 Forensic Investigation Personnel
- Attorney: legal advice/consulanting
- Expert Witness: experienced testimony
# 14, 213
- Tripwire: linux file integrity
- Nessus
- AIDE
- Samgain
- OpenVAS: Vulnerability assessment, authenticated testing
# 149 IR Rolse and Responsibilities
- IR Custodian: remediation and resolution
# 150 security level
- [low, mid, high, extreme]
# 157, 248 event type
- [Error(Loss of data/functionality), Warning, information(app load successfully), successful audit, failure audit]
# 164, 267, 276 Docker Container
- Cgrounp(control group): CPU, memory, swap
- Seccomp (secure computing mode): block specific syscall
- docker daemon: manage docker image, container
# 165 antenna characteristic
- directivity
# 178, 286 Linux cmd
- `sudo systemctl disable [service]`
- `update-rc.d -f [service name] remove`
# 179
- internet contetn filter: block sites
# 181 NIST
- Prepare
- Categorize
- Select
- Implement
- Assess
- Authorize
- Monitor
# 183, 199, 251 CA PKI
- CA (Certificate)
- RA (Registration): Verifier for the CA
- VA (Validation): for certification revocation state (CRL, OSCP)
# 186, 265 Information Security Policy
- EISP(Enterprise Infomation Security Policy): tpo
- ISSP(Issue-Specific Security Policy): email, password, nwtwork usage, internet bandwidth comsumption
- SSSP(System-Specific Security Policy): AUP(Acceptable Use Policy)
# 188
- cloud to user: fake bill+
# 192 Cisco cmd
- `Router(Config-if) # IP route - cache flow`: Netflow
# 205
- Windows Authentication: PAM(Pluggable Authentication Module)
# 207, 307 analyze attack surface
- [visualize(understand), identify, simulate, reduce]
- visualize: [assets, topology, policies]
# 209 ICMP
- C?
# 210, 247, 297 Virtualization Docker
- storage-level: storage pooling
- os-level: docker (container share host os)
- hardware-level: VMWare/hyper-v
- network-level: VLAN, VPN
# 212
- User Accecc Control: Company right
# 215
- masking: obscuring specific area
- retention
# 218
- IDS order [prevention, intrusion monitoring, intrusion detection, response]
# 225
- ipv4 mapped to ipv6
# 226 powershell 
- module logging: pipeline execution
- policy [restricted, allsigned, remotesigned, unrestricted]
# 229
- Network Protocal Analyzer: data lost leak
# 255
- TACACS (Terminal Access Controller Access Control System Plus)
# 259 wireless terminologies
- DSSS(Direct-sequence Spread Spectrum): multiplies signal with noise
# 260 RAM Type
- SRAM: 1-20ns
- DRAM/SDRAM: 50-150ns
- NAND Flash: slow
# 271 VNF
- Virtualized Infrastructure Manager: computing, storage, network resource
# 285
- security policy hierarchy [laws, regulation, policy, standad and procedure]