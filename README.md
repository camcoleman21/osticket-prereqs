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
<img width="2868" height="1562" alt="image" src="https://github.com/user-attachments/assets/d33c3d89-6c3f-4dd7-9bc2-0358ba0a0928" />
</p>
<p>
Install / Enable IIS in Windows WITH CGI. World Wide Web Services -> Application Development Features -> [X] CGI
</p>
<br />
