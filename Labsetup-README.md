
<h2>Description</h2>
A functional home lab with a SIEM at the center. Collect logs from multiple sources, write detection rules for common attack techniques (from the MITRE ATT&CK framework), and build a visual dashboard that tells the story of what happened on my network.
<br />
<h2> Phase 1 </h2>
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

- I configure each VM to forward logs to your SIEM via syslog or the Splunk Universal Forwarder
  
<br />
<img src="https://imgur.com/RSdnrjD.jpg"  height="80%" width="80%">
<img src="https://imgur.com/VT6pysM.jpg"  height="80%" width="80%">
<img src="https://imgur.com/VvRiHyq.jpg"  height="80%" width="80%">


<br />
<br />
<br />

<br />
<br />


