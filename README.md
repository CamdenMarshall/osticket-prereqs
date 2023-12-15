<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
 <h1>osTicket-Prerequisites and Installation Process</h1>
 The following will detail the required materials and process to install the open-source help desk ticketing system osTicket.

 <h2> Materials Used in Demonstration </h2>

 - Microsoft Azure (Virtual Machines and Network)
 - Windows 10 Operating System (Virtual Machines)
 - osTicket
 - Remote Desktop
 - IIS (Internet Information Services)
 - Microsoft Redistributable C++
 - PHP Manager
 - HeidiSQL

<h2> List of Prerequisites </h2>

-  osTicket
-  Windows 10
-  Remote Desktop
-  Internet Information Services
-  PHP Manager
-  Rewrite Module
-  Microsoft Visual C++ Redistributable
-  MySQL Server

<h2>Installation Process</h2>

Step one is to create the virtual machines and virtual network within Azure

Step two is to download all material needed to install osTicket
Begin with enabling or installing IIS (Internet Information Systems) in Windows
During install process of this ensure these folders are checked
(Screenshot the process here)

<h2>Download and Install PHP Manager</h2>
(Screenshot Process here)

<h2>Download and Install Rewrite Module</h2>
(Screenshot Process here)

From the install files download PHP 7.3.8 (Outdated files but this method still works)
(Screenshot this process)

Download and Install Microsoft Visual C++ Redistributable
(Screenshot this process)

<h2>Download and Install MySQL</h2>

You will be asked to configure and setup information. Ensure you can access and properly record your configuration and information during setup.
(Screenshot this process)

Open IIS as Admin

Register PHP from within IIS

Reload IIS

<h2>Install osTicket</h2>
-Extract and copy "upload" folder to c:\inetpub\wwwroot
-Within c:\inetpub\wwwroot, Rename "upload" to "osTicket"
-Reload IIS

Go to sites -> Default -> osTicket
-On the right, click "Browse *.80"

Note that some extensions are not enabled by default
Enable the following folders
(try to do Screenshots)

- php_imap.dll
- php_intl.dll
- php_opache.dll

<h2>Rename</h2>
change from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php

change to   C:\inetpub\wwwroot\osTicket\include\ost-config.php

Assign Permissions

-Disable inheritance > Remove All
-New Permissions > Everyone > All

Continue osTicket system

- Name Helpdesk
- Defauly email (receieves email from customers)

<h2>Download and Install HeidiSQL</h2>

-  Open Heidi SQL
-  Create a new session, root/Password1
-  Connect to the session
-  Create a database called "osTicket"

<h2>osTicket Continued</h2>

- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: Password1
- Click "Install Now!"

<h2>Install Process should be over!</h2>
