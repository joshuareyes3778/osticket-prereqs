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

- IIS must be enabled by enabling CGI and Common HTTP Features in Windows Features
- Have a web platform installed
- PHP Manager must be installed
- Having a PHP directory in the C: drive
- Install and create an account for MySQL
- Installing a C++ redistributable
- Installing HeidiSQLand connecting it to the mySQL server

<h2>Installation Steps</h2>


In order to begin installing osTicket, you will first need a machine to set all of this up on. A Windows 10 virtual machine was used in this example. The first thing that was done was that IIS needed to be enabled. This was done by enabling CGI, Common HTTP Features, and the IIS Management console all under "Turn Windows Features On or Off." Once this was set up and tested by going to 127.0.0.1, a PHP Manager and Rewrite Module were installed. In preparation for the next step, a directory of C:\PHP was created on the C drive. Then PHP 7.3.8 was downloaded and unzipped into the previously created c:\PHP directory. Two more things were installed: a C++ Redistributable and a MySQL server for osTicket to use. The MySQL server required a some credentials, so those were noted and used to complete the installation process. Now that all of this was set up, the PHP was registered from within IIS. After that, osTicket is ready to be installed. 
</p>
<br />

<p>
Once osTicket was installed, only a few more things needed to be done. Some extensions for osTicket were enabled from within IIS: "php_imap," "php_intl," and "php_opcache." At this time a file (C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig) was renamed to C:\inetpub\wwwroot\osTicket\include\ost-config, simply removing the sample portion from the name. This same folder had its permissions changed to allow anyone to change them. This was done so that the osTicket program could edit the data within properly. After downloading osTicket, a browser page came up showing the status of it and its necessary extensions. With this prior step completed, it was ready to be set up for its basic installation in a browser. One last program that was installed was HeidiSQL. A new session was created and connected to. A database called "osTTicket" was created for osTicket to use. After this the credentials to log into osTicket were created and the program was finally installed for use.
</p>

