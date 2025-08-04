# Scanning-local-network:
Elevate labs cybersecurity internship: This repository contains the output, analysis, and screenshots for **Task 1** of the internship. The objective of this task was to perform a basic TCP SYN scan on my local network using **Nmap**, analyze the results, and identify potential security risks.

# Environment-Setup:
Host OS: Windows (Running VMware Workstation)
Virtual Machines:
1. Kali Linux (Scanner system)
2. Metasploitable 2 (Target 1)
3. Windows 7 (Target 2)
   
# Tools_Used:
Nmap
Linux terminal

# Execution:
I determined my IP address range using "ip a" command in Kali. This returned an IP with subnet range. Then I started the scan on the target subnet range and used a flag "-oN" to save the results in a text file.
command used : nmap -sS 192.168.000.000/24 -oN task1_results.txt
-sS : Performs a stealthy TCP SYN scan, which sends SYN packets to identify open ports.

Scan results are available in:
1. task1_results.txt
2. Task_1_Screenshots.docx

# Service-Research & Analysis:
3389 RDP Remote Desktop Protocol Credential reuse, BlueKeep vulnerability

This task helped me understand:
1. Basics of network scanning and reconnaissance
2. Interpreting Nmap results
3. Identifying vulnerabilities from open ports
