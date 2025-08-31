# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
In this I will show you what you need before, and walk you through on how to install OsTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11 Pro</b> (24H2)

<h2>List of Prerequisites</h2>

- Item 1: A device to install OsTicket onto.
- Item 2: A internet connection
- Item 3: A web browser
- Item 4: [This tutorial will be based on this folder](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)


<h2>Installation Steps</h2>

<p>
<img width="672" height="170" alt="PF1" src="https://github.com/user-attachments/assets/e2053b6f-8248-4d0e-8d5f-197cb705993d" />

</p>
<p>
First, download the folder and extract everything onto your desktop. These files will be used to not only download osTicket but also its dependencies.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, click the windows button and navigate to the control panel of your computer. Then navigate to uninstall programs and head to "Turn Windows features on or off" on the left side of the screen. In this screen you will want to check the Internet Information Services box and expand the drop-down menu for it.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From this drop down menu, expand the World Wide Web Services folder, Then expand the Application Development Features folder, and when here check the box for CGI. Then press ok. You may then load a web page in microsoft with the address "127.0.0.1"
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have done that, access the osTicket installation files that we extracted. Now we are going to install PHPManager. Double click it, hit next, agree and hit next. Now we are going to install the Rewrite module. Just agree and hit install. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we are going to make a new directory on the C-drive of your computer and we will name it "PHP". Right click the file explorer icon and click "File explorer" to open a new window for it. Go into the c-drive (This pc -> drop down menu, Windows (C:)). While here, right click and make a new folder and title it "PHP" and then open the new folder. Now go back to the osTicket files and right click the php zip file and extract it into the new folder we created.
</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we are going to install the "VC_redist" which is once again located in the osTicket installation files.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
