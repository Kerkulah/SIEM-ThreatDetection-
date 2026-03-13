
<h2>Description</h2>
A functional home lab with a SIEM at the center. Collect logs from multiple sources, write detection rules for common attack techniques (from the MITRE ATT&CK framework), and build a visual dashboard that tells the story of what happened on my network.
<br />
<h2> Phase 1 Setup </h2>
<br />

- I installed three VMs on my Proxmox server: one running Ubuntu Server, one Windows 10, and one Kali Linux.
- On the Ubuntu Server VM, install Splunk Free.
- Install Sysmon on the Windows 10 VM using the SwiftOnSecurity config; this dramatically improves Windows log quality.
<br />

<br />
<img src="https://imgur.com/fVLzMva.jpg"  height="80%" width="80%">
<img src="https://imgur.com/ZASzJkt.jpg"  height="80%" width="80%">
<img src="https://imgur.com/L4zUbID.jpg"  height="80%" width="80%">
<br />

<h2> I configure each VM to forward logs to my SIEM via syslog and Splunk Universal Forwarder.</h2>
<br /> 
  
<br />
<img src="https://imgur.com/RSdnrjD.jpg"  height="80%" width="80%">
<img src="https://imgur.com/VT6pysM.jpg"  height="80%" width="80%">
<img src="https://imgur.com/VvRiHyq.jpg"  height="80%" width="80%">

<br />

<h2> After verifying and configuring each VM to forward logs, I verify logs are flowing into Splunk and check for Windows Event Logs, Linux auth logs, and Sysmon events</h2>
  
<br />
<br />

<img src="https://imgur.com/jyQYK4J.jpg"  height="80%" width="80%">
<img src="https://imgur.com/rJ7tjvK.jpg"  height="80%" width="80%">
<br />

<h2> Phase 2 Simulate Attacks --  I use Kali Linux to run controlled attack simulations against my Windows 10 VM.  </h2>


-  Nmap Port Scan (Network Reconnaissance)
-  Brute Force (Failed Logins)
-  Reverse Shell / C2 (Suspicious Process)
- File Drop / Malware (File Creation)
<br />

<br />

<img src="https://imgur.com/3ennHYG.jpg"  height="80%" width="80%">
<img src="https://imgur.com/WewCZ43.jpg"  height="80%" width="80%">
<img src="https://imgur.com/9m7HKTV.jpg"  height="80%" width="80%">
<img src="https://imgur.com/LwDzeHq.jpg"  height="80%" width="80%">
<br />

<br />
<br />

<br />
<br />


