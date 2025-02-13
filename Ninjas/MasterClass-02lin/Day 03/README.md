# Day 03 Notes  EC2 instance host ubantu default page and replce the homepage 
 <img src="assets/14.png" height="350px" width="500px" />

### 1. create a VM instance in AWS 
<img src="assets/1.png" height="350px" width="500px" /> 



<img src="assets/2.png" height="350px" width="500px" /> 
 Named the server as 'webseverDay03',and select OS 'ubuntu' 



<img src="assets/3.png" height="350px" width="500px" />
Create key pairs 



<img src="assets/4.png" height="350px" width="500px" />
Allow SSH ,HTTP ,HTTPS traffic 



<img src="assets/6.png" height="350px" width="500px" />
Connect to the VM 



### 2. install git in AWS instance -vm server
<img src="assets/7.png" height="350px" width="500px" />
sudo apt-get update



<img src="assets/8.png" height="350px" width="500px" />
sudo apt install git-all


### 3. install LAMP server 
<img src="assets/9.png" height="350px" width="500px" />
<img src="assets/10.png" height="350px" width="500px" />
git clone https://github.com/anuvindhs/GFS-Moo git
The GFS-Moo folder contains an automation script designed to help install and configure a set of services on Linux servers, including the LAMP stack 



<img src="assets/11.png" height="350px" width="500px" />
 install lamp server 



### 4. config -index.html within lamp server
<img src="assets/12.png" height="350px" width="500px" />
Using SSH connect to VM 



<img src="assets/13.png" height="350px" width="500px" />
https://13.236.60.86/ OR click Instances -13.236.60.86 | open address , the homepage apprears 
 



### 5. test by a new index.html 
<img src="assets/15.png" height="350px" width="500px" />
Reomved the original index.html 



<img src="assets/16.png" height="350px" width="500px" />
Homepage replaced 






