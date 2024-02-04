# Failed-RDP-to-IP-Geolocation-Information

<h2>Description</h2>
The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.

The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell: Extract RDP failed logon logs from Windows Event Viewer</b> 
- <b>ipgeolocation.io: IP Address to Geolocation API</b>

<h2>Environments Used </h2>

<p align="center">
<b>Windows 10 VM on Azure</b>
</b>  
<img src="https://i.imgur.com/pp9sZgn.png" height="100%" width="100%" />

<p align="center">
<b>NIC Honeypot</b>
</b>  
<img src="https://i.imgur.com/phIMCDg.png" height="100%" width="100%" />


<p align="center">
<b>Sentinel</b>
</b>  
<img src="https://i.imgur.com/vF5BkAw.png" height="100%" width="100%" />

<p align="center">
<b>Log Analytic</b>
</b>  
<img src="https://i.imgur.com/JHFn9rP.png" height="100%" width="100%" />


<h2>Attacks from all over the worl coming in; Custom logs being output with geodata before and after 24 hours</h2>

![2023-09-19 13-22-25](https://github.com/TheSelected1/Failed-RDP-to-IP-Geolocation-Information/assets/130491577/61b78e27-b0ff-4b9b-9f9c-8b241108983c) height="100%" width="100%"

