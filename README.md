<p align="center">
<img width="700" height="208" alt="image" src="https://github.com/user-attachments/assets/21a22a2f-c734-453b-b4b2-f4b0e0b7cd01" />
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Download osTicket Installation Files and Rewrite Module
- Creating PHP directory and installing VC and MySQL
- Registering PHP from IIS
- Install osTicket v1.15.8
- Final osTicket configurations

<h2>Installation Steps</h2>

<p>
<img width="2872" height="1472" alt="image" src="https://github.com/user-attachments/assets/3c74772c-e180-4760-9371-567f33cfe3e7" />
</p>
<p>
Create an Azure Virtual Machine Windows 10, 4 vCPUs. Log in to the VM with Remote Desktop.
</p>
<br />

<p>
<img width="2880" height="1726" alt="image" src="https://github.com/user-attachments/assets/106cd24a-1669-4933-af18-4066ae9aab82" />
</p>
<p>
Within the VM, download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”</p>
<br />

<p>
<img width="2868" height="1562" alt="image" src="https://github.com/user-attachments/assets/d33c3d89-6c3f-4dd7-9bc2-0358ba0a0928" />
</p>
<p>
Install / Enable IIS in Windows WITH CGI. World Wide Web Services -> Application Development Features -> [X] CGI
</p>
<br />

<p>
<img width="2880" height="1518" alt="image" src="https://github.com/user-attachments/assets/d80dff20-ddd3-43fe-86af-80546e5cf392" />
</p>
<p>
From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)</p>
<br />

<p>
<img width="2880" height="1508" alt="image" src="https://github.com/user-attachments/assets/33b06650-7279-44f3-80b1-31bc6879baaf" />
</p>
<p>
From the “osTicket-Installation-Files” folder, install the Rewrite Module (rewrite_amd64_en-US.msi)
</p>
<br />

<p>
<img width="2880" height="1714" alt="image" src="https://github.com/user-attachments/assets/91458d99-d538-4269-84c3-66a39017d3ea" />
</p>
<p>
Create the directory C:\PHP. From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder. </p>
<br />

<p>
<img width="2880" height="1478" alt="image" src="https://github.com/user-attachments/assets/92074847-f47d-44a5-8a0b-e8115cbff55c" />
</p>
<p>
From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe. </p>
<br />

<p>
<img width="2880" height="1578" alt="image" src="https://github.com/user-attachments/assets/1024ead9-a374-46fe-a8d9-9398a31627e0" />
</p>
<p>
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi). Typical Setup -> Launch Configuration Wizard (after install) -> Standard Configuration -> enter username and password.  </p>
<br />

<p>
<img width="2400" height="1558" alt="image" src="https://github.com/user-attachments/assets/bbd596f3-952d-4340-8a61-ae09c6bc0cb1" />
</p>
<p>
Open IIS as an Admin. Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe) </p>
<br />

<p>
<img width="1172" height="740" alt="image" src="https://github.com/user-attachments/assets/1d71e153-00b6-4ccb-9c2f-1a61dfda7029" />
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) </p>
<br />

<p>
<img width="2880" height="1708" alt="image" src="https://github.com/user-attachments/assets/0952bed7-d55f-4e29-be8b-32ee269cfa99" />
</p>
<p>
Install osTicket v1.15.8. From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”. Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”. </p>
<br />

<p>
<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/af4e0cb1-da9d-474e-9b3b-8010a5016582" />
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) Go to sites -> Default -> osTicket. On the right, click “Browse *:80” </p>
<br />

<p>
<img width="1172" height="740" alt="image" src="https://github.com/user-attachments/assets/1d71e153-00b6-4ccb-9c2f-1a61dfda7029" />
</p>
<p>
Go back to IIS, sites -> Default -> osTicket. Double-click PHP Manager, and click “Enable or disable an extension”. Enable php_imap.dll, php_intl.dll, and php_opcache.dll. Refresh the osTicket site in your browser, and observe the changes. </p>
<br />

<p>
<img width="1172" height="740" alt="image" src="https://github.com/user-attachments/assets/1d71e153-00b6-4ccb-9c2f-1a61dfda7029" />
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) </p>
<br />

<p>
<img width="1172" height="740" alt="image" src="https://github.com/user-attachments/assets/1d71e153-00b6-4ccb-9c2f-1a61dfda7029" />
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) </p>
<br />

<p>
<img width="1172" height="740" alt="image" src="https://github.com/user-attachments/assets/1d71e153-00b6-4ccb-9c2f-1a61dfda7029" />
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server) </p>
<br />
