# Day 06 Notes

**3 Tier Application in AWS**

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/3tierapplication.png)

**Installing and Configuring Wordpress deployed EC2 (Ubuntu)**

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/Wordpress.png)

- Git source code
- Apache Server, Php, MySQL || LAMP Server
- Deploy in EC2  
- Test
- Validate
- Repeat

**Codes in Gitbash:**

-   Git -v  ("Check if Git is available")
-   php -v  ("check if php is installed") 
-   Mysql –v  ("check if Mysql is installed") 
-   Sudo apt update -y  ("Updates list of packages and versions")
-   Sudo apt upgrade -y ("Upgrades outdated packages")
-   Sudo apt install apache2  ("install Apache2 web server") 
-   Validate Apache2 ("screenshot below"):

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/ValidateApache2.png)

***Install Wordpress in Ubuntu***

-   https://ubuntu.com/tutorials/install-and-configure-wordpress#1-overview

-   sudo apt install apache2 \ 				 ("install dependencies") 

                 ghostscript \ 

                 libapache2-mod-php \ 

                 mysql-server \ 

                 php \ 

                 php-bcmath \ 

                 php-curl \ 

                 php-imagick \ 

                 php-intl \ 

                 php-json \ 

                 php-mbstring \ 

                 php-mysql \ 

                 php-xml \ 

                 php-zip 

sudo mkdir -p /srv/www   ("make directory") 

sudo chown www-data: /srv/www  ("changing folder permission") 

curl https://wordpress.org/latest.tar.gz | sudo -u www-data tar zx -C /srv/www.  ("downloading wordpress site")

ls ("check directory contents")

***Configure Apache for Wordpress then create wordpress config file***

-   sudo nano /etc/apache2/sites-available/wordpress.conf ("Installs nano text editor to creat Apache site for Wordpress")
![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/nanoeditorconfigwordpress.png)

-   sudo a2ensite wordpress ("Enable the site but execute first ‘sudo systemctl reload apache2' ") 

-   sudo a2enmod rewrite ("Enable URL rewriting but execute first ‘sudo systemctl reload apache2’ ")

-   sudo a2dissite 000-default   ("Disable the default “It Works”)

-   Sudo nano /etc/hosts ("write config file and map hostname to Public IP of EC2 Instance")

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/editconfighostnametoPublicIP.png)

-   sudo service apache2 restart ("Restart apache") 

**Stop EC2 Instance using Cloudshell in AWS**

-   In Instance click up top ![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/CLIIcon.png)  in dashboard instance Cloudshell CLI 

-   aws ec2 stop-instances --instance-ids i-0112c103482e2997d 

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2006/Assets/CLIstop.png)

-   Public IP in AWS is random, if it stops then restarts 

-   Use Elastic IP Address to assign static IP address in AWS 