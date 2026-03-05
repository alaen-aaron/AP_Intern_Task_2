# Network Scan Report

## Target System
Metasploitable2

IP Address: 192.168.56.104

## Network Discovery

Command used:

nmap -sn 192.168.56.0/24

Result:
The scan discovered active hosts in the network including the Metasploitable target machine.

## Port Scanning

Command used:

nmap -sV 192.168.56.104

### Open Ports Detected

| Port | Service | Version |
|-----|------|------|
| 21 | FTP | vsftpd |
| 22 | SSH | OpenSSH |
| 23 | Telnet | Linux Telnet |
| 80 | HTTP | Apache |
| 3306 | MySQL | MySQL Server |

## Vulnerability Scan

Scanner Used: Nessus Essentials

Summary:

Critical: 0  
High: Several vulnerabilities detected  
Medium: Multiple outdated service warnings  
Low: Information disclosure issues  

Example vulnerability:

Outdated Apache HTTP Server

Description:
The target system is running an outdated Apache version which may contain known vulnerabilities.

Mitigation:
Update Apache to the latest version and apply security patches.

## Impact

Outdated services can allow attackers to exploit known vulnerabilities and gain unauthorized access to the system.

## Recommendation

- Update outdated software
- Disable unused services
- Use secure authentication methods
- Apply regular security patches
