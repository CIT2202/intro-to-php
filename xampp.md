# Getting started with XAMPP Portable

A good way to do the work for this module is to install a web server and database on a memory stick. You can then use this when at home and when you come into university.

The following explains how to install XAMPP (Cross-platform(X), Apache(A),Mysql/MariaDB(M), PHP\(P\), Perl\(P\))

Installing and getting up and running with XAMPP is easy but you need to make sure you download the correct version. I'm suggesting we use PHP version 7.3, and you need to **MAKE SURE YOU DOWNLOAD THE ZIP AND NOT THE .EXE**.

Open a browser and go to https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/7.3.20/

Download *xampp-portable-windows-x64-7.3.20-0-VC15.zip*. Unzip the resulting file into the **root** of your USB drive. It might take a bit of time.

> What do I mean by the root of the USB? When you view the files on the USB there should be a folder called XAMPP. You shouldn't have to click into any other folders first. When you go into the XAMPP folder there should be a file called xampp-control.exe.

* Navigate to this folder and click on xampp-control.exe.
* You might need to select a language
* A control panel should open
* Start the Apache web server
* Start MySQL
* Open a web browser and point it at http://localhost. You should see the xampp homepage.

## What to do if it doesn't work
Check the following:
1. You have downloaded the correct version. MAKE SURE YOU USE THE .zip. DON'T USE THE .exe.
2. You have unzipped the folder into the root of you USB drive. Do not put in a sub-folder.

## Where do I put my HTML, CSS and PHP files?
Your web applications are run from the *htdocs* folder.
* Navigate to the *htdocs* folder
* Create a new folder e.g. CIT2318
* Create a simple php page e.g. *test.php* and save it in the *CIT2202* folder
* Navigate to http://localhost/CIT2202/test.php to check it works.

## What can go wrong?
* You have to remember to stop Apache and MySQL before ejecting the USB.

## Important
* It is your responsibility to look after your USB drive.
* Back-up your work regularly
* Extensions to hand-in dates cannot be granted for lost or damaged USB drives.
