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

Step one is to create the virtual machines within Azure

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/7bdff5a9-f0da-4e21-a369-01e6c4c38b02)


Step two is to download all material needed to install osTicket or Remote Desktop in to the computer to download the materials


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

Click "Next" and then ensure "I Agree" is checked and then hit "Next" again. A download should have started and once it is finished select "Close" and the download is finished.

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/70ea7023-04b8-4ea6-b194-acd5dd8e532e)

<h2>Download and Install Rewrite Module</h2>

Click "Install" and once that is complete select "Finish" and Rewrite is installed

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/48aa5a17-ae13-4d38-9cf7-2d1d71480538)


<h2>Creating a PHP File and Downloading PHP</h2>

Go to the C: drive on your computer and create a file Named PHP

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/438adae4-4759-490f-9198-df35f950d329)

When PHP is downloaded it will be in a zip file. Right click it and hit "Extract all" and extract the files to the newly created PHP file on the C: drive.

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/4f81fbee-b517-4025-9af5-d0f1aeaaea81)


<h2>Download and Install Microsoft Visual C++ Redistributable</h2>

Click "Install" and once it is finished hit "Close"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/2f89b9a9-88d4-4f41-a301-b018aab972e1)


<h2>Download and Install MySQL</h2>

Once you are ready to install MySQL click "Next" and on the next page check the checkbox "I accept the terms..." and hit "Next"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/957591f3-5e44-4ca2-be2b-ffc52533e51f)

Check to do a "Typical" install and then click "Install"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/db574e7f-5242-4202-9f07-15ff6b38591c)

Once you click "Finish" you will be asked to configure and setup information. Ensure you can properly record your configuration and information during setup. Check for a Standard Configuration

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/1ee70b34-73c1-4fd9-90c2-d576d49869d9)


![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a2cd725d-57eb-41ab-a591-541cf70dbf10)

For the next page leave it as it is

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/75201d91-f9b7-4c60-b588-5a4d1b46353a)

This last page contains the part of information to record. The password can be whatever you deem it to be and the username associated with this is by default "root"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/68e3ad26-b360-4082-866f-686a74da1195)

Then hit Execute to let it run

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/901d83a8-da02-49dc-952b-d72b69f34a51)


<h2>Register PHP through IIS</h2>

Open IIS as Admin

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a2606f72-bb65-4d69-b907-1778894f0a17)

- Register PHP from within IIS
- Double click PHP Manager to get inside it

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/420306d5-48a5-49d7-84e1-1c50a96d4f16)

- Once there select "Register new PHP version"
- When prompted route it to the PHP file made under the C: drive and look for the PHP CGI file

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/f456f98d-8566-4826-acb6-01a0106a042b)

- Reload IIS by clicking on the name of the program in the left bar and finding "Restart" on the right side of the IIS box

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a703531a-67d1-43fc-acf8-344318202fa2)


<h2>Install osTicket</h2>

- Extract and copy "upload" folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename "upload" to "osTicket"
- Reload IIS

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/2ca42d38-f094-46bd-903e-833365e0bc6c)

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/fad7c2c9-07e4-4efb-8e0f-3f3a91a61ba4)

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/5fddf49d-82e9-4f29-988a-e41c86610a5e)

- Once finished Restart IIS once again
- Go to sites and open the drop down to see Default Web Site
- Hit the drop down button Default Web Site
- Select osTicket
- On the right, click "Browse *.80"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a614f99c-163d-4a49-b22a-b6da8088a5eb)

If it has worked properly you should see this screen

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/50926a6e-3adf-4212-b2c8-276a8114bfb2)


Note that some extensions are not enabled by default
Enable the following folders in IIS by clicking the PHP Manager

Once on this screen under the PHP Extensions section click on on Enable or disable extensions and enable the following extensions
- php_imap.dll
- php_intl.dll
- php_opache.dll


![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/de90e269-6cd1-4d87-bbd4-a911d5db9c63)

As they are enabled go back to your browser with osTicket and Refresh the page. There should be more green features than previously.

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/ca8f029d-efa4-4c2a-97fa-95c823f573ec)


<h2>Rename</h2>
Next is to change file names inside of the osTicket folder within the wwwwroot folder

- change from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- change to   C:\inetpub\wwwroot\osTicket\include\ost-config.php

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/a9af74ae-eaa0-4266-917a-080567e2014a)

It should be named like this now

Next is to assign permissions to that file

- Right click on ost-config.php and select properties
- Click the Security tab up top
- Then click advanced
- Click Disable inheritance
- Remove all permissions
- Click Add
- Click Select a principal
- Type in "everyone" and click check names then click OK
- Click "Full control" then hit OK
- Then click Apply after that click OK and then click OK again

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/843f7136-0c0f-4821-bcea-c04983bd8c09)



<h2>Continue osTicket system</h2>
Continuing in the web browser setup of osTicket. Hit "Continue" on the bottom of the page

This section can be setup as desired but ensure that the information is saved for later use

Once the two sections are entered the Database Settings section on the bottom will wait until Heidi SQL is installed

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/d539de7f-a92d-4d2f-93c0-3bec50d8a294)


<h2>Download and Install HeidiSQL</h2>

-  Open Heidi SQL
-  Click OK through everything and ensure it will launch once finished installing
-  Create a new session, root/Password1
-  Connect to the session
-  Create a database called "osTicket"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/af60ba2d-370d-4f13-8a64-fb71bd5d2ac2)

Once logged in you will see the following

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/59c8835f-7f04-4460-bbea-878245071bd2)

- Right Click Unnamed at the top left of the Heidi SQL box and select Create New/Database
- Name the new Database osTicket and then click OK

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/92ecb165-9c79-4793-8a9f-6323769ce7c9)



<h2>osTicket Continued</h2>
Back on the webpage of osTicket finish filling out the Database Settings section

- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: password1
- Click "Install Now!"

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/33ee6b25-ec82-4eca-8b3c-c0ea657b6bfc)



![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/926d8e39-1d1c-43bf-ab3c-8acd4417d9c6)


<h2>Cleanup Process</h2>

- Delete the "setup" folder within the osTicket folder under wwwroot folder
- Then go into the include folder under the same section of osTicket
- Change the permissions of the ost-config.php file back to "Read Only"
- Right click the file and select properties
- Click the security tab and then select Advanced
- Select Everyone and then click Edit
- Change Read & Execute and Read to the only permissions checked

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/37b9bf0a-bba4-4255-829d-9ca607aee227)


![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/5bdb705e-74fb-4788-8b95-e3efa2318861)

- Select Ok and then Apply
- Click the link on the Webpage for Staff login on the osTicket page and attempt to login as admin

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/4e0409aa-b23a-47bc-924c-89024a2ac973)

![image](https://github.com/CamdenMarshall/osticket-prereqs/assets/153537343/e0204cc0-ab2e-4c56-bcda-5c045319102f)


<h2>Install Process is over!</h2>
