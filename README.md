# Penetration Testing a pfSense Firewall

## Objective

The purpose of this lab was to perform hands-on penetration testing against a pfSense firewall and observe how firewall rule configurations affect vulnerability exposure. Students practiced scanning, analyzing, and securing network environments using a pfSense system and vulnerability scanning tools. This exercise reinforces foundational knowledge of firewall management, network defense, and security hardening techniques.

### Skills Learned

- Understanding firewall configurations and rule management using pfSense.

- Performing network scans and interpreting vulnerability reports.

- Identifying open ports and exposed services using Nmap and traceroute.

- Running vulnerability scans with OpenVAS and analyzing detailed scan results.

- Hardening firewall security by modifying and applying new rule sets.

- Applying best practices for DMZ deployment and isolation techniques.

### Tools Used

-pfSense Firewall – used to inspect, modify, and test firewall rules.

- Kali Linux – used to conduct penetration testing activities.

- Greenbone/OpenVAS – for advanced vulnerability scanning and reporting.

- Nmap – to perform OS detection and identify open services.

- Traceroute & Ping – for basic network reconnaissance and routing paths.

- Windows Server VM – targeted system used for testing rule effectiveness.

## Steps
Ref 1: WAN Rules Table
Screenshot showing the WAN rules in pfSense, used to examine allowed traffic into the network.
![image](https://github.com/user-attachments/assets/3d33df1c-6db1-4f83-9f4e-bab0ce3d4258)


Ref 2: Initial Penetration Test Results
Screenshot of scan results showing vulnerabilities identified before modifying any firewall rules.
![image](https://github.com/user-attachments/assets/c1c8062c-b174-46dc-88e8-fa2a4d844d76)


Ref 3: Vulnerability List
Detailed output from the initial scan showing specific vulnerabilities found in the system.
![image](https://github.com/user-attachments/assets/8a2b9484-c122-4d50-956c-4a7ca00e599c)


Ref 4: Updated Firewall Rules + New Scan Summary
Screenshot showing updated pfSense rules (deleting “Default allow LAN to any,” etc.) and a new vulnerability scan report confirming the firewall successfully blocked previous exposures.
![image](https://github.com/user-attachments/assets/dd8384c1-b22f-4ca1-a86c-4a63cc966acc)


Ref 5: Traceroute Results
Output from traceroute 172.40.0.20 showing the path between Kali and the remote server.
![image](https://github.com/user-attachments/assets/43d08e7b-515c-40ce-aad8-f24ac7fbd838)


Ref 6: Nmap OS Detection Scan
Result of running nmap -sV -O 202.20.1.3, identifying open services and estimating OS.
![image](https://github.com/user-attachments/assets/695f42c2-7db7-4f3c-bd53-833ca6ce4e9b)


Ref 7: OpenVAS Scan Report
Screenshot of the completed OpenVAS scan, showing summary of vulnerabilities detected.
![image](https://github.com/user-attachments/assets/508643e6-b9d0-4626-a6f4-56d6b182d575)


Ref 8: Detailed OpenVAS Report
Screenshot of the expanded vulnerability report from OpenVAS, showing severity levels and affected services.
![image](https://github.com/user-attachments/assets/44950568-3ef7-462d-b27c-be7e735e7d78)
