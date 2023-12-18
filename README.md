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

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/7bdff5a9-f0da-4e21-a369-01e6c4c38b02)


Step two is to download all material needed to install osTicket or Remote Desktop in to download the materials
Begin with enabling or installing IIS (Internet Information Systems) in Windows.
During the install process of this ensure these folders are checked
![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/4d102372-8387-4a18-9c13-62e3c3930eb5)

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/6aebaead-9d40-4518-875d-9dc4e123b6a8)

Then hit the expand button on World Wide Web Services 
Then expand Application Development Features and ensure that CGI is enabled

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a3501fe5-f7b2-4095-bb52-518e3cda15f2)

Then expand Common HTTP Features and enable all check boxes

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/4a12df17-2a09-48ef-a340-ab88314fbf0b)

After all the boxes are checked click "ok" and it will begin a download and apply the changes.
To ensure that it is installed and functioning go to a web browser and enter "127.0.0.1" into the search bar
If installed properly you will see this page
![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/d9df5bac-aee0-482a-8fc6-77e29cdd73f5)


<h2>Download and Install PHP Manager for IIS</h2>

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/70ea7023-04b8-4ea6-b194-acd5dd8e532e)
Click "Next" and then ensure "I Agree" is checked and then click "Next" again. A download should have started and once it is finished click "Close" and the download is finished.

<h2>Download and Install Rewrite Module</h2>

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/48aa5a17-ae13-4d38-9cf7-2d1d71480538)

Click "Install" and once that is complete click "Finish" and Rewrite is installed

<h2>Creating a PHP File and Downloading PHP</h2>

Go to the C: drive on your computer and create a file Named PHP

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/438adae4-4759-490f-9198-df35f950d329)

When PHP is downloaded it will be in a zip file. Right click it and hit "Extract all" and extract the files to the newly created PHP file on the C: drive.

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/4f81fbee-b517-4025-9af5-d0f1aeaaea81)


<h2>Download and Install Microsoft Visual C++ Redistributable</h2>

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/2f89b9a9-88d4-4f41-a301-b018aab972e1)

Click "Install" and once it is finished click "Close"

<h2>Download and Install MySQL</h2>

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/957591f3-5e44-4ca2-be2b-ffc52533e51f)

Once you are ready to install MySQL click "Next" and on the next page click the checkbox "I accept the terms..." and hit "Next"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/db574e7f-5242-4202-9f07-15ff6b38591c)

Click to do a "Typical" install and then click "Install"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/1ee70b34-73c1-4fd9-90c2-d576d49869d9)


Once you click "Finish" you will be asked to configure and setup information. Ensure you can access and properly record your configuration and information during setup. Click for a Standard Configuration

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a2cd725d-57eb-41ab-a591-541cf70dbf10)

For the next page leave it as it is

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/75201d91-f9b7-4c60-b588-5a4d1b46353a)

This last page contains the part of information to record. The password can be whatever you deem it to be and the username associated with this is default "root"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/68e3ad26-b360-4082-866f-686a74da1195)

Then hit Execute to let it run

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/901d83a8-da02-49dc-952b-d72b69f34a51)



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
