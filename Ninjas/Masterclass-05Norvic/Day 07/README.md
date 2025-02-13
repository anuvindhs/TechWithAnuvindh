# Day 07 Notes

**CLI to start an EC2 instance in AWS**

-   aws ec2 start-instances --instance-ids i-0112c103482e2997d 

![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2007/Assets/CLIstart.png)

**To configure WordPress, create MySQL database**

-   sudo mysql -u root ("login as root user(-u) to local mysql server")

-   Create database WORDPRESS; 

-   CREATE USER wordpress@localhost IDENTIFIED BY '<your-password>'; ("Create user and password ")

-   GRANT SELECT,INSERT,UPDATE,DELETE,CREATE,DROP,ALTER  ("Grant access user to database")

-   -> ON wordpress.* ("database created")

-   -> TO wordpress@localhost; ("user")

-   FLUSH PRIVILEGES; ("ensures any changes to user permissions are applied")

-   quit ("exit mysql")

-   sudo service mysql start   ("Enable MySQL service")

**Configure WordPress to connect to the database**

-   sudo -u www-data cp /srv/www/wordpress/wp-config-sample.php /srv/www/wordpress/wp-config.php     ("give user(-u) to copy(cp) data from folder (/srv/www/wordpress/wp-config-sample.php) to this folder (/srv/www/wordpress/wp-config.php)")

-   sudo -u www-data sed -i 's/database_name_here/wordpress/' /srv/www/wordpress/wp-config.php   ("set wordpress which is the database name after database_name_here")

-   sudo -u www-data sed -i 's/username_here/wordpress/' /srv/www/wordpress/wp-config.php  /("set wordpress which is the username after username_here")

sudo -u www-data sed -i 's/password_here/<your-password>/' /srv/www/wordpress/wp-config.php   ("replace “<your-password>” to the set password")

-   helpful codes: search(se) insert(-i) Print command(cat) 

-   SHOW DATABASES;  ("show the databases created")
-   DROP DATABASES; “database name”; ("Delete database")

-   sudo -u www-data nano /srv/www/wordpress/wp-config.php ("use editor to put the code content below to secure the database")
-   https://api.wordpress.org/secret-key/1.1/salt/

-   Check Public IP from Instance to validate and login to Wordpress site
![Screenshot](/Ninjas/Masterclass-05Norvic/Day%2007/Assets/testwordpresssite.png)