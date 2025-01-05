# 2025---SIEM-IDS-Log-Forwarding---Reverse-Shell-Detection
## Summary
This is a Splunk security information and event management (SIEM) and Snort intrusion detection system(IDS) log forwarding exercise. The setup is corroborated with Wireshark packet capturing. This is to test fundamental cybersecurity concepts/skills as well as application/tools, system, and network operability.

### Consdierations
<p>-I DO NOT CONDONE THE USE OF OFFENSIVE MEANS OR TOOLS OUTSIDE OF A TESTING ENVIRONMENT</p>
<p>-Overall, this baseline test is meant to be a standard for an ever refined test environment to practice concepts, familiarize various red and blue team tool usage, and apply GRC and other cybersecurity administrative concepts.</p>
<p>-The entire test is conducted within a closed VMware hypervisor environment, with three virtual machines; an attacker Kali Linux, a target Windows Server 2019, and a monitoring Windows 10.</p>
<img src="https://i.imgur.com/OqkHqgK.png" style="width: 75%;" alt="1">
<p><i>Current network topography.</i></p>
<img src="https://i.imgur.com/ngeTrRA.png" style="width: 75%;" alt="1">
<p><i>Current Snort rules for 'local.rules' file.</i></p>
<p>-This test has inspiration and is an adaptation of the exercise explored in: My DFIR - Cybersecurity Tip: Build A Basic Home Lab (3/3) - https://www.youtube.com/watch?v=-8X7Ay4YCoA.</p>
<p>-Snort forwarding configuration guidelines were taken from Enhanced Logging and Intrusion Detection: Deploying Splunk, Sysmon and Snort - https://victorcoil.tech/?page_id=591.</p>
<p>-The Windows Server 2019 has been configured to have its firewall and real-time antivirus turned off to allow for malware proof-of-concept deployment.</p>
<p>-Wireshark is used on the Windows 10 machine is used to monitor the Eth0 virtual adapter for traffic to and from the attacking and targeting virtual machines.</p>

### Tools/Applications Used
#### VMware hypervisor on a Lenovo Thinkbook 16 G6
##### Virtual Machine OS and installed tool/applications
<p>-Kali Linux</p>
<p>--Nmap CLI</p>
<p>--Metasploit CLI</p>
<p>--Python3 script (for HTTP listening session)</p>
<p>-Windows Server 2019</p>
<p>-Windows 10</p>
<p>--(Splunk, Snort, Wireshark)</p>

### Concepts/Skills demonstrated 
#### Concepts
##### Hardware
<p>-Networking architecture, ports, and protocols</p>

##### Policies, Principles, Procedures
<p>-Open Worldwide Application Security Project (OWASP) Secure Design Principles</p>
<p>--Defense In-depth (Splunk, Snort, Wireshark)</p>

##### Techniques
<p>-Cyber kill chain procedures</p>
<p>--Reconnaissance</p>
<p>--Weaponization</p>
<p>--Delivery</p>

##### Software</p>
<p>-Cybersecurity tools</p>
<p>--SIEM/SOC</p>
<p>--IDS</p>
<p>--Packet Sniffer</p>

#### Skills
##### Blue Team
<p>-Cybersecurity tools install, configuration, integration, and log forwarding</p>
<p>-Reconnaissance Detection - Snort IDS, Wireshark packet sniffer</p>
<p>-Weaponization Detection and Analysis- Snort IDS, Wireshark packet sniffer</p>
<p>-Log Aggregation - Splunk SIEM, Snort IDS, Wireshark packet sniffer</p>
<p>-Log Consolidation - Splunk SIEM, Snort IDS</p>

##### Red Team
<p>-Reconnaissance - enumerating target VM's ports</p>
<p>-Weaponization - Metasploit reverse shell payload creation</p>
<p>-Weaponization - Metasploit console configuration and execution</p>
<p>-Delivery - via web application</p>


### Timeline
<img src="https://i.imgur.com/43uiYv2.png" style="width: 75%;" alt="1">
<p><i>Ref 1:Snort captures of ICMP ping captures from attacking virtual machine.</i></p>
<img src="https://i.imgur.com/j9ZnABV.png" style="width: 100%;" alt="1">
<p><i>Ref 2:Splunk forwarded logs from Snort captures of ICMP  of a triggered port scan alert</i></p>
<img src="https://i.imgur.com/0TvbqDC.png" style="width: 100%;" alt="1">
<p><i>Ref 3:Splunk forwarded logs from Snort captures of ICMP ping captures.</i></p>
<img src="https://i.imgur.com/3eNwsvV.png" style="width: 100%;" alt="1">
<p><i>Ref 4:Splunk forwarded logs from Snort captures of a triggered port scan alert.</i></p>
<img src="https://i.imgur.com/EIJ7mO3.png" style="width: 100%;" alt="1">
<p><i>Ref 5:Nmap port scan results - Snort port scanning alert - captured scanning of ports 135 and 445.</i></p>
<img src="https://i.imgur.com/z43zNOJ.png" style="width: 100%;" alt="1">
<p><i>Ref 6:Snort capture of sustained reverse shell connection from attacking to target virtual machines.</i></p>
<img src="https://i.imgur.com/6ZL1L4S.png" style="width: 100%;" alt="1">
<p><i>Ref 7:Wireshark capture of target virtual machine file execution via HTTP GET flag.</i></p>
<img src="https://i.imgur.com/4hu44lJ.png" style="width: 100%;" alt="1">
<p><i>Ref 8:Wireshark capture of attacking virtual machine server and script information.</i </p>
<img src="https://i.imgur.com/tAb1STU.png" style="width: 100%;" alt="1">
<p><i>Ref 9:Wireshark capture of attacking virtual machine reverse shell script initiating and maintaining connection.</i></p>
<img src="https://i.imgur.com/tAb1STU.png" style="width: 100%;" alt="1">
<p><i>Ref 10:Splunk forwarded logs from Snort capture of Metasploit port 4444, indicating corroborating reverse shell execution.</i></p>

