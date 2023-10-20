<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration</h2>

- Enable ICMPv4 on the local Windows Firewall
- Installation and Configuration of Active Directory
- Create users and provide access to remote desktop

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/XfJGYvq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/p7sj3Xe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After setting up both the Domain Controller and Client 1 on Microsoft Azure, I ran a ping -t test from Client 1 and the first image shows what occured before I enabled the ICMPv4.  The second image shows after I went into the Domain Controller and enabled the ICMPv4 on the local windows firewall, which you can see is allowing a reply from the Domain Controller.
</p>
<br />

<p>
<img src="https://i.imgur.com/LYCQ1Uc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/zz1t9tQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/LtvSN0Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Active Directory has been installed on the Domain Controller. I went into Active Directory and created Organizational Units for Employees and Admins. I then added in a new admin and added the admin into the Domain Admins group.
</p>
<br />

<p>
<img src="https://i.imgur.com/arVIbTF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/wQF5vhT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/Lfmi0Nm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Active Directory has been configured I went in and created multiple new users who can now access the computers on the domain. I also went in and allowed all domain users acces to the remote desktop.
</p>
<br />
