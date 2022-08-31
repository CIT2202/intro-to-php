# Uploading Files to Selene

* From the start menu open FileZilla

* Enter the following settings
  * Host: sftp://selene.hud.ac.uk
  * Username: u0123456 (your student number)
  * Password : The same password you use to log into the university PCs
  * Click 'Quickconnect'.

You should then be able to move files from the local machine to your user space on the Selene web server.

* The URL of any files you move over will be http://selene.hud.ac.uk/student_number/folder_name/name_of_file.php e.g. if your student number is u1876543 and you move a folder onto selene called assign1 and inside this folder is a file named test.php, to view this page in a browser you would enter http://selene.hud.ac.uk/u1876543/assign1/test.php.

## Important!
Selene is a Linux web server. It is case sensitive with respect to filenames. For example, using the following ```<link>``` element
```
<link rel="stylesheet" type="text/css" href="style.css">
```
 to link to a file named **Style.css** will work fine in the PC labs. However, if we then upload the files to the Selene server, the link will no longer work (notice the capital 'S' in the file name).
