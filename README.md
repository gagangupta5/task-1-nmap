# task-1-nmap
#nmap: Used for network inventory, vulnerability scanning, network mapping, and troubleshooting network issues.

#For Host and Port Scanning
1.firstly scan nmap subnet with local ip to check which host is up or down (nmap -sn 192.168.1.0/24)
2.default scan to 1000 ports (nmap 192.168.1.10)
3.scan for all 65535 ports (nmap -p- 192.168.1.10)
4.scan for specific ports 80-http 443-https (nmap -p 80,192.168.1.10)

#For Service Scanning
5.scan which service/version running is the open ports(nmap -sV 192.168.1.10)

#For OS Detection
6.it scan which os is currently used and version of it (sudo nmap -O 192.168.1.10)

#Aggressive Scan Include OS, Version and Script Scanning
(nmap -A 192.168.1.10)

#Scan Types
7.-sS SCAN used for send syn packets to target (nmap -sS 192.168.1.10)
8.-sT uses full TCP connection 3-way handshake (nmap -sT 192.168.1.10) 9 -sU scans udp ports (nmap -sU 192.168.1.10)
9.-sA used to mapp firewall rules (nmap -sA 192.168.1.10)
10.-sN sends TCP packet with no flags set (nmap -sn 192.168.1.10)
-sS command is used to send the SYN packet to the target if the target is up and ready to connect it send SYN+ACK packet it means target is ready to connect, if it sends only SYN packet then it means target is down.
