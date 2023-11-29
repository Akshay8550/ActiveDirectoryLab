<h1>Active Directory Home Lab</h1>

<!-- ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo) -->

<h2>Description</h2>
In this project we're going to walk through how to create an Active Directory home lab Environment using Oracle Virtual Box. Corfiguring and running this lab will definitely help develop understanding of how active directory and windows networking works, so I'd highly recommend running through it a couple times, ask questions where stuff is unclear, and eventually try to build it on your own without guid. Please let me know if you have any questions!
<br />

<h2>Languages and Utilities</h2>

- <b>PowerShell</b> 
<!--- <b>Diskpart</b>--!>

<h2>Environments</h2>

- <b>Windows 10</b> (21H2)<br>
- <b>Windows Server 2019</b>

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
`<br/>
Set-ExecutionPolicy Unrestricted<br/>
<br/>`
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
