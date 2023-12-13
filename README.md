<h1>Active Directory Home Lab</h1>

<!-- ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo) -->

<h2>Description</h2>
<b>Active Directory Home Lab: Build Your Own Network from Scratch</b>
 <br/>
 <br/>
This project guides you through building a <b>functional Active Directory home lab environment.</b> <br/>You'll learn to:<br/>
<br/>

- <b>Manage user accounts and permissions</b> with Active Directory Domain Services (AD DS)<br/>
- <b>Set up network connectivity</b> with internal NICs, DHCP, and RAS/NAT<br/>
- <b>Automate tasks with PowerShell scripts</b><br/>


<b>Step-by-step instructions:</b> Clear and concise guides for each stage.<br/>
<b>Image illustrations:</b> Visual aids to enhance understanding.<br/>
<b>PowerShell automation:</b> Learn to automate user creation with a provided script.<br/>
<b>Fully functional network:</b> Connect your Windows 10 client to the domain and access the internet.<br/>
<br/>
<b>Benefits:</b><br/>

<b>Deepen your understanding of Active Directory:</b> Gain hands-on experience with essential AD DS concepts.<br/>
<b>Develop network administration skills:</b> Learn valuable skills for managing network infrastructure.<br/>
<b>Practice PowerShell scripting:</b> Automate tasks and improve your efficiency.<br/>
<br/>
<b>Ready to build your own Active Directory home lab?</b> Dive into this project and gain practical skills in managing user accounts, network connectivity, and automation!<br/>

<h2>Languages and Utilities</h2>

- <b>PowerShell</b>
- <b>Linux (CLI)</b>
- <b>Server Manager (Domain Controller)</b>

<!--- <b>Diskpart</b>--!>

<h2>Environments</h2>

- <b>Windows 10</b> (21H2)<br>
- <b>Windows Server 2019</b><br/>
- <b>Virtualization Platform:</b> Oracle VM VirtualBox<br/>

<h2>Architecture</h2>
<p align="center">
<img src="https://i.imgur.com/B8c8teJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<h2>Program walk-through</h2>
<ul>
  <li><b>Prerequisites & Basic Installation:</b></li>
</ul>

VirtualBox Installation & Setup: <br/>
<br/>
<p align="left">
<img src="https://i.imgur.com/o7WZbRL.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/fLR3fMO.png" height="45%" width="45%" alt="Disk Sanitization Steps"/> <br/>
<br/>
Setting up Internal NIC (Network Interface Cards) for WindowsServer2019: <br/>
<br/>
<img src="https://i.imgur.com/OLOXuyU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>

<ul>
  <li><b>Setting up AD DS (Active Directory Domain Service):</b></li>
</ul>
AD DS Installation: <br/>
<br/>
<img src="https://i.imgur.com/f5X8I7x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
AD DS a-aparulekar: <br/>
<br/>
</ul>
<img src="https://i.imgur.com/ohrnyKn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

<ul>
  <li><b>Setting up RAS / NAT:</b></li>
</ul>
Remote Access Service / Network Address Translation <br/>
Purpose of RAS/NAT is to allow a Windows 10 client to be on the private virtual network & still be able to access the internet through the Domain Controller.  <br/>
<br/>
RAS / NAT Installation: <br/>
<br/>
<img src="https://i.imgur.com/Aom9nDs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
RAS / NAT is Configured & Up: <br/>
<br/>
</ul>
<img src="https://i.imgur.com/G0troom.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>

<ul>
  <li><b>Setting up DHCP Server:</b></li>
</ul>
Dynamic Host Configuration Protocol <br/>
DHCP allow our Windows 10 client to get an IP address that will let them get on the internet.<br/>
<br/>
DHCP Server Installation: <br/>
<br/>
<img src="https://i.imgur.com/YtatSd1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
DHCP is Configured & Up: <br/>
<br/>
</ul>
<img src="https://i.imgur.com/8rDEHy7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>

<ul>
  <li><b>PowerShell Script:</b></li>
</ul>
PowerShell script is attached <br/>
This PowerShell script generates 1000+ names for our dummy users<br/>
<br/>
<pre>
<code>
Set-ExecutionPolicy Unrestricted
</code>
</pre>

<br/>
<img src="https://i.imgur.com/tjRYroW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

<ul>
  <li><b>Windows 10 Client Installation:</b></li>
</ul>
For Internal Network only.<br/>
<br/>
<img src="https://i.imgur.com/N5zzPRy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

Our Network Infrastructure is working properly:<br/>
<br/>
<img src="https://i.imgur.com/gHnNp0T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

We have 1 lease from our client computer(in Domain Controller):<br/>
<br/>
<img src="https://i.imgur.com/fiqQmay.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

Computer is listed in Active Directory:<br/>
<br/>
<img src="https://i.imgur.com/jUX5qYj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>

Logged In successfully in one of the users:<br/>
<br/>
Example 01:<br/>
<br/>
<img src="https://i.imgur.com/sLx7LkH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>


Example 02:<br/>
<br/>
<img src="https://i.imgur.com/su7kRFx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<h2>Conclusion</h2>
This project provides a comprehensive guide for building and managing your own Active Directory home lab. Through detailed instructions, visual aids, and practical examples, you'll gain valuable skills in network administration, user management, and automation.




























 
<!-- <br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> -->




<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
