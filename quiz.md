# 3, 98, 241
- push-based: syslog, SNMP
- pull-based : client-server, server catch through FTP from client
- Network-based
- host-based
# 4, 19 Risk Management Phase
1. Risk Identification: Establishing context, quantifying risk
2. Risk Assessment: likelihood * impact | exposure of risk | quantitative and qualitative
3. Risk Treament: [eliminate, transfer, mitigate, accept, avoidance]
4. Risk Tracking & Review
# 35, 59, 110, 118, 156, 246, 253 BC/DR
- BIA (Business Impact Analysis): examine [RTO: tolerable len, lost revenue | RPO:time frame, solution for DR/BC]
- BCP (Business Continueous Plan): final plan everyone follows
- Data-centric
- BC/DR [Prevention, Response, Resumption, Recovery, Restoration]
# 6, 44, 91, 117, 121, 289, 58
- RAID 0: dara stripping | > 2
- RAID 1: mirror | > 2
- RAID 3: 1 parity drive | > 3
- RAID 5: distributed parity | 1 broken | > 3
- RAID 6: distributed parity | 2 broken | > 4
- RAID 10: > 4 | high cost
- RAID 50: > 6 | high tolenrace + high speed | high tech
- SATA: hot plugging
# 11
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
- `update-rc.d -f [service name] remove`: Disable unwanted services (run command | init)
- `Get-WindowsOptionalFeature -Online -Feature smb1 protocol` (NO s)
# 14, 208
- PCI-DSS (Payment Card Industry Data Security Standard): credit card
- HIPAA (Health Insurance Portability and Accountability Act): health
- GDPR (General Data Protection Regulation): European personal privacy
- **GLBA** (Gramm-Leach-Bliley Act): financial institution, privacy of customer
- SOX (Sarbanes-Oxkey Act in 2002): financial reporting, accounting fraud
- DMCA (Digital Millennium Copyright Act): Intellectual Property Law
- FISMA (Federal Information Security Management Act): protect government info
# 23, 87, 296
- Security Reference Monitor (**SRM**):  kernel-mode | Ntoskrnl.exe | check user/process has the rights to access
- WinLogon and NetLogon: login interface
- Local Security Ahtuority Subsystem(**LSASS**): user-mode process | brain of the authentication sub-system | policy, token, audit, log
- Security Account Manager(**SAM**): database file (registry hive) | store user account and group hashed password
- Local Administrator Password Solution (**LAPS**): store admin password in AD
# 24, 37, 108, 172, 279, 287 wireshark
- TCP Flag [urgent, ack | push, rst, syn, fin] (Unskilled Attackers Pester Real System Folks)
- tcp.flags [000, 029, 02b]
- tcp.options.mss_val < 1460
- tcp.options.wscale_val==10
- tcp.dstport/udp.dstport==7
# 27, 131, 243 UPS
- Standby-Ferro: legacy, unstable
- line Interactive: small business
- true online / Double Conversion On-Line: 10kVA, AC to DC to AC, mission-crtical DC, completely isolation (airgp)
- Delta Conversion On-Line: modern double, efficiency, direct connectivity, partial/hybrid isolation
# 34, 127
- AppLocker: Path Rule
# 41, 88, 160
- DAS (Direct Attached Storage): external hard drive
- SAS (Serial Attached SCSI): physical connection, cable
- SAN (Storage Area Network): high-speed, dedicated network for storage, looks like a local hard drive (Block-level storage)
- NAS (Network Attached Storage): lives on existing LAN, looks like a shared folder (File-level storage)
    - Integrated NAS: Head, Network Interface, Storage all bundled into a single 'appliance'
    - Gateway NSA: independent Head / Storage
    - FreeNAS: Software-defined OS
# 45, 136 incident response / triage
- analysis, classification
- prioritization, notification
- containment, evidence gathering
- eradication, recovery
# 46, 83, 210, 247, 297 Virtualization Docker
- hardware-level: slow, takes place in VMs | VMWare/hyper-v | hypervisor | Guest OS
- Para Virtualization (OS Assisted): Guest OS knows it is not running on physical hardware | Xen
- os-level: fast, docker, No Guest OS, all container share host OS
- storage-level: storage pooling
- network-level: VLAN, VPN, SDN
# 50 SNMP
- TRAPS:PUSH for Help
- INFORM PUSH | SNMPv2c | Need manager send back confirm
- RESPONSE: agent back to manager
- SET: managet to agent
# 51, 93, 104, 222
- Amazon EC2 (Elastic Compute Cloud): Iaas (Infrastructure as a Service)
- AWS CloudTrial: viewing account activity and events | record API call
- AWS Shared Reponsibility Model: 
    - Infrastructure (EC2) : OS, patching, firewall, IAM, data
    - Container: firewall, IAM, data
    - Abstract: data
- AWS IAM identity: Inline Policy (1-to-1 relationship) | customer/AWS-managed are standalone
# 55, 96, 159, 299
- IoE: Potential Risk Exposure, missconfigured S3 bucket
- IoA: Remote code Execution, Beaconing attempt
- IoC: hash, ip, domain
- KRI (Key Risk Indicator): business metric used to predict the likelihood of an event that would exceed the organization's risk appetite. (ex: Percentage of staff who haven't completed security training.) | How risky an activity is | Risk Appetite | Notify, Identify, backward looking view 
# 56, 290
- VPN Concentrator: handle high volume of VPN tunnels
    - Manage Security Key: ISAKMP/IKE, keys are rotated and managed securely
    - Assign User Address: assign vitual internal IP for client
    - Enable I/O Operation: flow traffic, data transfer
- VPN QoS Model
    - Uniform: copies original priority to tunnel header | Trust carrier to manage and update your priority
    - Pipe: one customer edge to another | CE-to-CE | ensure client order
    - Short-Pipe: | Customer wants to control the final exit priority
    - hose-model: softer than pipe
# 65, 203
- Iris recognition: Front | Colored Ring
- Retianl Scanning: Back | Blood vessel
# 67, 164, 267, 276 Docker Container
- `--cpus="2"`: limit the hardware resource
- Cgrounp(control group): CPU, memory, swap | limit/account/isolate resource usage
- Seccomp (secure computing mode): block specific **syscall** | firewall for the kernel
- docker daemon: manage docker image, container
# 71, 120, 138, 175, 270
- NIST: IoT, SDLC | CSF (Cybersecurity Framework)
- ISO 27001: Requirement
- ISO 27002: The Controls
- ISO 27005: risk management
- ISO 27007: Auditing Guidance
- ISO 27018: Cloud
- COBIT: Governance & Alignment | IT and Businiess
- WASC(Web Application Security Consortium): create, refine and promote internet safety standdards
# 75, 257 Defense-in-Depth
- policy, procedure, awareness: BYOD
- physical: CCTV
- preimeter: router, firewall, dns server
- internal network: switch
- host: os, patch, antivirus, logging
- application: ACL, black/white listing
- data:
# 76, 158 Azure
- MicroBurst: powershell, vulnerability scan | how attacks happen
- Azure Key Vault: data at rest in Azure services
# 77, 113, 196, 231
- Risk = Asset + Threat + Vulnerability
- Attack = Motive(goal) + Method + Vulnerability
- risk factor = likelihood * impact | threat * vulnerability * consequence
# 79, 135, 163, 262 Wireless
- 802.11: IEEE standard
- 802.11b: DSSS (Direct-sequence Sprea Spectrum) | mutiplied with pseudo random noise
- 802.16: MAN (Metropolitan Are network)
# 82, 168, 193
- WEP: RC4, 24bit, CRC
- WPA: RC4/TKIP, 48bit, CRC, 4-way handshake
- WPA2: AES-CCMP, 4-way handshake, CBC-MAC (Cipher Block Chaining Message Authentication Code)
- WPA3: AES-GCMP 256, ECDH and ECDSA, BIP-GMAP-256 | IoT
# 86
- nwtowrk sniffing [Telnet Passwords, DNS traffic, Syslog Traffic]
# 90
- SSID cloaking
# 92, 150 security level
- extreme
- [low, mid, high, extreme]
# 101, 133, 145
- IoT Chip-level: JTAG
- Tool: SET
- Architecture layer [Device/Perception, Communication/Network, Platfform/Cloud (**Dashboard**), Application/Process]
# 12, 40, 42, 102, 106
- hub-and-spoke: main office connect to it's branch office
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
# 128, 165, 259 Wireless, WiFI terminologies
- Reflector Antenna: bossting a standard signal
- Yagi Antenna: point-to-point (between building)
- Dipole Antenna: standard routet "rabbit ears"
- Parabolic Grid Antenna: long range, narrow concentrated beam
- antenna Directivity: particular direction
- DSSS(Direct-sequence Spread Spectrum): multiplies signal with noise
- SSID(Service Set Identifieer): name
- OFDM(orthogonal frequency-division multiplexing): multi-carrier modulation method
- EAP(Extensible Authentication Protocal): framework allow different authentication methods
- LEAP(lightweight Authentication Protocal): Cisco
- TKIP(Temporal Key Integrity Protocal): used by WPA to replace WEP RC4
# 132, 152, 190, 238, 294 Vulnerability assessment plan/Management
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
- Tripwire: linux FIM (file integrity monitoring)
- AIDE: FIM
- Samgain: FIM
- Nessus: Vulnerability scanner/assessment
- OpenVAS (Greenbone): Vulnerability scanner/assessment, authenticated testing
- Burp suite: web pentesting
# 149 IR Rolse and Responsibilities
- IR Custodian: remediation and resolution
# 157, 248 event type
- [Error(Loss of data/functionality), Warning, information(app load successfully), successful audit, failure audit]
# 179, 229
- internet contetn filter: block sites
- Network Protocal Analyzer (packet analyzer): data lost leak | analyze packet
# 181 NIST
- Prepare
- Categorize: Defines criticality of information system according to potential worst-case
- Select: Applies tailoring quidance and supplemental controls as needed
- Implement: Set security control within an enterprise architecture
- Assess
- Authorize: Determine risk to organizational operations and assets
- Monitor
# 183, 199, 251 CA PKI
- CA (Certificate): issue cert | verify CA
- RA (Registration): Receptionist of CA | verify the identiy/entity requesting cert
- VA (Validation): for certification revocation state (CRL, OSCP)
# 186, 265 Information Security Policy
- EISP(Enterprise Infomation Security Policy): direction
- ISSP(Issue-Specific Security Policy): email, password, nwtwork usage, internet bandwidth comsumption, Acceptable usage policy
- SSSP(System-Specific Security Policy): firewall configuration, database access list, encryption, 
# 188
- cloud to user: fake bill+
# 192 Cisco cmd
- `Router(Config-if) # IP route - cache flow`: Netflow
# 205
- Windows AD Authentication: PAM(Pluggable Authentication Module)
# 207, 307 analyze attack surface
- [visualize(understand), identify IoE, simulate, reduce]
- visualize: [assets, topology, policies]
# 209 ICMP
- C? icmp.type==14/15/17
# 212
- User Accecc Control policy: monitor the activities of employee
# 215
- masking: obscuring specific area
- retention: lifecycle
# 218
- IDS order [prevention, intrusion monitoring, intrusion detection, response]
# 225
- ipv4 mapped to ipv6, port 21
# 226, 240 powershell 
- PS logging [Transcript: text-based (user input and terminal output) (autditing), Module: pipeline execution (variable and command invocation)], Script block: code blcok (actual code being run) (de-obfuscation)
- policy [restricted, allsigned, remotesigned, unrestricted]
- languagemode [Restricted, Constrained, Full]
# 255
- TACACS+ (Terminal Access Controller Access Control System Plus): encrypting whole communication 
# 260 RAM Type
- SRAM: 1-20ns
- DRAM/SDRAM: 50-150ns
- NAND Flash: slow
# 271 NFV (Network Function Virtualization) | VNF
- Orchestrator(NFVO): global coordination of services
- VNF Manager: Managing the Lifecycle of app
- VIM(Virtualized Infrastructure Manager): computing, storage, network resource
- NFVI: the actual physical hardware/hypervisor
# 285
- security policy hierarchy [laws, regulation, policy, standad and procedure]
# 309
- Kojoney: low interaction