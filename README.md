<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure
- Basic Knowledge of IIS (Information Internet Services)
- Remote Desktop Access
- osTicket Installalation Files
- HeidiSQL

<h2>Installation Steps</h2>
<p>
 In Microsoft Azure, we will create a Virtual Machine and make a new resource group, "osTicket".

- **VM Name:** osTicket-vm
- **Image:** Windows 10 Pro, version 22H2 - 64x Gen 2
- **Size:** 2 vCPUs, 8 Gig Memory Minimum 
</p>
<br />

<p>
<img src="https://imgur.com/thkBVC0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I connect to the VM to install Internet Information Services with CGI in control panel
</p>
<br />

![image](https://github.com/user-attachments/assets/05887490-9897-42cf-aa82-8c74a41be66b)

<p>
From the “osTicket-Installation-Files” folder, install PHP Manager for IIS
</p>
<br />

![image](https://github.com/user-attachments/assets/7e9987a2-71f9-4c74-af88-7179f9fba855)

<p>
From the “osTicket-Installation-Files” folder, install the Rewrite Module
</p>
<br />

![image](https://github.com/user-attachments/assets/8d3b879f-0d78-4501-8b93-2af07dd316d2)

<p>
Now I create the directory C:\PHP, from the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder
</p>
<br />

![image](https://github.com/user-attachments/assets/8e5ad7af-062a-4715-a4f3-eee51ae410d2)

<p>
From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
</p>
<br />

![image](https://github.com/user-attachments/assets/e44a1ae3-71b4-41bd-8317-57c222517ad3)

<p>
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62. Then setup username and password to be root.
</p>
<br />

![image](https://github.com/user-attachments/assets/7deb807e-e6c5-421e-bfdb-e71949250bc6)


<p>
Now I open IIS as an Admin
</p>
<br />

![image](https://github.com/user-attachments/assets/cdd7b2f0-6b41-484e-a3c9-491409432400)

<p>
Register PHP from within IIS, then open IIS, stop and start the server
</p>
<br />

![image](https://github.com/user-attachments/assets/7a834e19-ba51-46c7-91ad-5a70d4622035)

<p>
Now I install osTicket v1.15.8 from the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”
</p>
<br />

![image](https://github.com/user-attachments/assets/4be852c8-d0e9-4e41-957d-f8ba0d99f31e)

<p>
Reload IIS again, go to sites and click Browse *80 which opens the osticket installer page
</p>
<br />

![image](https://github.com/user-attachments/assets/b9d92669-52db-4747-ba48-fb830af610ef)


<p>
Now I open IIS as an Admin
</p>
<br />

