# 1.Need & Advantage
- Network Traffic Monitoring: Retrospective security approach
- Anomaly > Signature
# 2.Setting up the Environment
- Cisco: Switched Port Analyzer (**SPAN**) (Port Mirroring), 3Com: Roving Analysis Port (**RAP**)
# 3.Baseline
- [content, context]-based, [single(atomic), multiple(composite)]-based
# 4.Suspicious
- FTP:over TCP:21
- TFTP: rogue TFTP:69, security breach
- UFTP: 1044, high-performance, unauthorized UFTP session
- ICMP probe
    - (icmp.type==8 && (!imcp.code==8)) // unusual ICMP code
    - (icmp.type==13) || (icmp.type==15) || (icmp.type==17) // TIMESTAMP(13), information request(15)
- TCP probe
    - tcp.flags==0x00 || 0x02 || 0x29 || 0x2b (Unskilled Attacker Pester Real System Folks)(URG, ACK | PSH, RST, SYN, FIN)
    - tcp.options.wscale_val==10
    - tcp.window_size < 1025
    - tcp.options.mss_val < 1460
- Ping Sweep
    - icmp.type==8 || icmp.tupe==0
    - tcp.dstport==7
    - udp.dstport==7
- UDP Scan
    - icmp.type==3 && icmp.code==3
- Password Cracking
    - ftp.response.cde==230
- NBNS(NetBIOS Name Service): legacy protocal:137
- Wireless 
    - Deauthentication: wlan.fc.type_subtype==12
    - Fake AP: wlan.fc.type_subtype==8
- (abnormal pattern)
    - port 
    - Ack < 0
    - Syn && not yet Ack && Len > 0
    - TCP broadcast
    - TCP Reserved Bits
# 5.Performance and Bandwith
TODO
- Network performance monitoring ((**NPM**)) (Bandwidth Monitoring): Data caching, Data Compression

- Flowmon, Awake Security Platform, Cisco Secure Network Analysis


- FTP:21, TFTP:69, UFTP:1044
- nmap [ping sweep, arp sweep, stealth scan -sS, full scan -sT, nulll scan, udp scan]