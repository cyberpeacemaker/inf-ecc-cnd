# 3, 98, 241
- push-based: syslog, SNMP
- pull-based : client-server, server catch through FTP from client
- Network-based
- host-based
# 6, 44, 91, 117, 121, 289, 58
- RAID 0: dara stripping
- RAID 1: mirror
- RAID 3: 1 parity drive | > 3
- RAID 5: distributed parity | 1 broken | > 3
- RAID 6: distributed parity | 2 broken
- RAID 10: > 4
- RAID 50: > 6 | high tolenrace + high speed
- SATA: hot plugging
# q11
- S/MIME: RSA
# 13, 54, 64, 89, 129, 146, 115, 178, 286 cmd
- Debian: `apt-get`
- Red Hat: `up2date > yum > dnf`
- Slackware: `Swaret`
- Autoupdate: `RPM`
- `up2date -d -f -u`: Redhat downlad, force, update
- `sudo netstat -tunlp: list all port`: Displays protocol statistics and current TCP/IP network connections.
- `sudo systemctl disable [service]`
- `sudo apt-get dist-upgrade`
- `update-rc.d -f [service name] remove`: Disable unwanted services
- `Get-WindowsOptionalFeature -Online -Feature smb1 protocol` (NO s)
# 14, 208
- SOX (Sarbanes-Oxkey Act if 2002): traded company, accountint firm
- **GLBA** (Gramm-Leach-Bliley Act): financial institution, privacy of customer
- FISMA (Federal Information Security Management Act): protect government info
- DMCA (Digital Millennium Copyright Act): Intellectual Property Law
- PCI DSS: payment card
# 19
- risk management [identification, assessment, treatment, monitor & review]
# 23, 87, 296
- Security Reference Monitor (**SRM**):  kernel-mode | Ntoskrnl.exe | check user/process has the rights to access
- WinLogon and NetLogon: login interface
- Security Account Manager(**SAM**): database file (registry hive) | store user account and group hashed password
- Local Security Ahtuority Subsystem(**LSASS**): user-mode process | brain of the authentication sub-system | policy, token, audit, log
- Local Administrator Password Solution (**LAPS**): store admin password in AD
# 24, 37, 108, 172, 279, 287 wireshark
- TCP Flag [consgestion, ecn-echom urgent, ack | push, rst, syn, fin]
- tcp.flags [000, 029, 02b]
- tcp.options.mss_val < 1460
- tcp.dstport/udp.dstport==7
# 27, 131, 243 UPS
- Standby-Ferro: legacy, unstable
- line Interactive: small business
- ture online: double conversion
- Double Conversion On-Line: 10kVA, convert AC to DC, mission-crtical DC, isolation
- Delta Conversion On-Line: modern double, efficiency, direct connectivity
# 34, 127
- AppLocker: Path Rule
# 41, 88, 160
- SAS (Serial Attached SCSI): connection type
- SAN (Storage Area Network): independent network connect servers to data storage device
- NAS (Network Attached Storage): lives on existing LAN
    - Integrated NAS: Head, Network Interface, Storage all bundled into a single 'appliance'
    - Gateway NSA: independent Head
    - FreeNAS: Software
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
# 51, 93, 104, 222
- Amazon EC2 (Elastic Compute Cloud): Iaas (Infrastructure as a Service)
- AWS CloudTrial: viewing account activity and events
- AWS Shared Reponsibility Model: [Container, Abstract, Infrastructure]
- AWS IAM identity: Inline Policy
# 55, 96, 159, 299
- IoE: Potential Risk Exposure
- IoA: Remote code Execution, Beaconing attempt
- IoC
- KRI (Key Risk Indicator): How risky an activity is | Risk Appetite | Notify, Identify, backward looking view
# 56, 290
- VPN Concentrator [Security Key, User Address, I/O Operation]
- VPN pipe Model: one customer edge to another | CE-to-CE
# 4, 35, 59, 110, 118, 156, 246, 253 BC/DR
- Risk Assesment: what could go wrong
- BIA: if goes wrong, how abd is it | examine [RTO: tolerable len, lost revenue | RPO:time frame, solution for DR/BC]
- BCP: final plan everyone follows
- Risk Assesment, Business Impact Analysis
- Data-centric
- BC/DR [Prevention, Response, Resumption, Recovery, Restoration]
# 65, 203
- Iris recognition: Front | Colored Ring
- Retianl Scanning: Back | Blood vessel
# 67, 164, 267, 276 Docker Container
- `--cpus="2"`
- Cgrounp(control group): CPU, memory, swap
- Seccomp (secure computing mode): block specific **syscall**
- docker daemon: manage docker image, container
# 71, 138, 175, 270, 120
- NIST: IoT, SDLC
- ISO 27005: risk management
- ISO 27007: Auditing Guidance
- ISO 27018: Cloud
- COBIT: Governance & Alignment | IT and Businiess
- WASC(Web Application Security Consortium): create, refine and promote internet safety standdards
# 76, 158 Azure
- MicroBurst: powersheel, vulnerability scan | how attacks happen
- Azure Key Vault: data at rest in Azure services
# 77, 113, 196, 231
- Risk = Asset + Threat + Vulnerability
- Attack = Motive(goal) + Method + Vulnerability
- risk factor = likelihood * impact 
# 79, 135, 163, 262 Wireless
- 802.11: IEEE standard
- 802.11b: DSSS (Direct-sequence Sprea Spectrum) | mutiplied with pseudo random noise
- 802.16: MAN (Metropolitan Are network)
# 82, 168
- WEP: RC4, 24bit, CRC
- WPA: TIKIP, 48bit, CRC, 4-way handshake
- WPA2: AES-CCMP, CBC-MAC (Cipher Block Chaining Message Authentication Code), 4-way handshake
- WPA3: IoT, AES-GCMP 256, ECDH and ECDSA
# 46, 83, 210, 247, 297 Virtualization Docker
- Para Virtualization (OS Assisted): it knows it is not running on physical hardware
- storage-level: storage pooling
- os-level: docker (container share host os)
- hardware-level: takes place in VMs | VMWare/hyper-v
- network-level: VLAN, VPN
# 86
- nwtowrk sniffing [Telnet Passwords, DNS traffic, Syslog Traffic]
# 90
- SSID cloaking
# 92, 150 security level
- extreme
- [low, mid, high, extreme]
# 101, 133, 145
- IoT Chip-level: JTAG
- TooL: SET
- Architecture layer [Device/Perception, Communication/Network, Platfform/Cloud (**Dashboard**), Application/Process]
# 40, 42, 102, 106
- ring: each comp acts as a repeater
- mesh: link to all device
- star: easy to expand
- Ad-Hoc: same channel name and SSID
# 103
- PGP: App Layer
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
- Class C (electrical appliance): Dry chemical
- Class K (烹飪油脂): Foam(Wet chemical)
# 119, 258 path 
- Apache: `/var/log/httpd`
- default pwd policy: `/etc/login.defs`
- `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\EventLog\<Event Log>`
# 122, 252
- content-based: payload
- context-based: Header (IP, protocol, cks)
- atomic-signature-based: simge packet
- composite-signature-based: multiple packet
# 124
- registry [Resplendent registrar, Reg.exe, Regedit.exe]
# 125, 141, 216, 220
- Packet filtering: network (IP) | ip
- Circuit-level Gateway: session (transport)| hide private network information
- App-level Gateway: app layer | get, post
# 128, 165m 259 Wireless, WiFI terminologies
- Reflector Antenna: bossting a standard signal
- Yagi Antenna: point-to-point (between building)
- Dipole Antenna: standard routet "rabbit ears"
- Parabolic Grid Antenna: long range, narrow concentrated beam
- antenna Directivity: particular direction
- DSSS(Direct-sequence Spread Spectrum): multiplies signal with noise
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
# 140, 161, 217, 242 IPSec
- Tunnel Mode: new IP header
- Transport Mode: payload
- AH(Authentication Header): IA
- ESP(Encapsulating Security Payload): IA + Confidentiality(Encryption)
# 142 Forensic Investigation Personnel
- Attorney: legal advice/consulanting
- Expert Witness: experienced testimony
# 147, 213
- Tripwire: linux file integrity
- Nessus
- AIDE
- Samgain
- OpenVAS: Vulnerability assessment, authenticated testing
# 149 IR Rolse and Responsibilities
- IR Custodian: remediation and resolution
# 157, 248 event type
- [Error(Loss of data/functionality), Warning, information(app load successfully), successful audit, failure audit]
# 179, 229
- internet contetn filter: block sites
- Network Protocal Analyzer: data lost leak | analyze packet
# 181 NIST
- Prepare
- Categorize: Defines criticality of information system according to potential worst-case
- Select: Applies tailoring quidance and supplemental controls as needed
- Implement: Set security control within an enterprise architecture
- Assess
- Authorize: Determine risk to organizational operations and assets
- Monitor
# 183, 199, 251 CA PKI
- CA (Certificate)
- RA (Registration): Verifier for the CA
- VA (Validation): for certification revocation state (CRL, OSCP)
# 186, 265 Information Security Policy
- EISP(Enterprise Infomation Security Policy): direction
- ISSP(Issue-Specific Security Policy): email, password, nwtwork usage, internet bandwidth comsumption
- SSSP(System-Specific Security Policy): AUP(Acceptable Use Policy)
# 188
- cloud to user: fake bill+
# 192 Cisco cmd
- `Router(Config-if) # IP route - cache flow`: Netflow
# 205
- Windows AD Authentication: PAM(Pluggable Authentication Module)
# 207, 307 analyze attack surface
- [visualize(understand), identify, simulate, reduce]
- visualize: [assets, topology, policies]
# 209 ICMP
- C?
# 212
- User Accecc Control: Company right
# 215
- masking: obscuring specific area
- retention
# 218
- IDS order [prevention, intrusion monitoring, intrusion detection, response]
# 225
- ipv4 mapped to ipv6, port 21
# 226 powershell 
- PS logging [Transcript: Session, Script block: code blcok, Module: pipeline execution]
- languagemode [Restricted, Constrained, Full]
- policy [restricted, allsigned, remotesigned, unrestricted]
# 255
- TACACS+ (Terminal Access Controller Access Control System Plus): encrypting including userpassword
# 260 RAM Type
- SRAM: 1-20ns
- DRAM/SDRAM: 50-150ns
- NAND Flash: slow
# 271 NFV (Network Function Virtualization) | VNF
- Virtualized Infrastructure Manager: computing, storage, network resource
# 285
- security policy hierarchy [laws, regulation, policy, standad and procedure]
# 309
- Kojoney: low interaction