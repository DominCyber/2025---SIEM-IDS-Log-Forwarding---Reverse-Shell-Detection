# 2025---SIEM-IDS-Log-Forwarding---Reverse-Shell-Detection
## Summary
This is a Splunk security information and event management (SIEM) and Snort intrusion detection system(IDS) log forwarding exercise. The setup is corroborated with Wireshark packet capturing. This is to test fundamental cybersecurity concepts/skills as well as application/tools, system, and network operability.

### Consdierations
<p>-I DO NOT CONDONE THE USE OF OFFENSIVE MEANS OR TOOLS OUTSIDE OF A TESTING ENVIRONMENT</p>
<p>-Overall, this baseline test is meant to be a standard for an ever refined test environment to practice concepts, familiarize various red and blue team tool usage, and apply GRC and other cybersecurity administrative concepts.</p>
<p>-The entire test is conducted within a closed VMware hypervisor environment, with three virtual machines; an attacker Kali Linux, a target Windows Server 2019, and a monitoring Windows 10.</p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Current network topography.</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Current Snort rules for 'local.rules' file.</i></p>
<p>-This test has inspiration and is an adaptation of the exercise explored in: My DFIR - Cybersecurity Tip: Build A Basic Home Lab (3/3) - https://www.youtube.com/watch?v=-8X7Ay4YCoA.</p>
<p>-Snort forwarding configuration guidelines were taken from Enhanced Logging and Intrusion Detection: Deploying Splunk, Sysmon and Snort - https://victorcoil.tech/?page_id=591.</p>
<p>-The Windows Server 2019 has been configured to have its firewall and real-time antivirus turned off to allow for malware proof-of-concept deployment.</p>
<p>-Wireshark is used on the Windows 10 machine is used to monitor the Eth0 virtual adapter for traffic to and from the attacking and targeting virtual machines.</p>

### Tools/Applications Used
#### VMware hypervisor on a Lenovo Thinkbook 16 G6
##### Virtual Machine OS
<p>-VMware hypervisor on a Lenovo Thinkbook 16 G6</p>
<p>--Virtual Machine OS</p>
<p>---Kali Linux</p>
<p>----Nmap CLI</p>
<p>----Metasploit CLI</p>
<p>----Python3 script</p>
<p>---Windows Server 2019 </p>
<p>---Windows 10</p>
<p>----(Splunk, Snort, Wireshark)</p>

### Concepts/Skills demonstrated 
#### Concepts

<p>-Concepts</p>
<p>--Hardware</p>
<p>---Networking architecture, ports, and protocols</p>

<p>-Policies, Principles, Procedures</p>
<p>--Open Worldwide Application Security Project (OWASP) Secure Design Principles</p>
<p>---Defense In-depth (Splunk, Snort, Wireshark)</p>
<p>--Cyber kill chain procedures</p>
<p>---Reconnaissance</p>
<p>---Weaponization</p>
<p>---Delivery</p>
<p>--Software</p>
<p>--Cybersecurity tools</p>
<p>---SIEM/SOC</p>
<p>---IDS</p>
<p>---Packet Sniffer</p>

#### Skills
##### Blue Team

##### Red Team

### Timeline
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 1:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 2:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 3:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 4:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 5:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 6:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 7:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 8:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 9:</i></p>
<img src=" " style="width: 50%;" alt="1">
<p><i>Ref 10:</i></p>

