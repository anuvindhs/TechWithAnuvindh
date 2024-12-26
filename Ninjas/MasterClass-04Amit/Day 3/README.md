## **Progress and Activities**

### **1. Reviewing Day 2 Exercise**  
Remove all personal information from public repo, including SSH keys and email addresses for security.

---

### **2. AWS Lab**
In this lab a VM (EC2) is spun up in AWS with Ubuntu image, Git is installed for ease and speed of development and LAMP server is installed to host a custom website.
#### **Steps to create and configure EC2 virtual machine**
 <img src="Assets\ec1.jpg" alt="ec1" width="500">

1. **Create EC2 virtual machine with Ubuntu image** 
   <img src="Assets\ubuntu1.png" alt="ubuntu1" width="500">

2. **Create SSH Key to enable access to VM**  
   <img src="Assets\SSHcreate1.png" alt="SSHcreate1" width="500">

3. **Create a security group**  
   Configure access to the VM using the SSH protocol (port 22).  
   <img src="Assets\securitygroup1.png" alt="securitygroup1" width="500">

4. **Download code for future deployment and launch the instance**  
   <img src="Assets\launchinstance1.png" alt="launchinstance1" width="500">

5. **Connecting to the VM through desktop browser**  
   <img src="Assets\VMconnect1.png" alt="VMconnect1" width="500">  


   <img src="Assets\VMconnect2.png" alt="VMconnect2" width="500">  


   <img src="Assets\VMconnect3.png" alt="VMconnect3" width="500">


6. **Install Git on the server** 

To get the latest version use command: sudo apt-get update
<img src="Assets\VMconnect4.png" alt="VMconnect4" width="500">

To install Git use command: sudo apt install git-all
<img src="Assets\VMconnect5.png" alt="VMconnect5" width="500">

7. **Install LAMP server** 

LAMP server is a common software bundle with Linux, Apache, MySQL Perl/PHP/Python used for web applications.

<img src="Assets\VMconnect6.png" alt="VMconnect6" width="500">

a) This command uses git to clone the repository located at https://github.com/anuvindhs/GFS-Moo.git to the local machine.

git clone https://github.com/anuvindhs/GFS-Moo.git

b): This command lists the files and directories in the current directory and confirms GFS-Moo directory has been created.

ls

c): This command changes the working directory to GFS-Moo, allowing the user to work within the cloned repository.

cd GFS-Moo/

d) This command lists the files and directories in the current directory, showing the install.sh file.

ls

e) This command uses changes the mode to administrative privileges in order to execute the install.sh file.

sudo chmod +x install.sh

f) This command runs the install.sh script in the current directory.

./install.sh

g) Enter Option 1 to install the LAMP server.

8. **Connecting to VM through terminal using SSH** 

Shift right-click to open git bash in the downloads folder where SSH is located.
<img src="Assets\VMconnect7.png" alt="VMconnect7" width="500">

Copy the SSH client key information found in the instance into the gitbash to connect to the virtual machine from the local machine. The advantage of this method is that the session does not expire like the desktop browser and therefore is the preferred method.
<img src="Assets\VMconnect8.png" alt="VMconnect8" width="500">

Enter the public address of the virtual machine in a web browser to verify the LAMP server has been successfully installed.

<img src="Assets\VMconnect9.png" alt="VMconnect9" width="500">

9. **Updating the file structure with own website** 

a) Navigate to the root folder and go to the var, www location for the Apache server.

ls

Cd /

Clear

<img src="Assets\VMconnect10.png" alt="VMconnect10" width="500">


Cd var

Cd www

Cd html

<img src="Assets\VMconnect11.png" alt="VMconnect11" width="500">

b) To remove the default Apache 2 index html file from the root folder.

Sudo su

Rm -r index.html

Clear

<img src="Assets\VMconnect12.png" alt="VMconnect12" width="500">

c) Clone the index html file of the custom website to the root folder.

<img src="Assets\VMconnect13.png" alt="VMconnect13" width="500">

