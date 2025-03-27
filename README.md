# Networking Activities Lab 1 (Observing ICMP Traffic)
This lab kicks off a demo series of my networking and remote desktop skills. I use Microsoft Remote Connection to observe ICMP traffic between two Azure VMs. Using PowerShell, I ping one VM from the other and monitor the ICMP packets with Wireshark.


<h2>Programs, Languages, and Utilities Used</h2>

- <b>Microsoft Azure</b> 
- <b>Powershell</b>
- <b>Wireshark</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (23H2)

<h2>Program walk-through:</h2>

<p align="center">
Create resource group for Remote Desktop Lab  <br/>
<img src="https://i.imgur.com/8O4wdf7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Deploy Windows 11 virtual machine, new Vnet, and Subnet within resource group <br/>
<img src="https://i.imgur.com/JDoY4Ar.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Deploy Linux (Ubuntu) virtual machine, within the resource group, ensuring it's running on the same Vnet  <br/>
<img src="https://i.imgur.com/Q2zyZee.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connect to Windows 11 virtual machine with IP address using Remote Desktop Connection  <br/>
<img src="https://i.imgur.com/o4itvRG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Access WireShark through the Microsoft Edge browser in the virtual machine, and download the software  <br/>
<img src="https://i.imgur.com/OP295H2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Wireshark (Keeping all settings default is recommended)  <br/>
<img src="https://i.imgur.com/CV8Sqzw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/KWA87ft.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once Wireshark is installed, open up the program from the Windows Start menu <br/>
<img src="https://i.imgur.com/NoUCA73.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once Wireshark is open, click Ethernet and then click the Wireshark icon  <br/>
<img src="https://i.imgur.com/damiq4K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Examine Network Traffic of virtual machine and filter for ICMP traffic  <br/>
<img src="https://i.imgur.com/CiCxlgF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<img src="https://i.imgur.com/FRdpXJP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Obtain Private IP Address from Ubuntu/Linux virtual machine found in Azure
<img src="https://i.imgur.com/LO1KE3S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open Windows Powershell from the Windows Start menu in the Windows virtual machine
<img src="https://i.imgur.com/Ax7Ijqh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
In Windows Powershell, type "ping", followed by the Private IP Address from the Ubuntu virtual machine, and press Enter
<img src="https://i.imgur.com/16ybYeM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Examine the filtered Network Traffic of virtual machine in Wireshark applicatiion
<img src="https://i.imgur.com/Qpu6cQ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
