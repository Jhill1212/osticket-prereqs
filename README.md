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
Next we are going to install the "VC_redist" which is once again located in the osTicket installation files. Double click it and accept and install. Next we will install the "mysql" for data storage purposes. Double click it, hit next, accept then hit next and we are going to make it typical, then hit install. A new window should have appeared, hit next and choose the standard configuration and hit next, then hit next again, to avoid errors we will type "root" in both boxes then hit next, then execute.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we are going to open the IIS as an admin. So click the windows button and search for it, right click, run as administrator. Open the PHP manager as seen and click register new PHP version, navigate to the folder we created earlier and click on the "php-cgi.exe" file. This is our executable. Now press ok.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we need to restart the server. Do so by clicking restart, stop, then start it back up again. Now we are entering the last few steps. We are going to install osTicket itself. So lets go back to that osTicket zip folder and extract it. Now you should see two folders inside of this freshly extracted one. We are going to move the "upload" folder into the "wwwroot" folder. (C: inetpub -> wwwroot) then we will rename it to "osTicket". Now we need to stop and start the IIS again.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now on the left hand side we are going to go to sites and hit the drop down arrow, then default web site's drop down arrow, then osTicket and click that, on the right side there should be a "browse *80", click that. Now you should see the osTicket installer website but, before we get to wrapping this up lets activate some more of those permissions. Inside the IIS go back to the osTicket folder and click the PHP manager, click the Enable or disable extension button, and now enable the following [ php_imap.dll, php_intl.dll, php_opcache.dll ] And now we can go back and refresh the osTicket web page.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we need to delve back into some files. Navigate to the wwwroot folder, osTicket, Include, find "ost-sampleconfig.php" and rename the file "ost-config.php", then right click and go to properties, then security, then advanced, then we will disable inheritance, then we will add, select a principal, for the sake of the tutorial we will make it everyone then select full control, then apply.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we finished giving osTicket some permissions we can continue its installation. Head back to the website and hit continue, for the help desk name you can input whatever you like and also use any email that you see fit. For the admin user the email must be different from the one from before. Now before we finish setting this up we need to install one more thing, so pause for now after finishing the admin user and head back to the installation folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will now be installing "HeidiSQL". Now double click it, accept, next all the way and install it. Skip once it opens or you can donate if you feel inclined, click that new button, remember that password for this should be root unless chosen otherwise, now we can press open, now right click the seal looking thing on the left side of the screen labled "Unnamed" and create a new database and name it "osTicket" and now that we have that situated we can head back to the website.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we can fill out the database settings with all the info we just created. in the "MySQL Database" you will put osTicket, and then root for the username and password unless you have chosen differently, then hit install now. Now we can go to your login page with the following link (http://localhost/osTicket/scp/login.php) and congratulations you have successfully installed osTicket!
</p>
<br />
