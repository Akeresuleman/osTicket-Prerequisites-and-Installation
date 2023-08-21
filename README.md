<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create Virtual Machine in Azure
- Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
- download and install PHP Manager for IIS 
- download and install the Rewrite Module 
- download PHP 7.3.8 and unzip the contents into C:\PHP
- download and install VC_redist.x86.exe.
- download and install MySQL 5.5.62
- Register PHP from within IIS
- Install and setup osTicket v1.15.8
- download and install HeidiSQL.

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/duHHYZX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://imgur.com/AQDPGIB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I created a virtual machine in Azure as shown on the screenshot above, and logged in to the vm using Remote Desktop. I then Install / Enable IIS in Windows WITH CGI and Common HTTP Features and IIS Management Console and to make sure the IIS features was enabled successfully I searched 127.0.0.1 on my browser. The features to be enable are shown on the screenshot above

</p>
<br />

<p>
<img src="https://imgur.com/jqmKoqM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created a PHP folder in Local Disk C
  Downloaded and installed PHP Manager for IIS, Rewrite Module. Dowloaded PHP 7.3.8 and unzip the contents into C:\PHP. Downloaded and install VC_redist.x86.exe and MySQL 5.5.62. Registered PHP from within IIS(open IIS as admin).

<p>
<img src="https://imgur.com/dAiWUzF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Dowloaded, Installed and setup osTicket v1.15.8:
Extract and copy “upload” folder to c:\inetpub\wwwroot. Within c:\inetpub\wwwroot, Rename “upload” to “osTicket.Reload IIS and click "browse 80" on the right. Some extensions are still disabled so to enable them double-click PHP Manager then Click “Enable or disable an extension”.Enable: php_imap.dll, php_intl.dll and php_opcache.dll. Refresh the osTicket site in your browse, observe the changes. Rename: ost-config.php to ost-config.php. Assign full Permissions for everyone to            ost-config.php. Click continue on the osTicket in the browser

<p>
  
<https://imgur.com/CB9QQvH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <https://imgur.com/OY7ihsc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- download and install HeidiSQL
  Open Heidi SQL,Create a new session, root/Password1,Connect to the session and Create a database called “osTicket.
  Fill the osTicket System as follows
MySQL Database: osTicket
MySQL Username: root
MySQL Password: Password1
Click “Install Now!”. Finally Browse to your help desk login page: http://localhost/osTicket/scp/login.php



</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
