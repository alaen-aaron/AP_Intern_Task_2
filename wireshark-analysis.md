# Wireshark Packet Analysis

## Objective
Analyze network traffic and identify insecure protocols.

## FTP Credential Capture

Protocol: FTP

Observation:
FTP transmits credentials in plaintext.

Captured credentials:

Username: msfadmin  
Password: msfadmin

This demonstrates how attackers can intercept sensitive data when encryption is not used.

## HTTP Traffic Analysis

HTTP requests were captured while accessing the Metasploitable web server.

Observation:
Data is transmitted in plaintext and can be analyzed easily.

## SYN Flood Observation

Tool used: hping3

Command:

sudo hping3 -S 192.168.56.104 -p 80 --flood

Result:
Large number of SYN packets observed in Wireshark, indicating potential denial-of-service attack behavior.
