# Scanning-local-network:
Elevate labs cybersecurity internship: This repository contains the output, analysis, and screenshots for **Task 1** of the internship. The objective of this task was to perform a basic TCP SYN scan on my local network using **Nmap**, analyze the results, and identify potential security risks.

# Environment-Setup:
Host OS: Windows (Running VMware Workstation)
Virtual Machines:
1. Kali Linux (Scanner system)
2. Metasploitable 2 (Target 1)
3. Windows 7 (Target 2)
   
# Tools_Used:
1. Nmap
2. Linux terminal

# Execution:
I determined my IP address range using "ip a" command in Kali. This returned an IP with subnet range. Then I started the scan on the target subnet range.
command used : "nmap -sS 192.168.X.X/24 -oN task1_results.txt"
-sS : Performs a stealthy TCP SYN scan, which sends SYN packets to identify open ports.
-oN : To save the nmap scan results in a text file

Scan results are available in:
1. task1_results.txt
2. Task_1_SS.png

I have redact/modified the IP and MAC information in the results for security purpose.

# Service-Research & Analysis:
1. Port 3389 is open on the windows 7 - RDP (Remote Desktop Protocol) We can brute force the login or use "BlueKeep" vulnerability
to get access to the the target.
2. Port 3306 is open which runs a mysql server - we can try multiple techniques to exploit mysql server.

# This task helped me understand:
1. Basics of network scanning and reconnaissance
2. Interpreting Nmap results
3. Identifying vulnerabilities from open ports
